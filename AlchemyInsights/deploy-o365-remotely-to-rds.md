---
title: Menyebarkan Office 365 ProPlus untuk digunakan bersama di RDS, terminal server, atau VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959463"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="95db7-102">Menyebarkan Office 365 ProPlus untuk digunakan bersama di RDS, terminal server, atau VDI</span><span class="sxs-lookup"><span data-stu-id="95db7-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="95db7-103">Untuk menyebarkan Office 365 ProPlus menggunakan layanan desktop jarak jauh (RDS), sebelumnya bernama Layanan Terminal:</span><span class="sxs-lookup"><span data-stu-id="95db7-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="95db7-104">Anda harus memiliki Microsoft 365 untuk rencana bisnis atau Office 365 rencana yang mencakup Office 365 ProPlus, seperti Office 365 Enterprise E3 atau Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="95db7-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="95db7-105">Office 365 bisnis dan Office 365 rencana bisnis Premium tidak termasuk Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="95db7-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="95db7-106">Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="95db7-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="95db7-107">Anda juga dapat mengunduh dan menjalankan [dukungan Microsoft dan asisten pemulihan](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal Office 365 ProPlus dalam mode aktivasi komputer bersama.</span><span class="sxs-lookup"><span data-stu-id="95db7-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="95db7-108">Untuk informasi lebih lanjut tentang prasyarat, petunjuk penataan, dan Panduan pada instalasi disesuaikan dengan menggunakan alat penyebaran Office, lihat [menyebarkan office 365 ProPlus dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="95db7-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="95db7-109">Untuk memperbaiki kesalahan yang terkait dengan aktivasi komputer bersama:</span><span class="sxs-lookup"><span data-stu-id="95db7-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="95db7-110">Lihat [memecahkan masalah dengan aktivasi komputer bersama untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="95db7-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="95db7-111">Lihat [reset Office 365 ProPlus aktivasi negara](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="95db7-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="95db7-112">Jika Anda ingin menginstal Office 365 ProPlus di RDS dari Microsoft 365 Admin Center, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="95db7-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="95db7-113">Periksa apa Office 365 rencana yang Anda miliki.</span><span class="sxs-lookup"><span data-stu-id="95db7-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="95db7-114">[Pelajari caranya](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="95db7-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="95db7-115">Jika perlu, beralih ke rencana Office 365 yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="95db7-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="95db7-116">[Pelajari caranya](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="95db7-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="95db7-117">Jika Office sudah diinstal di RDS server menggunakan rencana Office 365 lainnya, bongkar.</span><span class="sxs-lookup"><span data-stu-id="95db7-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="95db7-118">Misalnya, dengan pergi ke **Control Panel** > **Uninstall program**.</span><span class="sxs-lookup"><span data-stu-id="95db7-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="95db7-119">Membongkar menggunakan [dukungan Microsoft dan pemulihan asisten](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda menjalankan ke masalah.</span><span class="sxs-lookup"><span data-stu-id="95db7-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="95db7-120">Di RDS server, masuk ke Microsoft 365 Admin Center dengan akun administrator dan [menginstal Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="95db7-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="95db7-121">Setelah Office diinstal, ***jangan membuka atau masuk*** ke aplikasi Office apa pun.</span><span class="sxs-lookup"><span data-stu-id="95db7-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="95db7-122">Di RDS server, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="95db7-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="95db7-123">Klik kanan tombol Windows di sudut kiri bawah layar Anda dan pilih **Jalankan**.</span><span class="sxs-lookup"><span data-stu-id="95db7-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="95db7-124">Di kotak buka, ketik **regedit**, dan kemudian pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="95db7-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="95db7-125">Pilih **ya** saat diminta untuk mengizinkan Penyunting registri untuk membuat perubahan pada perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="95db7-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="95db7-126">Di Penyunting registri, tambahkan nilai untai **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="95db7-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="95db7-127">Di RDS server, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa komputer bersama aktivasi diaktifkan untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="95db7-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

