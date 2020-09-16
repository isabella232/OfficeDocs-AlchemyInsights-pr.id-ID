---
title: Masalah aktivasi-kami tidak dapat menyambungkan sekarang
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725986"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="bd754-102">Memperbaiki aplikasi Microsoft 365 "kami tidak dapat menyambungkan sekarang" pesan</span><span class="sxs-lookup"><span data-stu-id="bd754-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="bd754-103">Jika Anda menerima pesan ini, cobalah hal berikut:</span><span class="sxs-lookup"><span data-stu-id="bd754-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bd754-104">Periksa firewall, perangkat lunak antivirus, dan pengaturan proksi Anda untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bd754-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="bd754-105">Lihat [Microsoft URL dan rentang alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="bd754-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="bd754-106">Masuk ke **mulai**  >  **Jalankan**, lalu ketikkan **Services. MSC**.</span><span class="sxs-lookup"><span data-stu-id="bd754-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="bd754-107">Pastikan bahwa layanan berikut ini berjalan:</span><span class="sxs-lookup"><span data-stu-id="bd754-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="bd754-108">Penyetelan otomatis perangkat yang tersambung ke jaringan</span><span class="sxs-lookup"><span data-stu-id="bd754-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="bd754-109">Layanan daftar jaringan</span><span class="sxs-lookup"><span data-stu-id="bd754-109">Network List Service</span></span>
    - <span data-ttu-id="bd754-110">Kesadaran lokasi jaringan</span><span class="sxs-lookup"><span data-stu-id="bd754-110">Network Location Awareness</span></span>
    - <span data-ttu-id="bd754-111">Log kejadian Windows</span><span class="sxs-lookup"><span data-stu-id="bd754-111">Windows Event Log</span></span>

<span data-ttu-id="bd754-112">Jika salah satu layanan ini tidak berjalan, cobalah untuk memulainya.</span><span class="sxs-lookup"><span data-stu-id="bd754-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="bd754-113">Jika Anda mengalami masalah memulai layanan, jalankan perintah berikut ini dengan membuka perintah dengan izin yang ditinggikan:</span><span class="sxs-lookup"><span data-stu-id="bd754-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="bd754-114">**SFC/SCANNOW**</span><span class="sxs-lookup"><span data-stu-id="bd754-114">**sfc /scannow**</span></span>

<span data-ttu-id="bd754-115">Setelah perintah ini selesai, mulai ulang komputer.</span><span class="sxs-lookup"><span data-stu-id="bd754-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="bd754-116">Untuk informasi mendetail, lihat ["Maaf, kami tidak dapat tersambung ke akun Anda. Kesalahan coba lagi nanti "saat Anda mengaktifkan Office dari Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="bd754-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>