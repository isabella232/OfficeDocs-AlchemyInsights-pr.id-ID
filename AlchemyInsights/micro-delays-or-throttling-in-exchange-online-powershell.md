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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314703"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Penundaan atau pembatasan mikro di Exchange Online PowerShell

Anda mungkin melihat peringatan "Keterlambatan mikro diterapkan" atau keterlambatan ketika menjalankan skrip dan cmdlet di Exchange Online. Berikut beberapa saran untuk mengatasi masalah ini:

- Jalankan diagnostik kami untuk relaksasi kebijakan pembatasan PowerShell penyewa Anda. Solusi ini akan menyelesaikan masalah sebagian besar.
- Jika masalah masih belum diatasi, gunakan modul [PowerShell Exchange Online v2,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)yang menyertakan CMDlets yang didasarkan pada API REST dan secara signifikan lebih sering digunakan. Ini dapat menjadi solusi yang baik untuk banyak Get- CMDlet yang sering digunakan.
- Jika anda perlu menggunakan CMDlets yang tidak tercakup dalam modul v2, silakan lihat Menjalankan [cmdlet PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)untuk sejumlah besar pengguna di Office 365 , yang membahas tentang cara mengelilingi batas pembatasan PowerShell di Exchange Online.
