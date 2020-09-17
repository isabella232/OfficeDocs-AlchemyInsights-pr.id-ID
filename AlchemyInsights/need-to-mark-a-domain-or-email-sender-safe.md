---
title: Perlu menandai domain atau pengirim email yang aman?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803248"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="f1d1e-102">Perlu menandai domain atau pengirim email yang aman?</span><span class="sxs-lookup"><span data-stu-id="f1d1e-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="f1d1e-103">Penggunaan **daftar pengirim aman tidak disarankan** karena membuka organisasi Anda ke spam, Phish, dan spoofing.</span><span class="sxs-lookup"><span data-stu-id="f1d1e-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="f1d1e-104">Namun, jika ada persyaratan bisnis, **sebaiknya gunakan** **[aturan alur email](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** untuk ini.</span><span class="sxs-lookup"><span data-stu-id="f1d1e-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="f1d1e-105">Panduan kami memastikan autentikasi pengirim (verifikasi pengiriman domain tidak bersifat palsu).</span><span class="sxs-lookup"><span data-stu-id="f1d1e-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="f1d1e-106">**Catatan**: kami tidak menyarankan mengelola false positive dengan menggunakan daftar pengirim aman, karena pengecualian untuk pemfilteran spam bisa membuka organisasi Anda untuk serangan keamanan.</span><span class="sxs-lookup"><span data-stu-id="f1d1e-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="f1d1e-107">Jika pengguna Anda menerima pesan yang salah ditandai sebagai email spam atau junk, silakan **[Laporkan pesan dan file ke Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="f1d1e-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="f1d1e-108">Pengirim aman di Outlook, daftar pengirim yang diperbolehkan, atau daftar domain yang diperbolehkan dalam kebijakan anti spam **harus dihindari** karena pengirim melewati semua spam, spoof, dan proteksi Phish, serta autentikasi pengirim (SPF, DKIM, dMarc).</span><span class="sxs-lookup"><span data-stu-id="f1d1e-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="f1d1e-109">Metode ini paling baik digunakan untuk uji sementara saja.</span><span class="sxs-lookup"><span data-stu-id="f1d1e-109">This method is best used for temporary testing only.</span></span>
