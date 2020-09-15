---
title: Sertifikat Federasi ADFS kedaluwarsa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686717"
---
# <a name="adfs-federation-certificate-expiring"></a>Sertifikat Federasi ADFS kedaluwarsa

Untuk mengatasi masalah ini, ikuti langkah-langkah berikut:
  
1. Instal modul Microsoft Azure Active Directory untuk Windows PowerShell di komputer (jika modul belum terinstal). Untuk melakukan ini, masuk ke [Kelola AZURE AD menggunakan Windows PowerShell](https://aka.ms/aadposh).

2. Ikuti langkah-langkah dalam "skenario 1: sertifikat penandatanganan token AD FS kedaluwarsa" dari ["ada masalah saat mengakses situs" dari AD FS ketika pengguna gabungan masuk ke Microsoft 365, Azure, atau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Ikuti langkah-langkah dalam [memperbarui atau memperbaiki pengaturan domain gabungan di Microsoft, Azure, atau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Untuk mempelajari selengkapnya tentang memperpanjang sertifikat Federasi, lihat [memperpanjang sertifikat Federasi untuk Microsoft 365 dan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
