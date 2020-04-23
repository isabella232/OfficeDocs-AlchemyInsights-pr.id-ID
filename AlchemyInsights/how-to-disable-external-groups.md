---
title: Cara menonaktifkan eksternal grup
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720771"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="0c5b7-102">Cara menonaktifkan eksternal grup</span><span class="sxs-lookup"><span data-stu-id="0c5b7-102">How to disable External Groups</span></span>

<span data-ttu-id="0c5b7-103">Pesan eksternal Yammer berlaku Exchange Transport Rules (ETRs), seperangkat kontrol proaktif untuk mencegah berbagi informasi perusahaan.</span><span class="sxs-lookup"><span data-stu-id="0c5b7-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="0c5b7-104">Untuk membatasi pengguna membuat grup eksternal, Anda harus mengkonfigurasi aturan transpor Exchange (ETR), dan kemudian mengkonfigurasi heboh menggunakan aturan Exchange Transport untuk memblokir pesan eksternal.</span><span class="sxs-lookup"><span data-stu-id="0c5b7-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="0c5b7-105">Setelah Anda membuat aturan di Exchange Online Admin Center, ikuti langkah berikut untuk menetapkan ETR untuk menerapkan di heboh:</span><span class="sxs-lookup"><span data-stu-id="0c5b7-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="0c5b7-106">Log on ke heboh sebagai admin diverifikasi, dan di **Pusat admin heboh**, pergi ke C **konten dan pengaturan keamanan keamanan \> .**</span><span class="sxs-lookup"><span data-stu-id="0c5b7-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="0c5b7-107">Di bawah **pesan eksternal**, pilih **menerapkan Exchange Online Exchange Transport Rules (etrs) di Yammer.**</span><span class="sxs-lookup"><span data-stu-id="0c5b7-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="0c5b7-108">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="0c5b7-108">Choose **Save**.</span></span>

<span data-ttu-id="0c5b7-109">Untuk informasi selengkapnya, lihat [menonaktifkan pesan eksternal di jaringan heboh](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="0c5b7-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  