---
title: Cara menonaktifkan eksternal grup
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739496"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="06c2b-102">Cara menonaktifkan eksternal grup</span><span class="sxs-lookup"><span data-stu-id="06c2b-102">How to disable External Groups</span></span>

<span data-ttu-id="06c2b-103">Pesan eksternal Yammer berlaku Exchange Transport Rules (ETRs), seperangkat kontrol proaktif untuk mencegah berbagi informasi perusahaan.</span><span class="sxs-lookup"><span data-stu-id="06c2b-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="06c2b-104">Untuk membatasi pengguna membuat grup eksternal, Anda harus mengkonfigurasi aturan transpor Exchange (ETR), dan kemudian mengkonfigurasi heboh menggunakan aturan Exchange Transport untuk memblokir pesan eksternal.</span><span class="sxs-lookup"><span data-stu-id="06c2b-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="06c2b-105">Setelah Anda membuat aturan di Exchange Online Admin Center, ikuti langkah berikut untuk menetapkan ETR untuk menerapkan di heboh:</span><span class="sxs-lookup"><span data-stu-id="06c2b-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="06c2b-106">Log on ke heboh sebagai admin diverifikasi, dan di **Pusat admin heboh**, pergi ke C **konten dan pengaturan keamanan keamanan \> .**</span><span class="sxs-lookup"><span data-stu-id="06c2b-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="06c2b-107">Di bawah **pesan eksternal**, pilih **menerapkan Exchange Online Exchange Transport Rules (etrs) di Yammer.**</span><span class="sxs-lookup"><span data-stu-id="06c2b-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="06c2b-108">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="06c2b-108">Choose **Save**.</span></span>

<span data-ttu-id="06c2b-109">Untuk informasi selengkapnya, lihat [menonaktifkan pesan eksternal di jaringan heboh](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="06c2b-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  