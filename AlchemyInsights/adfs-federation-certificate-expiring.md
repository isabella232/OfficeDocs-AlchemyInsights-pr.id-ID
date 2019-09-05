---
title: Sertifikat Federasi ADFS kedaluwarsa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737192"
---
# <a name="adfs-federation-certificate-expiring"></a>Sertifikat Federasi ADFS kedaluwarsa

Untuk mengatasi masalah ini, ikuti langkah berikut:
  
1. Instal Microsoft Azure Active Directory modul untuk Windows PowerShell di komputer (jika modul belum diinstal). Untuk melakukannya, buka [Kelola AZURE AD menggunakan Windows PowerShell](https://aka.ms/aadposh).

2. Ikuti langkah di "skenario 1: AD FS penandatanganan token sertifikat kedaluwarsa" bagian ["ada masalah mengakses situs" galat dari AD FS ketika pengguna gabungan masuk ke Office 365, Azure, atau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Ikuti langkah di [memperbarui atau memperbaiki pengaturan domain gabungan di Office 365, Azure, atau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Untuk mempelajari selengkapnya tentang memperbarui sertifikat Federasi, lihat [memperbarui sertifikat Federasi untuk Office 365 dan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
