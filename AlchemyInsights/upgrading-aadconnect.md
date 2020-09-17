---
title: 932 memutakhirkan AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806042"
---
# <a name="upgrade-azure-ad-connect"></a>Memutakhirkan Azure AD Connect

Secara default, pemutakhiran otomatis diaktifkan untuk Azure AD Connect, yang membantu memastikan Anda menjalankan versi terbaru. Untuk memverifikasi pengaturan pemutakhiran otomatis, gunakan cmdlet **Get-ADSyncAutoUpgrade** di Azure AD PowerShell. Cmdlet akan mengembalikan salah satu nilai berikut:

- **Diaktifkan**: pemutakhiran otomatis diaktifkan.

- **Dinonaktifkan**: pemutakhiran otomatis dinonaktifkan.

- **Ditangguhkan**: sistem tidak lagi memenuhi syarat untuk menerima Pemutakhiran otomatis. Anda tidak bisa mengonfigurasi nilai ini; ini diatur oleh sistem.

Untuk informasi selengkapnya, lihat [pemutakhiran otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Untuk mengunduh versi terbaru Azure AD Connect, masuk ke [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
