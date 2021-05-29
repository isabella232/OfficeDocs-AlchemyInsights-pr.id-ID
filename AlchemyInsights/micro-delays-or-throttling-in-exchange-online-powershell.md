---
title: Penundaan atau pembatasan mikro di Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702129"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Penundaan atau pembatasan mikro di Exchange Online PowerShell

Anda mungkin melihat peringatan "Keterlambatan mikro diterapkan" atau keterlambatan ketika menjalankan skrip dan cmdlet di Exchange Online. Berikut beberapa saran untuk mengatasi masalah ini:

- Jalankan diagnostik kami untuk blak-atik kebijakan pembatasan PowerShell penyewa Anda. Solusi ini akan menyelesaikan masalah sebagian besar.
- Jika masalah masih belum diatasi, gunakan modul [PowerShell Exchange Online v2,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)yang menyertakan CMDlets yang didasarkan pada REST API dan secara signifikan lebih banyak melakukan. Ini dapat menjadi solusi yang baik untuk banyak Get- CMDlet yang sering digunakan.
- Jika anda perlu menggunakan CMDlets yang tidak tercakup dalam modul v2, silakan lihat Menjalankan [cmdlet PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)untuk sejumlah besar pengguna di Office 365 , yang membahas tentang cara mengelilingi batas pembatasan PowerShell di Exchange Online.
