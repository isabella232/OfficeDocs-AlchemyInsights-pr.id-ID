---
title: Penundaan atau pembatasan mikro di Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947910"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Penundaan atau pembatasan mikro di Exchange Online PowerShell

Anda mungkin melihat peringatan "Keterlambatan mikro diterapkan" atau keterlambatan ketika menjalankan skrip dan cmdlet di Exchange Online. Berikut ini adalah dua saran terkait hal ini:

- Anda mungkin ingin menggunakan [modul Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), yang menyertakan CMDlet yang berdasarkan REST API dan secara signifikan lebih berkinerja. Ini dapat menjadi solusi yang baik untuk banyak Get- CMDlet yang sering digunakan.
- Jika Anda perlu menggunakan CMDlet yang belum tercakup dalam modul v2, lihat [Menjalankan cmdlet PowerShell untuk banyak pengguna di Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), yang membahas tentang cara mengatur batas pembatasan PowerShell di Exchange Online.
