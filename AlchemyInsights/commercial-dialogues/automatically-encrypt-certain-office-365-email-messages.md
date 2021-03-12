---
title: Secara otomatis mengenkripsi pesan email Office 365 tertentu
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746128"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="d5333-102">Secara otomatis mengenkripsi pesan email Office 365 tertentu</span><span class="sxs-lookup"><span data-stu-id="d5333-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="d5333-103">Anda dapat secara otomatis mengenkripsi pesan yang dikirim pengguna ke orang atau organisasi tertentu.</span><span class="sxs-lookup"><span data-stu-id="d5333-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="d5333-104">Untuk melakukan ini, lakukan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="d5333-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="d5333-105">Dari [Pusat admin Exchange](https://outlook.office365.com/ecp/), pilih **aturan > alur email**.</span><span class="sxs-lookup"><span data-stu-id="d5333-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="d5333-106">Klik ikon **baru (+)** , lalu klik **Terapkan enkripsi pesan Office 365 dan perlindungan hak ke pesan**.</span><span class="sxs-lookup"><span data-stu-id="d5333-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="d5333-107">Di **nama**, masukkan nama untuk aturan tersebut, seperti *mengenkripsi pesan yang dikirim ke DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="d5333-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="d5333-108">Dalam **menerapkan aturan ini**, pilih **penerima > adalah orang ini**.</span><span class="sxs-lookup"><span data-stu-id="d5333-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="d5333-109">Di jendela **pilih anggota** , pilih nama orang yang ingin Anda Terapkan aturan enkripsi, lalu klik **Tambahkan**.</span><span class="sxs-lookup"><span data-stu-id="d5333-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="d5333-110">Bila Anda sudah selesai menambahkan pengguna, klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="d5333-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="d5333-111">Di samping bidang **lakukan berikut** , klik **pilih satu**.</span><span class="sxs-lookup"><span data-stu-id="d5333-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="d5333-112">Di menu turun bawah **Templat RMS** , pilih **Enkripsikan**, lalu klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="d5333-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="d5333-113">(Jika Anda tidak melihat opsi ini, itu berarti paket Anda tidak menyertakan enkripsi otomatis.</span><span class="sxs-lookup"><span data-stu-id="d5333-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="d5333-114">Tapi Anda bisa menambahkannya!)</span><span class="sxs-lookup"><span data-stu-id="d5333-114">But you can add it!)</span></span>
9. <span data-ttu-id="d5333-115">Pilih pilihan opsional apa pun (dari daftar pilihan opsional yang bisa Anda buat pada saat ini, banyak yang bisa dibiarkan dengan pengaturan default untuk kesederhanaan).</span><span class="sxs-lookup"><span data-stu-id="d5333-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="d5333-116">Klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="d5333-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d5333-117">Anda dapat selalu kembali dan mengedit aturan ini nanti.</span><span class="sxs-lookup"><span data-stu-id="d5333-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="d5333-118">Untuk informasi selengkapnya tentang membuat aturan untuk enkripsi, lihat [menentukan aturan aliran email untuk mengenkripsi pesan email di Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="d5333-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

