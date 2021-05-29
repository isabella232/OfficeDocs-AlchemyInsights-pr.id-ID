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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702093"
---
# <a name="11-call-recording"></a>Rekaman panggilan 1:1

Jika tombol **Mulai Perekaman** berwarna abu-abu dalam panggilan 1:1, Anda perlu mengubah pengaturan kebijakan untuk pengguna yang terkena dampak. Untuk memeriksa pengaturan kebijakan, jalankan Diagnostik untuk pengguna yang terkena dampak dengan mengetik **diag: Teams 1:1** Perekaman Panggilan di atas.     

Mulai 31 Mei 2021, kami akan mulai memberlakukan Kebijakan Teams *Baru AllowCloudRecordingForCalls*. Sebelum perubahan ini, rekaman panggilan 1:1 dikontrol oleh *AllowCloudRecording Teams* Meeting. Perubahan ini didokumentasikan dalam postingan Pusat Pesan: [(Diperbarui) 1:1 Pengenalan kebijakan perekaman panggilan](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   opsi kebijakan panggilan otomatis diatur **$False** secara default. Jika Anda lebih suka memblokir semua pengguna merekam panggilan 1:1, Anda tidak perlu melakukan tindakan apa pun.  

Untuk mengaktifkan perekaman panggilan bagi semua pengguna dalam panggilan 1:1, [gunakan Teams PowerShell](/microsoftteams/teams-powershell-install) untuk menjalankan cmdlet berikut: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternatifnya, Anda bisa membuat kebijakan baru dan mengatur **-AllowCloudRecordingForCalls** **$true** dan menetapkan kebijakan tersebut ke pengguna Anda. 

Untuk informasi selengkapnya, lihat [Kontrol Kebijakan Perekaman Panggilan 1:1 Are (Hampir!) Di sini](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
