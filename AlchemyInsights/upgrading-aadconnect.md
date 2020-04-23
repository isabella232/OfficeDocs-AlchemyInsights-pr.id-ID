---
title: 932 upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766496"
---
# <a name="upgrade-azure-ad-connect"></a>Meningkatkan Azure AD menyambung

Secara default, upgrade otomatis diaktifkan untuk Azure AD menyambung, yang membantu untuk memastikan bahwa Anda menjalankan versi terbaru. Untuk memverifikasi pengaturan upgrade otomatis, gunakan cmdlet **Get-ADSyncAutoUpgrade** di Azure AD PowerShell. Cmdlet akan mengembalikan salah satu nilai berikut:

- **Enabled**: upgrade otomatis diaktifkan.

- **Nonaktif**: peningkatan otomatis dinonaktifkan.

- **Ditangguhkan**: sistem tidak lagi memenuhi syarat untuk menerima upgrade otomatis. Anda tidak dapat mengkonfigurasi nilai ini; itu diatur oleh sistem.

Untuk informasi lebih lanjut, lihat [upgrade otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Untuk mengunduh versi terbaru Azure AD menyambung, kunjungi [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
