---
title: Diagnosis untuk masalah Access port yang berbeda
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035781"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="5a3a8-102">Diagnosis untuk masalah Access port yang berbeda</span><span class="sxs-lookup"><span data-stu-id="5a3a8-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="5a3a8-103">Untuk mengatasi masalah Access port yang berbeda, lakukan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="5a3a8-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="5a3a8-104">Hentikan/deallocate mesin virtual (VM) dari portal, mulai ulang VM, dan uji lagi.</span><span class="sxs-lookup"><span data-stu-id="5a3a8-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="5a3a8-105">Periksa pengaturan jaringan VM Anda untuk mengetahui apakah Anda memiliki jaringan keamanan grup (NSGs) yang memblokir Traffic.</span><span class="sxs-lookup"><span data-stu-id="5a3a8-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="5a3a8-106">Anda juga dapat menggunakan [alat verifikasi alur jaringan](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) untuk memeriksa lalu lintas pemblokiran, User-Defined rute (udrs) lalu lintas kembali ke lokal (' rute default ' 0.0.0.0/0), atau ke alat jaringan.</span><span class="sxs-lookup"><span data-stu-id="5a3a8-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="5a3a8-107">Jika Anda masih mengalami masalah setelah mencoba langkah-langkah di atas, Harap berikan nama VM dan port TCP yang sedang Anda coba untuk mengirim email untuk diagnosis lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="5a3a8-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="5a3a8-108">**Dokumen yang Disarankan**</span><span class="sxs-lookup"><span data-stu-id="5a3a8-108">**Recommended Documents**</span></span>

[<span data-ttu-id="5a3a8-109">Keterbatasan dan rekomendasi untuk mengirimkan email keluar melalui port 25</span><span class="sxs-lookup"><span data-stu-id="5a3a8-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)