---
title: perekaman panggilan 1:1
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733852"
---
# <a name="11-call-recording"></a>perekaman panggilan 1:1

Administrator perlu melakukan tindakan sekarang untuk terus memungkinkan pengguna merekam panggilan 1:1.
 
Mulai 12 April 2021, kita akan mulai memberlakukan opsi kebijakan panggilan teams baru *Allowcloudrecordingforcalls*. 

Saat ini kemampuan perekaman panggilan 1:1 dikontrol oleh opsi *Allowcloudrecording* di kebijakan teams Rapat. Jika pengguna Anda diperbolehkan untuk merekam Rapat teams, mereka juga bisa merekam panggilan 1:1.

Jika Anda lebih suka memblokir semua pengguna dari merekam panggilan 1:1, Anda tidak perlu melakukan tindakan apa pun. Opsi kebijakan panggilan *Allowcloudrecordingforcalls* akan $false secara default.

Perubahan ini didokumentasikan dalam postingan pusat pesan berikut ini: [(Diperbarui) pengenalan kebijakan perekaman panggilan 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) untuk mengatur opsi kebijakan panggilan teams Anda harus menggunakan [teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Untuk mengaktifkan perekaman panggilan di panggilan 1:1:** Set-CsTeamsCallingPolicy-identitas global-AllowCloudRecordingForCalls $True

**Untuk menonaktifkan perekaman panggilan di panggilan 1:1:** Set-CsTeamsCallingPolicy-identitas global-AllowCloudRecordingForCalls $false

