---
title: Menyebarkan aplikasi Microsoft 365 untuk perusahaan untuk penggunaan bersama di RDS, terminal server, atau VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200676"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="e787c-102">Menyebarkan aplikasi Microsoft 365 untuk perusahaan untuk penggunaan bersama di RDS, terminal server, atau VDI</span><span class="sxs-lookup"><span data-stu-id="e787c-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="e787c-103">Untuk menggunakan aplikasi Microsoft 365 untuk perusahaan dengan Remote Desktop Services (RDS), sebelumnya bernama Services terminal:</span><span class="sxs-lookup"><span data-stu-id="e787c-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="e787c-104">Anda harus memiliki paket Microsoft 365 for Business atau paket Office 365 yang menyertakan aplikasi Microsoft 365 untuk perusahaan, seperti Office 365 Enterprise E3 atau Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="e787c-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="e787c-105">Aplikasi Microsoft 365 untuk bisnis dan Microsoft 365 paket standar bisnis tidak menyertakan aplikasi Microsoft 365 untuk perusahaan.</span><span class="sxs-lookup"><span data-stu-id="e787c-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="e787c-106">Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="e787c-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="e787c-107">Anda juga bisa mengunduh dan menjalankan [asisten dukungan dan pemulihan Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal aplikasi Microsoft 365 untuk perusahaan dalam mode aktivasi komputer bersama.</span><span class="sxs-lookup"><span data-stu-id="e787c-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="e787c-108">Untuk informasi selengkapnya tentang prasyarat, instruksi penyetelan, dan panduan tentang instalasi yang dikustomisasi dengan menggunakan alat penyebaran Office, lihat [menyebarkan aplikasi Microsoft 365 untuk perusahaan dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="e787c-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="e787c-109">Untuk memperbaiki kesalahan terkait aktivasi komputer bersama:</span><span class="sxs-lookup"><span data-stu-id="e787c-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="e787c-110">Lihat [memecahkan masalah dengan aktivasi komputer bersama untuk aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="e787c-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="e787c-111">Lihat [Mengatur ulang status aktivasi Aplikasi Microsoft 365 untuk perusahaan](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="e787c-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="e787c-112">Jika Anda ingin menginstal aplikasi Microsoft 365 untuk perusahaan di RDS dari Pusat admin Microsoft 365, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="e787c-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="e787c-113">Periksa langganan yang Anda miliki.</span><span class="sxs-lookup"><span data-stu-id="e787c-113">Check what subscription you have.</span></span> <span data-ttu-id="e787c-114">[Pelajari caranya](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="e787c-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="e787c-115">Jika perlu, alihkan ke langganan lain.</span><span class="sxs-lookup"><span data-stu-id="e787c-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="e787c-116">[Pelajari caranya](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="e787c-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="e787c-117">Jika Office telah terinstal di server RDS menggunakan langganan Microsoft lainnya, hapus instalan.</span><span class="sxs-lookup"><span data-stu-id="e787c-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="e787c-118">Misalnya, dengan masuk ke **panel kontrol**  >  **hapus instalan program**.</span><span class="sxs-lookup"><span data-stu-id="e787c-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="e787c-119">Hapus instalan menggunakan [asisten dukungan dan pemulihan Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda mengalami masalah.</span><span class="sxs-lookup"><span data-stu-id="e787c-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="e787c-120">Di server RDS, masuk ke Pusat admin Microsoft 365 dengan akun administrator Anda dan [instal aplikasi Microsoft 365 untuk perusahaan](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="e787c-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="e787c-121">Setelah Office terinstal, ***jangan buka atau masuk*** ke aplikasi Office apa pun.</span><span class="sxs-lookup"><span data-stu-id="e787c-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="e787c-122">Di server RDS, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="e787c-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="e787c-123">Klik kanan tombol Windows di sudut kiri bawah layar Anda, lalu pilih **Jalankan**.</span><span class="sxs-lookup"><span data-stu-id="e787c-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="e787c-124">Dalam kotak buka, ketikkan **regedit**, lalu pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="e787c-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="e787c-125">Pilih **ya** ketika diminta untuk memperbolehkan editor registri untuk membuat perubahan pada perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="e787c-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="e787c-126">Dalam editor registri, tambahkan nilai string **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="e787c-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="e787c-127">Di server RDS, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa aktivasi komputer bersama diaktifkan untuk aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="e787c-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
