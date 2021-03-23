---
title: Saya mendapatkan diblokir oleh akses bersyarat dengan perangkat gabungan domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036700"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="c3851-102">Saya mendapatkan diblokir oleh akses bersyarat dengan perangkat gabungan domain</span><span class="sxs-lookup"><span data-stu-id="c3851-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="c3851-103">**Alat yang sangat direkomendasikan**</span><span class="sxs-lookup"><span data-stu-id="c3851-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="c3851-104">[Alat pemecah masalah registrasi perangkat](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -alat yang membantu memecahkan masalah pendaftaran perangkat yang paling umum.</span><span class="sxs-lookup"><span data-stu-id="c3851-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="c3851-105">[Uji skrip konektivitas pendaftaran perangkat](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -skrip yang membantu memastikan bahwa perangkat bisa mengakses titik akhir pendaftaran perangkat di bawah akun sistem.</span><span class="sxs-lookup"><span data-stu-id="c3851-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="c3851-106">[Skrip pembersihan perangkat AZURE AD](https://github.com/mzmaili/AzureADDeviceCleanup) -skrip yang memungkinkan Anda mencari dan mengelola perangkat yang basi di lingkungan Anda.</span><span class="sxs-lookup"><span data-stu-id="c3851-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="c3851-107">Berikut adalah beberapa alasan umum mengapa akses bersyarat mungkin gagal menggunakan sebuah perangkat yang telah bergabung dalam domain (hibrid Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c3851-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="c3851-108">**Tidak ada AZURE AD PRT di perangkat** -Anda harus memastikan bahwa perangkat tersebut memiliki token refresh utama Azure AD (PRT).</span><span class="sxs-lookup"><span data-stu-id="c3851-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="c3851-109">Untuk informasi selengkapnya tentang PRT, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)ini.</span><span class="sxs-lookup"><span data-stu-id="c3851-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="c3851-110">Untuk memverifikasi apakah Anda memiliki Azure AD PRT, Anda bisa menjalankan `dsregcmd/status` perintah pada perangkat dan memverifikasi apakah "AzureAdPrt" sama dengan "ya".</span><span class="sxs-lookup"><span data-stu-id="c3851-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="c3851-111">Jika "AzureAdPrt" adalah "tidak", periksalah hal berikut ini:</span><span class="sxs-lookup"><span data-stu-id="c3851-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="c3851-112">**Apakah Anda memiliki lingkungan gabungan dengan AD FS, dan tidak dapat dijangkau dari jaringan rumah pengguna Anda**: dalam hal ini, pastikan bahwa titik akhir "usernamemixhe" dapat diakses dari ekspor.</span><span class="sxs-lookup"><span data-stu-id="c3851-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="c3851-113">Jika AD FS Anda berada di belakang VPN, pastikan pengguna tersambung ke VPN dan masuk kembali ke perangkat.</span><span class="sxs-lookup"><span data-stu-id="c3851-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="c3851-114">Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)ini.</span><span class="sxs-lookup"><span data-stu-id="c3851-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="c3851-115">**Apakah TPM perangkat rusak dan dengan demikian tidak dapat mengotentikasi perangkat**: centang "TPM. MSC" untuk melihat apakah status TPM "sudah siap".</span><span class="sxs-lookup"><span data-stu-id="c3851-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="c3851-116">Jika tidak, jalankan `dsregcmd/leave` dan biarkan perangkat bergabung kembali ke AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="c3851-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="c3851-117">Lalu, coba lagi.</span><span class="sxs-lookup"><span data-stu-id="c3851-117">Then, try again.</span></span> <span data-ttu-id="c3851-118">Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)ini.</span><span class="sxs-lookup"><span data-stu-id="c3851-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="c3851-119">**Anda menggunakan penyedia identitas pihak ketiga, yang tidak mendukung protokol WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="c3851-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="c3851-120">Seperti yang diuraikan dalam dokumen kami, perangkat gabungan Azure AD yang digabungkan tidak dapat berfungsi dalam kasus ini.</span><span class="sxs-lookup"><span data-stu-id="c3851-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="c3851-121">Silakan bekerja dengan penyedia identitas Anda untuk dukungan.</span><span class="sxs-lookup"><span data-stu-id="c3851-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="c3851-122">**Pengguna menggunakan browser Chrome tanpa akun Windows 10** atau **Chrome ekstensi Office tidak secara otomatis menggunakan PRT pada perangkat yang tergabung dengan AAD atau hibrid-AAD**: hal ini menyebabkan kegagalan setiap kebijakan akses bersyarat berbasis perangkat, dengan pesan kesalahan "perangkat tidak terdaftar" ditampilkan.</span><span class="sxs-lookup"><span data-stu-id="c3851-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="c3851-123">Untuk menggunakan browser Chrome dengan benar, Anda harus menginstal "Akun Windows 10" atau "ekstensi Office ke browser Chrome pengguna" melalui SCCM atau Intune.</span><span class="sxs-lookup"><span data-stu-id="c3851-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="c3851-124">Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)ini.</span><span class="sxs-lookup"><span data-stu-id="c3851-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="c3851-125">Jika tidak memungkinkan untuk mendorong ekstensi dari jarak jauh, beri tahu pengguna untuk menginstal secara manual salah satu ekstensi di atas untuk mengakses aplikasi di balik akses bersyarat berbasis perangkat.</span><span class="sxs-lookup"><span data-stu-id="c3851-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="c3851-126">Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)ini.</span><span class="sxs-lookup"><span data-stu-id="c3851-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="c3851-127">**Perangkat telah bergabung dengan benar AZURE AD, namun tidak sengaja dihapus atau dinonaktifkan, baik karena sinkronisasi dengan perubahan di AZURE AD Connect atau dari portal Azure**: jika hal ini terjadi, objek perangkat tidak lagi dikenali sebagai perangkat yang bersambungan penuh meskipun status "Azureadjoin" dan "PRT" muncul sebagai valid pada perangkat.</span><span class="sxs-lookup"><span data-stu-id="c3851-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="c3851-128">Untuk memperbaiki masalah ini, jalankan `dsregcmd/leave` pada perangkat yang terpengaruh dan biarkan mereka bergabung kembali dengan AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="c3851-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="c3851-129">Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)ini.</span><span class="sxs-lookup"><span data-stu-id="c3851-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="c3851-130">Jika perangkat Anda berada di Windows 10, pembaruan 1809, dengan proksi VPN/awan dan melihat masalah dengan status "AzureAdPrt" atau aplikasi apa pun dengan masalah SSO (Outlook tidak tersambung ke kotak surat meskipun Anda telah memiliki PRT), pastikan Anda memiliki patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) atau pembaruan kumulatif April [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) untuk mencegah kegagalan PRT pada mesin tersebut.</span><span class="sxs-lookup"><span data-stu-id="c3851-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















