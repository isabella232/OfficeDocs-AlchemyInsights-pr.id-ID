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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581878"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="0e1f0-102">Memperbaiki aplikasi Microsoft 365 "kami tidak dapat terhubung sekarang" pesan</span><span class="sxs-lookup"><span data-stu-id="0e1f0-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="0e1f0-103">Jika Anda menerima pesan ini, cobalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="0e1f0-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="0e1f0-104">Periksa firewall, perangkat lunak antivirus, dan pengaturan proxy untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0e1f0-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="0e1f0-105">Lihat [Microsoft URL dan kisaran alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="0e1f0-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="0e1f0-106">Pergi ke **mulai**  >  **menjalankan**, dan kemudian ketik **Services. MSC**.</span><span class="sxs-lookup"><span data-stu-id="0e1f0-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="0e1f0-107">Pastikan bahwa layanan berikut ini berjalan:</span><span class="sxs-lookup"><span data-stu-id="0e1f0-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="0e1f0-108">Jaringan tersambung perangkat Auto-setup</span><span class="sxs-lookup"><span data-stu-id="0e1f0-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="0e1f0-109">Layanan daftar jaringan</span><span class="sxs-lookup"><span data-stu-id="0e1f0-109">Network List Service</span></span>
    - <span data-ttu-id="0e1f0-110">Kesadaran lokasi jaringan</span><span class="sxs-lookup"><span data-stu-id="0e1f0-110">Network Location Awareness</span></span>
    - <span data-ttu-id="0e1f0-111">Log peristiwa Windows</span><span class="sxs-lookup"><span data-stu-id="0e1f0-111">Windows Event Log</span></span>

<span data-ttu-id="0e1f0-112">Jika salah satu layanan ini tidak berjalan, cobalah untuk memulainya.</span><span class="sxs-lookup"><span data-stu-id="0e1f0-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="0e1f0-113">Jika Anda memiliki masalah memulai layanan, jalankan perintah berikut ini dengan membuka prompt perintah dengan izin yang ditinggikan:</span><span class="sxs-lookup"><span data-stu-id="0e1f0-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="0e1f0-114">**SFC/SCANNOW**</span><span class="sxs-lookup"><span data-stu-id="0e1f0-114">**sfc /scannow**</span></span>

<span data-ttu-id="0e1f0-115">Setelah perintah ini selesai, mulai ulang komputer.</span><span class="sxs-lookup"><span data-stu-id="0e1f0-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="0e1f0-116">Untuk informasi terperinci, lihat ["Maaf, kami tidak dapat tersambung ke akun Anda. Silakan coba lagi nanti "galat saat Anda mengaktifkan Office dari Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="0e1f0-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>