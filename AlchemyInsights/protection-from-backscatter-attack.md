---
title: Proteksi dari serangan Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036074"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="5cf2c-102">Proteksi dari serangan Backscatter</span><span class="sxs-lookup"><span data-stu-id="5cf2c-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="5cf2c-103">Backscatter adalah laporan tidak terkirim (juga dikenal sebagai NDR atau pesan pantulan) yang Anda terima untuk pesan yang tidak terkirim.</span><span class="sxs-lookup"><span data-stu-id="5cf2c-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="5cf2c-104">Spammer menempa (spoof) Alamat **dari:** dari pesan mereka, dan mereka sering menggunakan alamat email nyata untuk meminjamkan kredibilitas pada pesan mereka.</span><span class="sxs-lookup"><span data-stu-id="5cf2c-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="5cf2c-105">Jadi, saat spammer tidak mau mengirimkan pesan ke penerima yang tidak ada, server email tujuan pada dasarnya ditipu untuk mengembalikan pesan yang tidak terkirim dalam NDR ke pengirim yang ditempa di alamat **dari:** .</span><span class="sxs-lookup"><span data-stu-id="5cf2c-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="5cf2c-106">Informasi tambahan dapat ditemukan dalam [Backscatter di EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="5cf2c-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="5cf2c-107">**Mengaktifkan proteksi Backscatter**</span><span class="sxs-lookup"><span data-stu-id="5cf2c-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="5cf2c-108">Untuk mengaktifkan proteksi Backscatter, ikuti jalur di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="5cf2c-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="5cf2c-109">**protection.office.com > Threat Management > Policy > AntiSpam > memilih kebijakan filter spam dan mengedit kebijakan > properti spam > Tandai sebagai spam > NDR Backscatter > menetapkannya ke "aktif"**</span><span class="sxs-lookup"><span data-stu-id="5cf2c-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="5cf2c-110">Jika Anda yakin akun telah disalahgunakan, lihat yang berikut ini:</span><span class="sxs-lookup"><span data-stu-id="5cf2c-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="5cf2c-111">Membalas akun email yang dikompromikan</span><span class="sxs-lookup"><span data-stu-id="5cf2c-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="5cf2c-112">Menghapus pengguna yang diblokir dari portal pengguna terbatas di Office 365</span><span class="sxs-lookup"><span data-stu-id="5cf2c-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



