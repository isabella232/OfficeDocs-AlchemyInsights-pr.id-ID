---
title: Memperbaiki aplikasi Microsoft 365 Maaf, kami mengalami pesan masalah server sementara
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835274"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="11a94-102">Memperbaiki pesan "Maaf, kami mengalami masalah server sementara" aplikasi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="11a94-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="11a94-103">Jika Anda menerima pesan ini, cobalah hal berikut:</span><span class="sxs-lookup"><span data-stu-id="11a94-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="11a94-104">Periksa pengaturan firewall, perangkat lunak antivirus, dan proksi untuk mengonfirmasi bahwa firewall dan proksi tidak memblokir akses Internet ke aplikasi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="11a94-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="11a94-105">Lihat [URL dan rentang alamat IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="11a94-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="11a94-106">Buka **Mulai**  >  **Jalankan**, lalu ketik **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="11a94-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="11a94-107">Pastikan semua layanan berikut ini berjalan:</span><span class="sxs-lookup"><span data-stu-id="11a94-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="11a94-108">Penyetelan Otomatis Perangkat Tersambung Jaringan</span><span class="sxs-lookup"><span data-stu-id="11a94-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="11a94-109">Layanan Daftar Jaringan</span><span class="sxs-lookup"><span data-stu-id="11a94-109">Network List Service</span></span>
    - <span data-ttu-id="11a94-110">Kesadaran Lokasi Jaringan</span><span class="sxs-lookup"><span data-stu-id="11a94-110">Network Location Awareness</span></span>
    - <span data-ttu-id="11a94-111">Log Kejadian Windows</span><span class="sxs-lookup"><span data-stu-id="11a94-111">Windows Event Log</span></span>

<span data-ttu-id="11a94-112">Jika salah satu layanan ini tidak berjalan, cobalah memulainya.</span><span class="sxs-lookup"><span data-stu-id="11a94-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="11a94-113">Jika mengalami masalah saat memulai layanan, jalankan perintah berikut dengan membuka prompt perintah dengan izin yang ditingkatkan:</span><span class="sxs-lookup"><span data-stu-id="11a94-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="11a94-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="11a94-114">**sfc /scannow**</span></span>

<span data-ttu-id="11a94-115">Setelah perintah ini selesai, mulai ulang komputer.</span><span class="sxs-lookup"><span data-stu-id="11a94-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="11a94-116">Untuk informasi selengkapnya, lihat ["Maaf, kami tidak bisa tersambung ke akun Anda. Coba lagi nanti" saat Anda mengaktifkan](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="11a94-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>