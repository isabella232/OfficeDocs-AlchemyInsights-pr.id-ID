---
title: Memperbaiki aplikasi Microsoft 365 Maaf, kami mengalami pesan masalah server sementara
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582706"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="de9c1-102">Memperbaiki aplikasi Microsoft 365 "Maaf, kami mengalami masalah server sementara" pesan</span><span class="sxs-lookup"><span data-stu-id="de9c1-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="de9c1-103">Jika Anda menerima pesan ini, cobalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="de9c1-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="de9c1-104">Periksa firewall, perangkat lunak antivirus, dan pengaturan proxy untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="de9c1-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="de9c1-105">Lihat [rentang URL dan alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="de9c1-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="de9c1-106">Pergi ke **mulai**  >  **menjalankan**, dan kemudian ketik **Services. MSC**.</span><span class="sxs-lookup"><span data-stu-id="de9c1-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="de9c1-107">Pastikan bahwa layanan berikut ini berjalan:</span><span class="sxs-lookup"><span data-stu-id="de9c1-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="de9c1-108">Jaringan tersambung perangkat Auto-setup</span><span class="sxs-lookup"><span data-stu-id="de9c1-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="de9c1-109">Layanan daftar jaringan</span><span class="sxs-lookup"><span data-stu-id="de9c1-109">Network List Service</span></span>
    - <span data-ttu-id="de9c1-110">Kesadaran lokasi jaringan</span><span class="sxs-lookup"><span data-stu-id="de9c1-110">Network Location Awareness</span></span>
    - <span data-ttu-id="de9c1-111">Log peristiwa Windows</span><span class="sxs-lookup"><span data-stu-id="de9c1-111">Windows Event Log</span></span>

<span data-ttu-id="de9c1-112">Jika salah satu layanan ini tidak berjalan, cobalah untuk memulainya.</span><span class="sxs-lookup"><span data-stu-id="de9c1-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="de9c1-113">Jika Anda memiliki masalah memulai layanan, jalankan perintah berikut ini dengan membuka prompt perintah dengan izin yang ditinggikan:</span><span class="sxs-lookup"><span data-stu-id="de9c1-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="de9c1-114">**SFC/SCANNOW**</span><span class="sxs-lookup"><span data-stu-id="de9c1-114">**sfc /scannow**</span></span>

<span data-ttu-id="de9c1-115">Setelah perintah ini selesai, mulai ulang komputer.</span><span class="sxs-lookup"><span data-stu-id="de9c1-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="de9c1-116">Untuk informasi terperinci, lihat ["Maaf, kami tidak dapat tersambung ke akun Anda. Silakan coba lagi nanti "galat saat Anda mengaktifkan](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="de9c1-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>