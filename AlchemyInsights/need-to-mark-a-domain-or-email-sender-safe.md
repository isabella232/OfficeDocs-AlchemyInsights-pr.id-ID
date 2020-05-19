---
title: Perlu untuk menandai domain atau pengirim email yang aman?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281175"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="f46e1-102">Perlu untuk menandai domain atau pengirim email yang aman?</span><span class="sxs-lookup"><span data-stu-id="f46e1-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="f46e1-103">Penggunaan **daftar pengirim aman tidak disarankan** karena membuka organisasi Anda untuk spam, Phish, dan serangan spoofing.</span><span class="sxs-lookup"><span data-stu-id="f46e1-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="f46e1-104">Namun, jika ada kebutuhan bisnis, kami **sarankan** menggunakan **[mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** untuk ini.</span><span class="sxs-lookup"><span data-stu-id="f46e1-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="f46e1-105">Panduan kami memastikan autentikasi pengirim (memverifikasi pengiriman domain tidak diputus).</span><span class="sxs-lookup"><span data-stu-id="f46e1-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="f46e1-106">**Catatan**: kami tidak menyarankan mengelola positif palsu dengan menggunakan daftar pengirim yang aman, karena pengecualian untuk pemfilteran spam dapat membuka organisasi Anda untuk serangan keamanan.</span><span class="sxs-lookup"><span data-stu-id="f46e1-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="f46e1-107">Jika pengguna Anda (s) menerima pesan salah ditandai sebagai spam atau email sampah, silakan **[Laporkan pesan dan file ke Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="f46e1-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="f46e1-108">Pengirim aman di Outlook, daftar pengirim yang diizinkan, atau daftar domain yang dibolehkan dalam kebijakan anti-spam **harus dihindari** karena pengirim mengabaikan semua spam, spoof, dan perlindungan Phish, serta autentikasi pengirim (SPF, DKIM, dMarc).</span><span class="sxs-lookup"><span data-stu-id="f46e1-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="f46e1-109">Metode ini paling tepat digunakan untuk pengujian sementara saja.</span><span class="sxs-lookup"><span data-stu-id="f46e1-109">This method is best used for temporary testing only.</span></span>
