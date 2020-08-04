---
title: Menjeda pembaruan terjadwal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555510"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="2b657-102">Menjeda pembaruan terjadwal</span><span class="sxs-lookup"><span data-stu-id="2b657-102">Pausing scheduled updates</span></span>

<span data-ttu-id="2b657-103">Ketika perintah jeda dikeluarkan, perangkat tidak memproses perintah sampai waktu berikutnya mereka Check-in ke Intune.</span><span class="sxs-lookup"><span data-stu-id="2b657-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="2b657-104">Karena itu, perangkat Anda mungkin memiliki:</span><span class="sxs-lookup"><span data-stu-id="2b657-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="2b657-105">Menginstal pembaruan terjadwal sebelum Check-in.</span><span class="sxs-lookup"><span data-stu-id="2b657-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="2b657-106">Dimatikan ketika Anda mengeluarkan perintah jeda.</span><span class="sxs-lookup"><span data-stu-id="2b657-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="2b657-107">Dalam hal ini, ketika perangkat dihidupkan, mereka mungkin telah didownload dan diinstal update dijadwalkan sebelum Check-in.</span><span class="sxs-lookup"><span data-stu-id="2b657-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>