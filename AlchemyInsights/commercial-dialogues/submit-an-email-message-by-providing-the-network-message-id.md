---
title: Mengirim pesan email dengan menyediakan ID pesan jaringan
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745519"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="d529a-102">Mengirim pesan email dengan menyediakan ID pesan jaringan</span><span class="sxs-lookup"><span data-stu-id="d529a-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="d529a-103">Dalam Flyout **penyerahan baru** , pilih **email** dan **id pesan jaringan**.</span><span class="sxs-lookup"><span data-stu-id="d529a-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="d529a-104">Ikuti langkah-langkah ini untuk menemukan ID pesan untuk pesan email di Outlook:</span><span class="sxs-lookup"><span data-stu-id="d529a-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="d529a-105">Klik ganda pesan email untuk membukanya.</span><span class="sxs-lookup"><span data-stu-id="d529a-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="d529a-106">Pilih   >  **properti** file.</span><span class="sxs-lookup"><span data-stu-id="d529a-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="d529a-107">Buka Notepad atau dokumen Word kosong, lalu salin dan tempel konten yang ditemukan di kotak **header Internet** ke dalam dokumen yang terbuka untuk visibilitas yang lebih baik.</span><span class="sxs-lookup"><span data-stu-id="d529a-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="d529a-108">Temukan bidang **id pesan-jaringan-X-MS-Exchange-organisasi** .</span><span class="sxs-lookup"><span data-stu-id="d529a-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="d529a-109">Nilai setelah **:** adalah id yang Anda perlukan untuk pengiriman Anda.</span><span class="sxs-lookup"><span data-stu-id="d529a-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="d529a-110">Di bawah **penerima**, jika email mendarat di folder email sampah untuk semua penerima email ini, pilih **Pilih Semua**.</span><span class="sxs-lookup"><span data-stu-id="d529a-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="d529a-111">Jika tidak, pilih hanya pengguna yang melaporkan masalahnya.</span><span class="sxs-lookup"><span data-stu-id="d529a-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="d529a-112">Di **bawah alasan untuk penyerahan**, jika Anda **memilih seharusnya diblokir**, Tentukan apakah pesan tersebut seharusnya diblokir sebagai **spam**, **phishing**, atau **malware**, lalu pilih **kirim**.</span><span class="sxs-lookup"><span data-stu-id="d529a-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="d529a-113">Untuk mempelajari selengkapnya, lihat [cara mengirimkan dugaan spam, Phish, URL, dan file ke Microsoft untuk pemindaian](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="d529a-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
