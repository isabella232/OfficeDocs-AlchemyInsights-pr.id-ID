---
title: Sertifikat Federasi ADFS kedaluwarsa
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952972"
---
# <a name="adfs-federation-certificate-expiring"></a>Sertifikat Federasi ADFS kedaluwarsa

Untuk mengatasi masalah ini, ikuti langkah-langkah berikut:
  
1. Instal Microsoft Azure Active Directory Module untuk Windows PowerShell di komputer (jika modul belum diinstal). Untuk melakukannya, buka [Mengelola Azure AD menggunakan Windows PowerShell](https://aka.ms/aadposh).

2. Ikuti langkah-langkah dalam bagian "Skenario 1: Sertifikat token AD FS kedaluwarsa" dari bagian "Terdapat masalah dalam mengakses situs" dari AD FS ketika pengguna gabungan masuk ke [Microsoft 365, Azure, atau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Ikuti langkah-langkah [dalam Memperbarui atau memperbaiki pengaturan domain gabungan di Microsoft, Azure, atau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Untuk mempelajari selengkapnya tentang memperpanjang sertifikat Federasi, lihat [Memperpanjang sertifikat federasi untuk Microsoft 365 dan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
