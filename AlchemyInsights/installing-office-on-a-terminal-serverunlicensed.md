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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/25/2019
ms.locfileid: "37205412"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8d0f7-102">Menginstal Office di terminal server</span><span class="sxs-lookup"><span data-stu-id="8d0f7-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8d0f7-103">Untuk menyebarkan Office 365 ProPlus di Windows Server menggunakan layanan desktop jarak jauh (RDS), sebelumnya bernama Layanan Terminal:</span><span class="sxs-lookup"><span data-stu-id="8d0f7-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8d0f7-104">Anda harus memiliki rencana Office 365 yang mencakup Office 365 ProPlus, seperti Office 365 Enterprise E3 atau Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8d0f7-105">Office 365 bisnis dan Office 365 rencana bisnis Premium tidak termasuk Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="8d0f7-106">Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8d0f7-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="8d0f7-107">Jika Anda ingin menginstal Office 365 ProPlus di RDS dari Microsoft 365 Admin Center, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="8d0f7-108">Anda juga dapat mengunduh dan menjalankan [dukungan Microsoft dan asisten pemulihan](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal Office 365 ProPlus dalam mode aktivasi komputer bersama.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="8d0f7-109">Periksa apa Office 365 rencana yang Anda miliki.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="8d0f7-110">Pelajari caranya</span><span class="sxs-lookup"><span data-stu-id="8d0f7-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="8d0f7-111">Jika perlu, beralih ke rencana Office 365 yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="8d0f7-112">Pelajari caranya</span><span class="sxs-lookup"><span data-stu-id="8d0f7-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="8d0f7-113">Jika Office sudah diinstal di RDS server menggunakan rencana Office 365 lainnya, bongkar.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="8d0f7-114">Sebagai contoh, dengan pergi ke Control Panel \> Uninstall program.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8d0f7-115">Membongkar menggunakan [dukungan Microsoft dan pemulihan asisten](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda menjalankan ke masalah.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="8d0f7-116">Di RDS server, masuk ke Microsoft 365 Admin Center dengan akun administrator dan [menginstal Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="8d0f7-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="8d0f7-117">Setelah Office diinstal, ***jangan membuka atau masuk*** ke aplikasi Office apa pun.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="8d0f7-118">Di RDS server, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="8d0f7-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="8d0f7-119">Klik kanan tombol Windows di sudut kiri bawah layar dan pilih Jalankan.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8d0f7-120">Di kotak buka, ketik **regedit**, dan kemudian pilih OK.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="8d0f7-121">Pilih Ya saat diminta untuk mengizinkan Penyunting registri untuk membuat perubahan pada perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="8d0f7-122">Di Penyunting registri, tambahkan nilai untai **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="8d0f7-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="8d0f7-123">Di RDS server, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa komputer bersama aktivasi diaktifkan untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="8d0f7-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="8d0f7-124">Untuk rincian lebih lanjut tentang prasyarat, petunjuk penataan dan Panduan pada instalasi disesuaikan dengan menggunakan alat penyebaran Office, silakan lihat [menyebarkan office 365 ProPlus dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="8d0f7-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="8d0f7-125">Untuk memperbaiki kesalahan yang terkait dengan aktivasi komputer bersama, silakan lihat [memecahkan masalah dengan aktivasi komputer bersama untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8d0f7-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  