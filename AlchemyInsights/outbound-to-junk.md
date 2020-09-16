---
title: Email keluar ke folder email sampah
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769186"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="d4f68-102">Email keluar ke folder email sampah</span><span class="sxs-lookup"><span data-stu-id="d4f68-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="d4f68-103">Jika Anda melihat pesan keluar yang ditandai sebagai sampah, lakukan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="d4f68-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="d4f68-104">Jika belum melakukannya, pertimbangkan untuk [mengonfigurasi pemberitahuan kebijakan spam keluar](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="d4f68-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="d4f68-105">Gunakan [jejak pesan](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) untuk melihat apakah pesan keluar memiliki nilai kejadian **spam** dengan detail tambahan: **gunakan kumpulan pengiriman berisiko tinggi**.</span><span class="sxs-lookup"><span data-stu-id="d4f68-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="d4f68-106">Untuk pesan ini, periksa konten pesan untuk melihat apa yang mungkin dianggap spam.</span><span class="sxs-lookup"><span data-stu-id="d4f68-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="d4f68-107">Misalnya, tanda tangan bisa menyebabkan masalah bagi banyak pengguna.</span><span class="sxs-lookup"><span data-stu-id="d4f68-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="d4f68-108">Jika Anda memiliki beberapa contoh pesan keluar yang sah yang sedang ditandai sebagai sampah, buka tiket dukungan dan minta agen dukungan untuk mengirimkan pesan sebagai positif palsu kepada analis spam kami.</span><span class="sxs-lookup"><span data-stu-id="d4f68-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="d4f68-109">Bersiaplah untuk menyediakan contoh pesan yang menyertakan semua header pesan.</span><span class="sxs-lookup"><span data-stu-id="d4f68-109">Be prepared to provide sample messages that include all message headers.</span></span>
