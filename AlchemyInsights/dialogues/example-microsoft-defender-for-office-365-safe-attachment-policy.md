---
title: Contoh kebijakan Microsoft Defender untuk Office 365 Safe attachment
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693828"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="2d637-102">Contoh kebijakan Microsoft Defender untuk Office 365 Safe attachment</span><span class="sxs-lookup"><span data-stu-id="2d637-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="2d637-103">Pengaturan ini mengaktifkan kebijakan yang *tidak disebut keterlambatan* yang akan mengirimkan pesan dengan segera lalu melepaskan kembali lampiran setelah dipindai:</span><span class="sxs-lookup"><span data-stu-id="2d637-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="2d637-104">**Nama**: tidak ada keterlambatan</span><span class="sxs-lookup"><span data-stu-id="2d637-104">**Name**: No delays</span></span>
- <span data-ttu-id="2d637-105">**Deskripsi**: mengirimkan pesan dengan segera dan melampirkan kembali lampiran setelah pemindaian.</span><span class="sxs-lookup"><span data-stu-id="2d637-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="2d637-106">**Respons**: Pilih opsi **pengiriman dinamis** .</span><span class="sxs-lookup"><span data-stu-id="2d637-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="2d637-107">Untuk informasi selengkapnya, lihat [pengiriman dinamis dalam kebijakan lampiran aman](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="2d637-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="2d637-108">Bagian **lampiran pengalihan** : Pilih opsi untuk **mengaktifkan pengalihan**, lalu masukkan alamat email administrator global Microsoft 365, administrator keamanan, atau analis keamanan yang akan menyelidiki lampiran berbahaya.</span><span class="sxs-lookup"><span data-stu-id="2d637-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="2d637-109">**Diterapkan ke** bagian: Pilih **domain Penerima**, lalu pilih domain Anda.</span><span class="sxs-lookup"><span data-stu-id="2d637-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="2d637-110">Pilih **Tambahkan**, lalu pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="2d637-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="2d637-111">Setelah selesai, pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="2d637-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="2d637-112">Untuk mempelajari selengkapnya, lihat [lampiran aman di Microsoft Defender untuk Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="2d637-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
