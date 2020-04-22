---
title: Sertifikat Federasi ADFS kedaluwarsa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710410"
---
# <a name="adfs-federation-certificate-expiring"></a>Sertifikat Federasi ADFS kedaluwarsa

Untuk mengatasi masalah ini, ikuti langkah berikut:
  
1. Instal Microsoft Azure Active Directory modul untuk Windows PowerShell di komputer (jika modul belum diinstal). Untuk melakukannya, buka [Kelola AZURE AD menggunakan Windows PowerShell](https://aka.ms/aadposh).

2. Ikuti langkah di "skenario 1: AD FS penandatanganan token sertifikat kedaluwarsa" bagian ["ada masalah mengakses situs" galat dari AD FS ketika pengguna gabungan masuk ke Microsoft 365, Azure, atau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Ikuti langkah di [memperbarui atau memperbaiki pengaturan domain gabungan di Microsoft, Azure, atau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Untuk mempelajari selengkapnya tentang memperbarui sertifikat Federasi, lihat [memperbarui sertifikat Federasi untuk Microsoft 365 dan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
