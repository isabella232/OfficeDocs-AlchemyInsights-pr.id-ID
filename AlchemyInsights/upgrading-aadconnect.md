---
title: 932 upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389696"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade iklan Azure terhubung

Secara default, upgrade otomatis diaktifkan untuk Azure iklan Connect, yang membantu untuk memastikan Anda sedang menjalankan versi terbaru. Untuk memverifikasi pengaturan upgrade otomatis, gunakan cmdlet **Get-ADSyncAutoUpgrade** di Azure iklan PowerShell. Cmdlet akan kembali salah satu nilai berikut: 

- **Diaktifkan**: upgrade otomatis diaktifkan.

- **Dinonaktifkan**: upgrade otomatis dinonaktifkan.

- **Suspended**: sistem ini tidak lagi memenuhi syarat untuk menerima upgrade otomatis. Anda tidak dapat mengkonfigurasi nilai ini; diatur oleh sistem. 

Untuk informasi lebih lanjut, lihat [upgrade otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Untuk men-download versi terbaru dari Azure iklan terhubung, pergi ke [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
