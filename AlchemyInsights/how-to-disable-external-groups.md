---
title: Cara menonaktifkan grup eksternal
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704131"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="060e1-102">Cara menonaktifkan grup eksternal</span><span class="sxs-lookup"><span data-stu-id="060e1-102">How to disable External Groups</span></span>

<span data-ttu-id="060e1-103">Pesan eksternal Yammer menerapkan Exchange Transport Rules (ETRs), sekumpulan kontrol proaktif untuk mencegah agar informasi perusahaan tidak dibagikan.</span><span class="sxs-lookup"><span data-stu-id="060e1-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="060e1-104">Untuk membatasi pengguna dari membuat grup eksternal, Anda perlu mengonfigurasi aturan transpor Exchange (ETR), lalu mengonfigurasi Yammer untuk menggunakan aturan transpor Exchange untuk memblokir pesan eksternal.</span><span class="sxs-lookup"><span data-stu-id="060e1-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="060e1-105">Setelah Anda membuat aturan di pusat admin Exchange Online, ikuti langkah-langkah ini untuk mengatur ETR untuk diterapkan di Yammer:</span><span class="sxs-lookup"><span data-stu-id="060e1-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="060e1-106">Masuk ke Yammer sebagai admin terverifikasi, dan di **Pusat admin Yammer**, masuk ke **konten C dan \> pengaturan keamanan keamanan.**</span><span class="sxs-lookup"><span data-stu-id="060e1-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="060e1-107">Di bawah **pesan eksternal**, pilih **Terapkan aturan transpor Exchange Online Exchange (etrs) di Yammer.**</span><span class="sxs-lookup"><span data-stu-id="060e1-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="060e1-108">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="060e1-108">Choose **Save**.</span></span>

<span data-ttu-id="060e1-109">Untuk informasi selengkapnya, lihat [menonaktifkan pesan eksternal di jaringan Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="060e1-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  