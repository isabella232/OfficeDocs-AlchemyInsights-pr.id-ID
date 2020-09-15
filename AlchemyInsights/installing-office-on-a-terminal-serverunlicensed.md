---
title: Menginstal Office di terminal server-tanpa lisensi
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663120"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="4f2cf-102">Menginstal Office di server terminal</span><span class="sxs-lookup"><span data-stu-id="4f2cf-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="4f2cf-103">Untuk menyebarkan aplikasi Microsoft 365 untuk perusahaan di server Windows menggunakan layanan desktop jarak jauh (RDS), sebelumnya bernama Layanan Terminal:</span><span class="sxs-lookup"><span data-stu-id="4f2cf-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="4f2cf-104">Anda harus memiliki langganan Microsoft 365 yang menyertakan aplikasi Microsoft 365 untuk perusahaan, seperti Office 365 Enterprise E3 atau Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="4f2cf-105">Paket aplikasi Microsoft 365 untuk bisnis dan Microsoft 365 aplikasi untuk bisnis Premium tidak menyertakan aplikasi Microsoft 365 untuk perusahaan.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="4f2cf-106">Anda perlu mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="4f2cf-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="4f2cf-107">Jika Anda ingin menginstal aplikasi Microsoft 365 untuk perusahaan di RDS dari Pusat admin Microsoft 365, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="4f2cf-108">Anda juga bisa mengunduh dan menjalankan [asisten dukungan dan pemulihan Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal aplikasi Microsoft 365 untuk perusahaan dalam mode aktivasi komputer bersama.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="4f2cf-109">Lihat langganan Microsoft 365 apa yang Anda miliki.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="4f2cf-110">Pelajari caranya</span><span class="sxs-lookup"><span data-stu-id="4f2cf-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="4f2cf-111">Jika perlu, alihkan ke langganan Microsoft 365 yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="4f2cf-112">Pelajari caranya</span><span class="sxs-lookup"><span data-stu-id="4f2cf-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="4f2cf-113">Jika Office telah terinstal di server RDS menggunakan langganan Microsoft 365 lainnya, Hapus instalasinya.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="4f2cf-114">Misalnya, dengan masuk ke panel kontrol \> hapus instalan program.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="4f2cf-115">Hapus instalan menggunakan [asisten dukungan dan pemulihan Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda mengalami masalah.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="4f2cf-116">Di server RDS, masuk ke Pusat admin Microsoft 365 dengan akun administrator Anda dan [instal aplikasi Microsoft 365 untuk perusahaan](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="4f2cf-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="4f2cf-117">Setelah Office terinstal, ***jangan buka atau masuk*** ke aplikasi Office apa pun.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="4f2cf-118">Di server RDS, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="4f2cf-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="4f2cf-119">Klik kanan tombol Windows di sudut kiri bawah layar Anda, lalu pilih Jalankan.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="4f2cf-120">Dalam kotak buka, ketikkan **regedit**, lalu pilih OK.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="4f2cf-121">Pilih Ya ketika diminta untuk memperbolehkan editor registri untuk membuat perubahan pada perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="4f2cf-122">Dalam editor registri, tambahkan nilai string **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="4f2cf-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="4f2cf-123">Di server RDS, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa aktivasi komputer bersama diaktifkan untuk aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="4f2cf-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="4f2cf-124">Untuk detail selengkapnya tentang prasyarat, instruksi penyetelan dan panduan tentang instalasi yang dikustomisasi dengan menggunakan alat penyebaran Office, silakan lihat [menyebarkan aplikasi Microsoft 365 untuk perusahaan dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="4f2cf-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="4f2cf-125">Untuk memperbaiki kesalahan terkait aktivasi komputer bersama, silakan lihat [memecahkan masalah dengan aktivasi komputer bersama untuk aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="4f2cf-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  