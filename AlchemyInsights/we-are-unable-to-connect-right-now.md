---
title: Masalah aktivasi-kami tidak dapat terhubung saat ini
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628245"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="51d11-102">Memperbaiki aplikasi Office "kami tidak dapat terhubung sekarang" pesan</span><span class="sxs-lookup"><span data-stu-id="51d11-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="51d11-103">Jika Anda menerima pesan ini, cobalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="51d11-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="51d11-104">Periksa firewall, perangkat lunak antivirus, dan pengaturan proxy untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Office.</span><span class="sxs-lookup"><span data-stu-id="51d11-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="51d11-105">Lihat [Office 365 URL dan kisaran alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="51d11-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="51d11-106">Pergi ke **mulai** > **menjalankan**, dan kemudian ketik **Services. MSC**.</span><span class="sxs-lookup"><span data-stu-id="51d11-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="51d11-107">Pastikan bahwa layanan berikut ini berjalan:</span><span class="sxs-lookup"><span data-stu-id="51d11-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="51d11-108">Jaringan tersambung perangkat Auto-setup</span><span class="sxs-lookup"><span data-stu-id="51d11-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="51d11-109">Layanan daftar jaringan</span><span class="sxs-lookup"><span data-stu-id="51d11-109">Network List Service</span></span>
    - <span data-ttu-id="51d11-110">Kesadaran lokasi jaringan</span><span class="sxs-lookup"><span data-stu-id="51d11-110">Network Location Awareness</span></span>
    - <span data-ttu-id="51d11-111">Log peristiwa Windows</span><span class="sxs-lookup"><span data-stu-id="51d11-111">Windows Event Log</span></span>

<span data-ttu-id="51d11-112">Jika salah satu layanan ini tidak berjalan, cobalah untuk memulainya.</span><span class="sxs-lookup"><span data-stu-id="51d11-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="51d11-113">Jika Anda memiliki masalah memulai layanan, jalankan perintah berikut ini dengan membuka prompt perintah dengan izin yang ditinggikan:</span><span class="sxs-lookup"><span data-stu-id="51d11-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="51d11-114">**SFC/SCANNOW**</span><span class="sxs-lookup"><span data-stu-id="51d11-114">**sfc /scannow**</span></span>

<span data-ttu-id="51d11-115">Setelah perintah ini selesai, mulai ulang komputer.</span><span class="sxs-lookup"><span data-stu-id="51d11-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="51d11-116">Untuk informasi terperinci, lihat ["Maaf, kami tidak dapat tersambung ke akun Anda. Silakan coba lagi nanti "galat saat Anda mengaktifkan Office dari Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="51d11-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>