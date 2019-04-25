---
title: Menginstal office pada Server Terminal - tanpa izin
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410125"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8bac5-102">Menginstal Office pada Terminal Server</span><span class="sxs-lookup"><span data-stu-id="8bac5-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8bac5-103">Untuk menggunakan kantor 365 ProPlus pada Windows Server menggunakan Remote Desktop Services (RDS), sebelumnya bernama Layanan Terminal:</span><span class="sxs-lookup"><span data-stu-id="8bac5-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8bac5-104">Anda harus memiliki rencana Office 365 yang mencakup kantor 365 ProPlus, seperti kantor 365 Enterprise E3 atau Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="8bac5-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8bac5-105">Office 365 bisnis dan kantor 365 bisnis Premium rencana tidak termasuk kantor 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="8bac5-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="8bac5-106">Anda perlu untuk mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8bac5-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="8bac5-107">Jika Anda ingin menginstal Office 365 ProPlus pada RDS dari portal Office 365, \*\* *yang menggunakan pengaturan default instalasi* \*\*, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="8bac5-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="8bac5-108">Periksa apa rencana Office 365 yang Anda miliki.</span><span class="sxs-lookup"><span data-stu-id="8bac5-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="8bac5-109">Pelajari bagaimana</span><span class="sxs-lookup"><span data-stu-id="8bac5-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. <span data-ttu-id="8bac5-110">Jika perlu, beralih ke Office 365 berbeda berencana.</span><span class="sxs-lookup"><span data-stu-id="8bac5-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="8bac5-111">Pelajari bagaimana</span><span class="sxs-lookup"><span data-stu-id="8bac5-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. <span data-ttu-id="8bac5-112">Jika kantor sudah diinstal pada server RDS menggunakan rencana Office 365 lain, uninstall.</span><span class="sxs-lookup"><span data-stu-id="8bac5-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="8bac5-113">Sebagai contoh, dengan pergi ke Control Panel \> Uninstall sebuah program.</span><span class="sxs-lookup"><span data-stu-id="8bac5-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8bac5-114">Uninstall menggunakan [Microsoft Support dan asisten pemulihan](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda menjalankan ke masalah.</span><span class="sxs-lookup"><span data-stu-id="8bac5-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="8bac5-115">Di RDS server, masuk ke portal 365 kantor dengan administrator account dan [menginstal Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="8bac5-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="8bac5-116">Setelah kantor diinstal, \*\* *tidak membuka atau masuk* \*\* untuk aplikasi kantor.</span><span class="sxs-lookup"><span data-stu-id="8bac5-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="8bac5-117">Di RDS server, mengaktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="8bac5-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="8bac5-118">Klik kanan tombol Windows di sudut kiri bawah layar Anda, lalu pilih Jalankan.</span><span class="sxs-lookup"><span data-stu-id="8bac5-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8bac5-119">Di kotak buka, ketikkan **regedit**, dan kemudian pilih OK.</span><span class="sxs-lookup"><span data-stu-id="8bac5-119">In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="8bac5-120">Pilih Ya saat diminta agar Registry Editor untuk membuat perubahan ke perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="8bac5-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="8bac5-121">Di Penyunting registri, menambahkan nilai string dari **SharedComputerLicensing** dengan suasana 1 di bawah HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="8bac5-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="8bac5-122">Di RDS server, \*\* *masuk sebagai pengguna akhir* \*\* dan [memverifikasi bahwa komputer bersama aktivasi diaktifkan untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="8bac5-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="8bac5-123">Untuk detail lebih lanjut tentang prasyarat, setup instruksi dan panduan instalasi yang disesuaikan dengan menggunakan alat penyebaran kantor, silakan lihat [Menyebarkan kantor 365 ProPlus dengan menggunakan Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="8bac5-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="8bac5-124">Untuk memperbaiki kesalahan yang berhubungan dengan komputer bersama aktivasi, lihat [mengatasi masalah masalah dengan komputer bersama aktivasi untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8bac5-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

