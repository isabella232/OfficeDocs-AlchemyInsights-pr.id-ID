---
title: Menghapus versi MSI sebelumnya dari Office
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680723"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="4c579-102">Menghapus versi MSI sebelumnya dari Office</span><span class="sxs-lookup"><span data-stu-id="4c579-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="4c579-103">Saya menyarankan untuk menghapus Office versi penginstal Windows (MSI) sebelum menginstal Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="4c579-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="4c579-104">Berikut ini cara melakukan ini:</span><span class="sxs-lookup"><span data-stu-id="4c579-104">Here's how to do this:</span></span>

1. <span data-ttu-id="4c579-105">Jika Anda menggunakan MSI untuk menginstal Office, Anda bisa menggunakan Office Deployment Tool (ODT) untuk menghapus instalan Office.</span><span class="sxs-lookup"><span data-stu-id="4c579-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="4c579-106">Anda dapat menggunakan elemen RemoveMSI dalam file **configuration.xml** .</span><span class="sxs-lookup"><span data-stu-id="4c579-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="4c579-107">Ikuti instruksi dalam artikel ini: [pusat kepatuhan & keamanan Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="4c579-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>