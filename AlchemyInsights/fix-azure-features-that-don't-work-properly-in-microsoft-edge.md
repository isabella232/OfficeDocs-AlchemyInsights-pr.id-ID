---
title: Apa yang harus dilakukan jika fitur Azure tidak berfungsi dengan baik di Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583459"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="3d91d-102">Apa yang harus dilakukan jika fitur Azure tidak berfungsi dengan baik di Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3d91d-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="3d91d-103">Microsoft Edge telah [mengetahui masalah](https://go.microsoft.com/fwlink/?linkid=2140608) yang terkait dengan zona keamanan dan mungkin mempengaruhi cara pengguna Azure masuk ke Pusat admin Windows.</span><span class="sxs-lookup"><span data-stu-id="3d91d-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="3d91d-104">Jika Anda mengalami masalah dalam menggunakan fitur Azure dengan Microsoft Edge, cobalah langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="3d91d-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="3d91d-105">Di menu **mulai** , Cari **Opsi Internet** dan pilih.</span><span class="sxs-lookup"><span data-stu-id="3d91d-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="3d91d-106">Dalam kotak dialog **properti Internet** , masuk ke tab **keamanan** .</span><span class="sxs-lookup"><span data-stu-id="3d91d-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="3d91d-107">Pilih zona **situs tepercaya** lalu pilih tombol **situs** .</span><span class="sxs-lookup"><span data-stu-id="3d91d-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="3d91d-108">Dalam kotak dialog **situs tepercaya** , Tambahkan URL Gateway Anda serta [https://login.microsoftonline.com](https://login.microsoftonline.com) , lalu [https://login.live.com](https://login.live.com) pilih **tutup**.</span><span class="sxs-lookup"><span data-stu-id="3d91d-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="3d91d-109">Dalam kotak dialog **properti Internet** , masuk ke tab **privasi** .</span><span class="sxs-lookup"><span data-stu-id="3d91d-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="3d91d-110">Di bagian **Pemblokir pop-up** , pilih **pengaturan**.</span><span class="sxs-lookup"><span data-stu-id="3d91d-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="3d91d-111">Dalam kotak dialog yang terbuka, Tambahkan URL Gateway Anda serta [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) , lalu pilih **tutup**.</span><span class="sxs-lookup"><span data-stu-id="3d91d-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
