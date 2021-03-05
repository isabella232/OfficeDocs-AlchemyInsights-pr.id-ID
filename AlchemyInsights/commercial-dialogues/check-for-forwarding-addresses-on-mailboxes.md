---
title: Periksa alamat pengalihan pada kotak surat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482774"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="db120-102">Periksa alamat pengalihan pada kotak surat</span><span class="sxs-lookup"><span data-stu-id="db120-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="db120-103">Terkadang pengguna mengirim pesan email kepada mereka sendiri, jadi pertama-tama kami akan memeriksa alamat dan aturan penerusan pada kotak surat.</span><span class="sxs-lookup"><span data-stu-id="db120-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="db120-104">Lalu kita akan memeriksa log audit.</span><span class="sxs-lookup"><span data-stu-id="db120-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="db120-105">Berikut cara memeriksa alamat pengalihan:</span><span class="sxs-lookup"><span data-stu-id="db120-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="db120-106">Pilih **pengguna pengguna**  >  **aktif**.</span><span class="sxs-lookup"><span data-stu-id="db120-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="db120-107">Pilih pengguna yang akunnya telah dikompromikan.</span><span class="sxs-lookup"><span data-stu-id="db120-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="db120-108">Dalam Flyout yang muncul, Perluas **pengaturan email**, lalu klik **Edit** untuk **penerusan email**.</span><span class="sxs-lookup"><span data-stu-id="db120-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="db120-109">Hapus semua alamat penerusan yang tidak Anda kenali.</span><span class="sxs-lookup"><span data-stu-id="db120-109">Remove any forwarding addresses you don't recognize.</span></span>