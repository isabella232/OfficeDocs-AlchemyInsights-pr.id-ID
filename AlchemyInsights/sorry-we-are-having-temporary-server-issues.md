---
title: Memperbaiki aplikasi Office Maaf, kami mengalami pesan masalah server sementara
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627993"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="904e5-102">Memperbaiki aplikasi Office "Maaf, kami mengalami masalah server sementara" pesan</span><span class="sxs-lookup"><span data-stu-id="904e5-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="904e5-103">Jika Anda menerima pesan ini, cobalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="904e5-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="904e5-104">Periksa firewall, perangkat lunak antivirus, dan pengaturan proxy untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Office.</span><span class="sxs-lookup"><span data-stu-id="904e5-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="904e5-105">Lihat [Office 365 URL dan kisaran alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="904e5-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="904e5-106">Pergi ke **mulai** > **menjalankan**, dan kemudian ketik **Services. MSC**.</span><span class="sxs-lookup"><span data-stu-id="904e5-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="904e5-107">Pastikan bahwa layanan berikut ini berjalan:</span><span class="sxs-lookup"><span data-stu-id="904e5-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="904e5-108">Jaringan tersambung perangkat Auto-setup</span><span class="sxs-lookup"><span data-stu-id="904e5-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="904e5-109">Layanan daftar jaringan</span><span class="sxs-lookup"><span data-stu-id="904e5-109">Network List Service</span></span>
    - <span data-ttu-id="904e5-110">Kesadaran lokasi jaringan</span><span class="sxs-lookup"><span data-stu-id="904e5-110">Network Location Awareness</span></span>
    - <span data-ttu-id="904e5-111">Log peristiwa Windows</span><span class="sxs-lookup"><span data-stu-id="904e5-111">Windows Event Log</span></span>

<span data-ttu-id="904e5-112">Jika salah satu layanan ini tidak berjalan, cobalah untuk memulainya.</span><span class="sxs-lookup"><span data-stu-id="904e5-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="904e5-113">Jika Anda memiliki masalah memulai layanan, jalankan perintah berikut ini dengan membuka prompt perintah dengan izin yang ditinggikan:</span><span class="sxs-lookup"><span data-stu-id="904e5-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="904e5-114">**SFC/SCANNOW**</span><span class="sxs-lookup"><span data-stu-id="904e5-114">**sfc /scannow**</span></span>

<span data-ttu-id="904e5-115">Setelah perintah ini selesai, mulai ulang komputer.</span><span class="sxs-lookup"><span data-stu-id="904e5-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="904e5-116">Untuk informasi terperinci, lihat ["Maaf, kami tidak dapat tersambung ke akun Anda. Silakan coba lagi nanti "galat saat Anda mengaktifkan Office dari Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="904e5-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>