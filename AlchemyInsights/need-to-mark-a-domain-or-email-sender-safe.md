---
title: Perlu menandai domain atau pengirim email dengan aman?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792135"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="d4121-102">Perlu menandai domain atau pengirim email dengan aman?</span><span class="sxs-lookup"><span data-stu-id="d4121-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="d4121-103">Penggunaan daftar **pengirim aman tidak direkomendasikan karena** membuka organisasi Anda untuk serangan spam, pengelabuan, dan spoofing.</span><span class="sxs-lookup"><span data-stu-id="d4121-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="d4121-104">Namun, jika ada persyaratan bisnis, kami menyarankan **Agar Anda** menggunakan **[Aturan Aliran Email](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** untuk hal ini.</span><span class="sxs-lookup"><span data-stu-id="d4121-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="d4121-105">Panduan kami memastikan bahwa autentikasi pengirim (memverifikasi bahwa domain yang dikirim tidak merupakan spoofed).</span><span class="sxs-lookup"><span data-stu-id="d4121-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="d4121-106">**Catatan**: Kami tidak menyarankan Anda mengelola positif palsu dengan menggunakan daftar pengirim aman, karena pengecualian pemfilteran spam dapat membuka organisasi Anda untuk serangan keamanan.</span><span class="sxs-lookup"><span data-stu-id="d4121-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="d4121-107">Jika pengguna Anda menerima pesan yang salah ditandai sebagai spam atau email sampah, silakan **[Laporkan pesan dan file ke Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="d4121-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="d4121-108">Pengirim Aman di Outlook, Daftar pengirim yang diperbolehkan, atau  daftar domain yang diperbolehkan dalam kebijakan anti spam harus dihindari karena pengirim melewati semua spam, spoof, dan proteksi phish, serta autentikasi pengirim (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="d4121-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="d4121-109">Metode ini paling baik digunakan untuk pengujian sementara saja.</span><span class="sxs-lookup"><span data-stu-id="d4121-109">This method is best used for temporary testing only.</span></span>
