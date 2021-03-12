---
title: Secara otomatis mengenkripsi pesan email tertentu dari Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746133"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="92848-102">Secara otomatis mengenkripsi pesan email tertentu dari Office 365</span><span class="sxs-lookup"><span data-stu-id="92848-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="92848-103">Dari [Pusat admin Exchange](https://outlook.office365.com/ecp/), pilih **aturan > alur email**.</span><span class="sxs-lookup"><span data-stu-id="92848-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="92848-104">Klik ikon **baru (+)** , lalu klik **Terapkan enkripsi pesan Office 365 dan perlindungan hak ke pesan**.</span><span class="sxs-lookup"><span data-stu-id="92848-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="92848-105">Di **nama**, masukkan nama untuk aturan, seperti *Enkripsikan semua pesan*.</span><span class="sxs-lookup"><span data-stu-id="92848-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="92848-106">Dalam **menerapkan aturan ini**, pilih **[Terapkan ke semua pesan]**.</span><span class="sxs-lookup"><span data-stu-id="92848-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="92848-107">Di samping bidang **lakukan berikut** , klik **pilih satu**.</span><span class="sxs-lookup"><span data-stu-id="92848-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="92848-108">Di menu turun bawah **Templat RMS** , pilih **Enkripsikan**, lalu klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="92848-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="92848-109">(Jika Anda tidak melihat opsi ini, itu berarti paket Anda tidak menyertakan enkripsi otomatis.</span><span class="sxs-lookup"><span data-stu-id="92848-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="92848-110">Tapi Anda bisa menambahkannya!)</span><span class="sxs-lookup"><span data-stu-id="92848-110">But you can add it!)</span></span>
7. <span data-ttu-id="92848-111">Periksa kotak centang **audit aturan ini dengan tingkat keparahan** , lalu pilih tingkat yang diinginkan.</span><span class="sxs-lookup"><span data-stu-id="92848-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="92848-112">Jika perusahaan Anda memiliki kewajiban kontraktual untuk mengirim semua email terenkripsi, saya menyarankan untuk mengatur tingkat ke **tinggi**.</span><span class="sxs-lookup"><span data-stu-id="92848-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="92848-113">Di bawah **Pilih model untuk aturan ini**, klik **Terapkan**.</span><span class="sxs-lookup"><span data-stu-id="92848-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="92848-114">Pilih pilihan opsional apa pun (dari daftar pilihan opsional yang bisa Anda buat pada saat ini, banyak yang bisa dibiarkan dengan pengaturan default untuk kesederhanaan).</span><span class="sxs-lookup"><span data-stu-id="92848-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="92848-115">Klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="92848-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="92848-116">Anda dapat selalu kembali dan mengedit aturan ini nanti.</span><span class="sxs-lookup"><span data-stu-id="92848-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="92848-117">Untuk informasi selengkapnya tentang membuat aturan untuk enkripsi, lihat [menentukan aturan aliran email untuk mengenkripsi pesan email di Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="92848-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

