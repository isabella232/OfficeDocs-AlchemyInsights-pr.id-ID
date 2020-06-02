---
title: Menginstal Office di terminal server-tidak berlisensi
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508631"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="5d469-102">Menginstal Office di terminal server</span><span class="sxs-lookup"><span data-stu-id="5d469-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="5d469-103">Untuk menyebarkan Microsoft 365 aplikasi untuk perusahaan di Windows Server menggunakan layanan desktop jarak jauh (RDS), sebelumnya bernama Layanan Terminal:</span><span class="sxs-lookup"><span data-stu-id="5d469-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="5d469-104">Anda harus memiliki langganan Microsoft 365 yang mencakup Microsoft 365 aplikasi untuk perusahaan, seperti Office 365 Enterprise E3 atau Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="5d469-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="5d469-105">Microsoft 365 aplikasi untuk bisnis dan Microsoft 365 aplikasi untuk bisnis Premium rencana tidak termasuk Microsoft 365 aplikasi untuk perusahaan.</span><span class="sxs-lookup"><span data-stu-id="5d469-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="5d469-106">Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="5d469-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="5d469-107">Jika Anda ingin menginstal Microsoft 365 aplikasi untuk perusahaan di RDS dari Microsoft 365 Admin Center, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini.</span><span class="sxs-lookup"><span data-stu-id="5d469-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="5d469-108">Anda juga dapat mengunduh dan menjalankan [dukungan Microsoft dan asisten pemulihan](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal Microsoft 365 aplikasi untuk perusahaan dalam mode aktivasi komputer bersama.</span><span class="sxs-lookup"><span data-stu-id="5d469-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="5d469-109">Periksa apa langganan Microsoft 365 yang Anda miliki.</span><span class="sxs-lookup"><span data-stu-id="5d469-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="5d469-110">Pelajari caranya</span><span class="sxs-lookup"><span data-stu-id="5d469-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="5d469-111">Jika perlu, beralih ke langganan Microsoft 365 yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="5d469-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="5d469-112">Pelajari caranya</span><span class="sxs-lookup"><span data-stu-id="5d469-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="5d469-113">Jika Office sudah diinstal di RDS server menggunakan langganan Microsoft 365 lainnya, uninstall.</span><span class="sxs-lookup"><span data-stu-id="5d469-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="5d469-114">Sebagai contoh, dengan pergi ke Control Panel \> Uninstall program.</span><span class="sxs-lookup"><span data-stu-id="5d469-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="5d469-115">Membongkar menggunakan [dukungan Microsoft dan pemulihan asisten](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda menjalankan ke masalah.</span><span class="sxs-lookup"><span data-stu-id="5d469-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="5d469-116">Di RDS server, masuk ke Pusat admin Microsoft 365 dengan akun administrator dan [menginstal microsoft 365 aplikasi untuk perusahaan](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="5d469-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="5d469-117">Setelah Office diinstal, ***jangan membuka atau masuk*** ke aplikasi Office apa pun.</span><span class="sxs-lookup"><span data-stu-id="5d469-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="5d469-118">Di RDS server, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="5d469-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="5d469-119">Klik kanan tombol Windows di sudut kiri bawah layar dan pilih Jalankan.</span><span class="sxs-lookup"><span data-stu-id="5d469-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="5d469-120">Di kotak buka, ketik **regedit**, dan kemudian pilih OK.</span><span class="sxs-lookup"><span data-stu-id="5d469-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="5d469-121">Pilih Ya saat diminta untuk mengizinkan Penyunting registri untuk membuat perubahan pada perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="5d469-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="5d469-122">Di Penyunting registri, tambahkan nilai untai **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="5d469-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="5d469-123">Di RDS server, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa komputer bersama aktivasi diaktifkan untuk Microsoft 365 aplikasi untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="5d469-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="5d469-124">Untuk rincian lebih lanjut tentang prasyarat, petunjuk penataan dan Panduan pada instalasi disesuaikan dengan menggunakan alat penyebaran Office, silakan lihat [menyebarkan Microsoft 365 aplikasi untuk perusahaan dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="5d469-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="5d469-125">Untuk memperbaiki kesalahan yang terkait dengan aktivasi komputer bersama, silakan lihat [memecahkan masalah dengan aktivasi komputer bersama untuk Microsoft 365 aplikasi untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="5d469-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  