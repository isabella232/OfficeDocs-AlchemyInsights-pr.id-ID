---
title: Tulis balik kata sandi tidak berfungsi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243368"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="07876-102">Tulis balik kata sandi tidak berfungsi</span><span class="sxs-lookup"><span data-stu-id="07876-102">Password Writeback is not working</span></span>

<span data-ttu-id="07876-103">**Saya mengalami masalah saat mengonfigurasi tulis balik kata sandi**</span><span class="sxs-lookup"><span data-stu-id="07876-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="07876-104">Tulis balik kata sandi adalah fitur Premium.</span><span class="sxs-lookup"><span data-stu-id="07876-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="07876-105">Pastikan bahwa Anda memahami persyaratan Lisensi:</span><span class="sxs-lookup"><span data-stu-id="07876-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="07876-106">Anda harus memiliki setidaknya satu lisensi yang ditetapkan di organisasi Anda</span><span class="sxs-lookup"><span data-stu-id="07876-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="07876-107">**Pengguna awan saja** -SKU Office 365 (O365) berbayar apa pun, atau Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="07876-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="07876-108">**Pengguna awan dan/atau di** tempat-Azure AD Premium P1 atau P2, mobilitas perusahaan + keamanan (EMS), atau mengamankan perusahaan produktif (SPE)</span><span class="sxs-lookup"><span data-stu-id="07876-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="07876-109">Untuk mempelajari selengkapnya tentang persyaratan lisensi, lihat [persyaratan lisensi untuk pengaturan ulang kata sandi layanan mandiri AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="07876-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="07876-110">Anda memiliki setidaknya satu akun administrator dan satu akun pengguna uji dengan salah satu lisensi yang sesuai.</span><span class="sxs-lookup"><span data-stu-id="07876-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="07876-111">Anda harus menyambungkan Azure AD Connect ke emulator pengontrol domain utama untuk mencari tulis balik untuk bekerja.</span><span class="sxs-lookup"><span data-stu-id="07876-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="07876-112">Anda bisa mengonfigurasi Azure AD Connect untuk menggunakan pengontrol domain utama dengan mengklik kanan pada **properti** konektor sinkronisasi direktori aktif, lalu memilih **Konfigurasikan partisi direktori**.</span><span class="sxs-lookup"><span data-stu-id="07876-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="07876-113">Dari sana, Cari bagian **pengaturan koneksi pengontrol domain** dan centang kotak berjudul **hanya gunakan pengontrol domain pilihan**.</span><span class="sxs-lookup"><span data-stu-id="07876-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="07876-114">Jika DC pilihan bukan emulator PDC, Azure AD Connect masih akan menghubungi PDC untuk memasukkan kata sandi.</span><span class="sxs-lookup"><span data-stu-id="07876-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="07876-115">Reset kata sandi telah dikonfigurasikan dan diaktifkan di penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="07876-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="07876-116">Untuk informasi selengkapnya, lihat [mengaktifkan pengguna untuk mereset kata sandi AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="07876-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="07876-117">Pastikan bahwa akun administrator yang digunakan untuk mengaktifkan tulis balik kata sandi adalah akun administrator awan (dibuat di Azure AD not on-Premises AD)</span><span class="sxs-lookup"><span data-stu-id="07876-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="07876-118">Anda memiliki satu atau beberapa Forest AD Deployment di tempat yang menjalankan Windows Server 2008 R2, Windows Server 2012, atau Windows Server 2012 R2 dengan paket layanan terbaru yang terinstal</span><span class="sxs-lookup"><span data-stu-id="07876-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="07876-119">Anda memiliki alat Azure AD Connect yang terinstal dan Anda telah menyiapkan lingkungan iklan Anda untuk sinkronisasi ke awan.</span><span class="sxs-lookup"><span data-stu-id="07876-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="07876-120">Sebelum menguji tulis balik kata sandi, pastikan bahwa Anda telah menyelesaikan impor lengkap dan sinkronisasi penuh baik dari AD maupun Azure AD di Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="07876-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="07876-121">Untuk mempelajari selengkapnya, Lihat cara melakukan [sinkronisasi penuh dan impor penuh di AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="07876-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="07876-122">**Saya mengalami masalah dengan konektivitas tulis balik kata sandi**</span><span class="sxs-lookup"><span data-stu-id="07876-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="07876-123">Mengunduh dan mengaktifkan versi terbaru [AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="07876-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="07876-124">Konfigurasi firewall: alat Azure AD Connect (1.1.443 dan yang lebih baru) akan memerlukan akses **https keluar** ke:</span><span class="sxs-lookup"><span data-stu-id="07876-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="07876-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="07876-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="07876-126">servicebus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="07876-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="07876-127">Izinkan koneksi idle bertahan setidaknya selama 2-3 menit</span><span class="sxs-lookup"><span data-stu-id="07876-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="07876-128">**Saya masih mengalami masalah dengan tulis balik kata sandi**</span><span class="sxs-lookup"><span data-stu-id="07876-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="07876-129">Jika Anda masih mengalami kesulitan, coba Nonaktifkan dan aktifkan kembali Layanan tulis balik kata sandi di alat Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="07876-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="07876-130">Untuk mempelajari selengkapnya, Lihat cara [menonaktifkan dan mengaktifkan kembali tulis ulang kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="07876-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
