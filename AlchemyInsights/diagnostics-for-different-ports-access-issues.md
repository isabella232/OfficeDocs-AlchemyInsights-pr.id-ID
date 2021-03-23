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
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnosis untuk masalah Access port yang berbeda

Untuk mengatasi masalah Access port yang berbeda, lakukan langkah-langkah berikut:

1. Hentikan/deallocate mesin virtual (VM) dari portal, mulai ulang VM, dan uji lagi. 
2. Periksa pengaturan jaringan VM Anda untuk mengetahui apakah Anda memiliki jaringan keamanan grup (NSGs) yang memblokir Traffic. Anda juga dapat menggunakan [alat verifikasi alur jaringan](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) untuk memeriksa lalu lintas pemblokiran, User-Defined rute (udrs) lalu lintas kembali ke lokal (' rute default ' 0.0.0.0/0), atau ke alat jaringan.
Jika Anda masih mengalami masalah setelah mencoba langkah-langkah di atas, Harap berikan nama VM dan port TCP yang sedang Anda coba untuk mengirim email untuk diagnosis lebih lanjut.

**Dokumen yang Disarankan**

[Keterbatasan dan rekomendasi untuk mengirimkan email keluar melalui port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)