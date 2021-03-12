---
title: Secara otomatis mengenkripsi pesan email Office 365 yang dikirim ke domain tertentu
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746049"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="c0b7d-102">Secara otomatis mengenkripsi pesan email Office 365 yang dikirim ke domain tertentu</span><span class="sxs-lookup"><span data-stu-id="c0b7d-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="c0b7d-103">Dari [Pusat admin Exchange](https://outlook.office365.com/ecp/), pilih **aturan > alur email**.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="c0b7d-104">Klik ikon **baru (+)** , lalu klik **Terapkan enkripsi pesan Office 365 dan perlindungan hak ke pesan**.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="c0b7d-105">Di **nama**, masukkan nama untuk aturan tersebut, seperti *mengenkripsi pesan yang dikirim ke contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="c0b7d-106">Dalam **menerapkan aturan ini**, pilih **penerima domain >**.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="c0b7d-107">Masukkan nama domain, seperti **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="c0b7d-108">Klik ikon **Tambahkan (+)** , lalu klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="c0b7d-109">Di samping bidang **lakukan berikut** , klik **pilih satu**.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="c0b7d-110">Di menu turun bawah **Templat RMS** , pilih **Enkripsikan**, lalu klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="c0b7d-111">(Jika Anda tidak melihat opsi ini, itu berarti paket Anda tidak menyertakan enkripsi otomatis.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="c0b7d-112">Tapi Anda bisa menambahkannya!)</span><span class="sxs-lookup"><span data-stu-id="c0b7d-112">But you can add it!)</span></span>
9. <span data-ttu-id="c0b7d-113">Pilih pilihan opsional apa pun (dari daftar pilihan opsional yang bisa Anda buat pada saat ini, banyak yang bisa dibiarkan dengan pengaturan default untuk kesederhanaan).</span><span class="sxs-lookup"><span data-stu-id="c0b7d-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="c0b7d-114">Klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c0b7d-115">Anda dapat selalu kembali dan mengedit aturan ini nanti.</span><span class="sxs-lookup"><span data-stu-id="c0b7d-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="c0b7d-116">Untuk informasi selengkapnya tentang membuat aturan untuk enkripsi, lihat [menentukan aturan aliran email untuk mengenkripsi pesan email di Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="c0b7d-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>