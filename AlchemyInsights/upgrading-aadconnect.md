---
title: 932 Memutakhirkan AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104815"
---
# <a name="upgrade-azure-ad-connect"></a>Memutakhirkan Azure AD Koneksi

Secara default, pemutakhiran otomatis diaktifkan untuk Azure AD Koneksi, yang membantu memastikan Anda menjalankan versi terbaru. Untuk memverifikasi pengaturan pemutakhiran otomatis, gunakan cmdlet **Get-ADSyncAutoUpgrade** di PowerShell Azure AD. Cmdlet akan mengembalikan salah satu nilai berikut:

- **Diaktifkan**: Pemutakhiran otomatis diaktifkan.

- **Dinonaktifkan**: Pemutakhiran otomatis dinonaktifkan.

- **Ditangguhkan**: Sistem tidak lagi memenuhi syarat untuk menerima pemutakhiran otomatis. Anda tidak bisa mengonfigurasi nilai ini; diatur oleh sistem.

Untuk informasi selengkapnya, lihat [Pemutakhiran otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Untuk mengunduh versi terbaru Azure AD Koneksi, buka [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
