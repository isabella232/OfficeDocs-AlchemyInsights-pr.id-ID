---
title: Rekaman panggilan 1:1
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
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696961"
---
# <a name="11-call-recording"></a>Rekaman panggilan 1:1

Jika tombol **Mulai Perekaman** berwarna abu-abu dalam panggilan 1:1, Anda perlu mengubah pengaturan kebijakan untuk pengguna yang terkena dampak.   

Mulai 31 Mei 2021, kami akan mulai memberlakukan Kebijakan Teams *Baru AllowCloudRecordingForCalls*. Sebelum perubahan ini, rekaman panggilan 1:1 dikontrol oleh *AllowCloudRecording Teams* Meeting. Perubahan ini didokumentasikan dalam postingan Pusat Pesan: [(Diperbarui) 1:1 Pengenalan kebijakan perekaman panggilan](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   opsi kebijakan panggilan otomatis diatur **$False** secara default. Jika Anda lebih suka memblokir semua pengguna merekam panggilan 1:1, Anda tidak perlu melakukan tindakan apa pun.  

Untuk mengaktifkan perekaman panggilan bagi semua pengguna dalam panggilan 1:1, gunakan Teams PowerShell untuk menjalankan cmdlet berikut: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternatifnya, Anda bisa membuat kebijakan baru dan mengatur **-AllowCloudRecordingForCalls** **$true** dan menetapkan kebijakan tersebut ke pengguna Anda. 

Untuk informasi selengkapnya, lihat [Kontrol Kebijakan Perekaman Panggilan 1:1 Are (Hampir!) Di sini](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
