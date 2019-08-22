---
title: 932 upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506086"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade iklan Azure terhubung

Secara default, upgrade otomatis diaktifkan untuk Azure iklan Connect, yang membantu untuk memastikan Anda sedang menjalankan versi terbaru. Untuk memverifikasi pengaturan upgrade otomatis, gunakan cmdlet **Get-ADSyncAutoUpgrade** di Azure iklan PowerShell. Cmdlet akan kembali salah satu nilai berikut:

- **Diaktifkan**: upgrade otomatis diaktifkan.

- **Dinonaktifkan**: upgrade otomatis dinonaktifkan.

- **Suspended**: sistem ini tidak lagi memenuhi syarat untuk menerima upgrade otomatis. Anda tidak dapat mengkonfigurasi nilai ini; diatur oleh sistem.

Untuk informasi lebih lanjut, lihat [upgrade otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Untuk men-download versi terbaru dari Azure iklan terhubung, pergi ke [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
