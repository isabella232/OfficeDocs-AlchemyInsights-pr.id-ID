---
title: Memblokir tanda tangan email yang dibuat pengguna
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243638"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="a1417-102">Memblokir tanda tangan email yang dibuat pengguna</span><span class="sxs-lookup"><span data-stu-id="a1417-102">Block user-made email signatures</span></span>

<span data-ttu-id="a1417-103">Solusi berikut ini hanya berlaku untuk tanda tangan email yang dibuat di Outlook di web.</span><span class="sxs-lookup"><span data-stu-id="a1417-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="a1417-104">Anda hanya bisa memblokir tanda tangan di aplikasi Outlook jika Anda memiliki server Exchange di tempat.</span><span class="sxs-lookup"><span data-stu-id="a1417-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="a1417-105">Di pusat admin, pilih Exchange **Pusat admin**  >  .</span><span class="sxs-lookup"><span data-stu-id="a1417-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="a1417-106">Klik **izin**  >  **kebijakan Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="a1417-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="a1417-107">Pilih kebijakan, lalu klik ikon pensil untuk mengeditnya.</span><span class="sxs-lookup"><span data-stu-id="a1417-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="a1417-108">Klik **fitur**  >  **lainnya**.</span><span class="sxs-lookup"><span data-stu-id="a1417-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="a1417-109">Di bawah **pengalaman pengguna**, kosongkan kotak centang **tanda tangan email** , lalu klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="a1417-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="a1417-110">**Penting:** Jika tanda tangan ditambahkan sebelum mengosongkan kotak centang ini, pengguna masih dapat menggunakannya.</span><span class="sxs-lookup"><span data-stu-id="a1417-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="a1417-111">Mintalah mereka menghapusnya.</span><span class="sxs-lookup"><span data-stu-id="a1417-111">Ask them to remove it.</span></span>
