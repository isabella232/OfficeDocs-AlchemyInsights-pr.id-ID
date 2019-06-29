---
title: Cara menonaktifkan kelompok-kelompok eksternal
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
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384828"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="cc970-102">Cara menonaktifkan kelompok-kelompok eksternal</span><span class="sxs-lookup"><span data-stu-id="cc970-102">How to disable External Groups</span></span>

<span data-ttu-id="cc970-103">Heboh pesan eksternal berlaku Aturan Transport Exchange (atas gaji setiap bulan), set proaktif kontrol untuk mencegah informasi perusahaan dari sedang dibagi.</span><span class="sxs-lookup"><span data-stu-id="cc970-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="cc970-104">Untuk membatasi pengguna membuat grup eksternal, Anda perlu mengkonfigurasi aturan transport Exchange (ETR), dan kemudian mengkonfigurasi heboh menggunakan aturan Exchange Transport untuk memblokir pesan eksternal.</span><span class="sxs-lookup"><span data-stu-id="cc970-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="cc970-105">Setelah Anda membuat aturan di Exchange Online admin center, ikuti langkah berikut untuk menetapkan ETR untuk menerapkan di heboh:</span><span class="sxs-lookup"><span data-stu-id="cc970-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="cc970-106">Log on ke heboh sebagai admin diverifikasi, dan dalam **heboh Pusat admin**, pergi ke C **konten dan keamanan \> pengaturan keamanan.**</span><span class="sxs-lookup"><span data-stu-id="cc970-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="cc970-107">**Pesan eksternal**, pilih **menegakkan Anda Exchange Online Aturan Transport Exchange (atas gaji setiap bulan) di heboh.**</span><span class="sxs-lookup"><span data-stu-id="cc970-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="cc970-108">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="cc970-108">Choose **Save**.</span></span>

<span data-ttu-id="cc970-109">Untuk selengkapnya, lihat [kontrol eksternal messaging jaringan heboh dengan aturan Exchange Transport](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="cc970-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  