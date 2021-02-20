---
title: Apakah pengguna Anda menerima email berbahaya
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291795"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="dede4-102">Apakah pengguna Anda menerima email berbahaya?</span><span class="sxs-lookup"><span data-stu-id="dede4-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="dede4-103">Sekarang Anda dapat melaporkan email berbahaya tersebut ke Microsoft menggunakan [Pengumpulan Admin di Pusat Keamanan & Kepatuhan](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="dede4-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="dede4-104">Pesan yang dikirimkan di [pengumpulan admin](https://sip.protection.office.com/reportsubmission) dipindai, dan hasilnya akan ditampilkan di flyout **detail**:</span><span class="sxs-lookup"><span data-stu-id="dede4-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="dede4-105">Jika terjadi kegagalan dalam autentikasi email pengirim pada saat pengiriman.</span><span class="sxs-lookup"><span data-stu-id="dede4-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="dede4-106">Informasi tentang kebijakan terkait yang mungkin terpengaruh atau tertimpa putusan pesan.</span><span class="sxs-lookup"><span data-stu-id="dede4-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="dede4-107">Hasil detonasi saat ini untuk melihat apakah URL atau file yang ada dalam pesan berbahaya atau tidak.</span><span class="sxs-lookup"><span data-stu-id="dede4-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="dede4-108">Umpan balik dari pemberi nilai</span><span class="sxs-lookup"><span data-stu-id="dede4-108">Feedback from graders</span></span>

<span data-ttu-id="dede4-109">Jika ditemukan timpaan, proses pemindaian ulang akan selesai dalam beberapa menit.</span><span class="sxs-lookup"><span data-stu-id="dede4-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="dede4-110">Jika tidak ada masalah dalam autentikasi email atau jika pengiriman tidak terpengaruh oleh timpaan, umpan balik dari pemberi nilai dapat memakan waktu hingga satu hari.</span><span class="sxs-lookup"><span data-stu-id="dede4-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="dede4-111">Jika Anda tidak setuju dengan keputusan akhir pada pesan, URL atau file (diblokir vs. tidak diblokir), kirimkan pesan lagi setelah satu hari untuk pemindaian ulang.</span><span class="sxs-lookup"><span data-stu-id="dede4-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="dede4-112">Kemungkinan besar, keputusan akan berubah setelah mengirimkan pesan kembali.</span><span class="sxs-lookup"><span data-stu-id="dede4-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="dede4-113">Sementara itu, Anda dapat menghapus email berbahaya dari kotak masuk pengguna dengan mengikuti petunjuk dalam [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="dede4-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="dede4-114">Pelanggan dengan Pertahanan Microsoft untuk Office 365 dapat:</span><span class="sxs-lookup"><span data-stu-id="dede4-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="dede4-115">gunakan [Penjelajah Ancaman untuk Menemukan dan Menghapus email Berbahaya](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="dede4-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="dede4-116">[menggunakan Link Aman untuk memblokir akses ](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) ke URL berbahaya</span><span class="sxs-lookup"><span data-stu-id="dede4-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="dede4-117">melacak pengguna yang mengklik dan mengakses URL berbahaya: [Menampilkan URL pengelabuan dan mengklik data keputusan](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="dede4-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="dede4-118">secara manual [mulai Penyelidikan Otomatis](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="dede4-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="dede4-119">Anda juga dapat melindungi dari file dan URL berbahaya dengan mengikuti instruksi dalam [Perlindungan dari URL dan file berbahaya](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="dede4-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>