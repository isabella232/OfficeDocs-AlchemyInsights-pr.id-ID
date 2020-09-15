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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="8ceac-102">Sertifikat Federasi ADFS kedaluwarsa</span><span class="sxs-lookup"><span data-stu-id="8ceac-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="8ceac-103">Untuk mengatasi masalah ini, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="8ceac-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="8ceac-104">Instal modul Microsoft Azure Active Directory untuk Windows PowerShell di komputer (jika modul belum terinstal).</span><span class="sxs-lookup"><span data-stu-id="8ceac-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="8ceac-105">Untuk melakukan ini, masuk ke [Kelola AZURE AD menggunakan Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="8ceac-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="8ceac-106">Ikuti langkah-langkah dalam "skenario 1: sertifikat penandatanganan token AD FS kedaluwarsa" dari ["ada masalah saat mengakses situs" dari AD FS ketika pengguna gabungan masuk ke Microsoft 365, Azure, atau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="8ceac-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="8ceac-107">Ikuti langkah-langkah dalam [memperbarui atau memperbaiki pengaturan domain gabungan di Microsoft, Azure, atau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="8ceac-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="8ceac-108">Untuk mempelajari selengkapnya tentang memperpanjang sertifikat Federasi, lihat [memperpanjang sertifikat Federasi untuk Microsoft 365 dan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="8ceac-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
