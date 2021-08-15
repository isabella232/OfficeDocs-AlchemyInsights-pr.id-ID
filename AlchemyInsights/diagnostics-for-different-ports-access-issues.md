---
title: Diagnostik untuk masalah akses port yang berbeda
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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030905"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostik untuk masalah akses port yang berbeda

Untuk mengatasi masalah akses port yang berbeda, lakukan langkah-langkah berikut ini:

1. Hentikan/deallocate mesin virtual (VM) dari portal, mulai ulang VM, dan uji lagi. 
2. Periksa pengaturan jaringan VM untuk mengetahui apakah Anda memiliki Network Security Groups (NSGs) yang memblokir lalu lintas. Anda juga dapat menggunakan alat verifikasi aliran IP Network Watcher untuk memeriksa NSGs yang memblokir lalu lintas, Rute User-Defined (UDR, [Network Watcher)](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) untuk kembali ke perangkat lokal ('Default Route' 0.0.0.0/0), atau ke alat jaringan.
Jika masih mengalami masalah setelah mencoba langkah-langkah di atas, harap sediakan nama VM dan port TCP yang sedang Anda coba untuk mengirim email untuk pemeriksaan lebih lanjut.

**Dokumen yang Disarankan**

[Batasan dan rekomendasi untuk mengirim email keluar melalui port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)