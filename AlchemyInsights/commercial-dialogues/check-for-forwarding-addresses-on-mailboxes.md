---
title: Memeriksa penerusan alamat pada kotak surat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403314"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="53e61-102">Memeriksa penerusan alamat pada kotak surat</span><span class="sxs-lookup"><span data-stu-id="53e61-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="53e61-103">Terkadang peretas meneruskan pesan email pengguna ke diri mereka sendiri, jadi pertama-dulu kita akan memeriksa penerusan alamat dan aturan di kotak surat.</span><span class="sxs-lookup"><span data-stu-id="53e61-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="53e61-104">Maka kami akan memeriksa log audit tersebut.</span><span class="sxs-lookup"><span data-stu-id="53e61-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="53e61-105">Berikut cara memeriksa alamat penerusan:</span><span class="sxs-lookup"><span data-stu-id="53e61-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="53e61-106">Pilih **Pengguna**  >  **Pengguna aktif.**</span><span class="sxs-lookup"><span data-stu-id="53e61-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="53e61-107">Pilih pengguna yang akunnya telah dibobol.</span><span class="sxs-lookup"><span data-stu-id="53e61-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="53e61-108">Di flyout yang muncul, **perluas Pengaturan Email**, lalu klik **Edit** untuk **Penerusan email.**</span><span class="sxs-lookup"><span data-stu-id="53e61-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="53e61-109">Hapus setiap alamat penerusan yang tidak Anda kenali.</span><span class="sxs-lookup"><span data-stu-id="53e61-109">Remove any forwarding addresses you don't recognize.</span></span>