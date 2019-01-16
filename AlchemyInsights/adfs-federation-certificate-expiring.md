---
title: Federasi ADFS sertifikat kedaluwarsa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294845"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="c02a5-102">Federasi ADFS sertifikat kedaluwarsa</span><span class="sxs-lookup"><span data-stu-id="c02a5-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="c02a5-103">Untuk mengatasi masalah ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="c02a5-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="c02a5-p101">Menginstal Microsoft Azure aktif direktori modul untuk Windows PowerShell di komputer (jika tidak menginstal modul). Untuk melakukan ini, pergi ke [Manage Azure iklan menggunakan Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="c02a5-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="c02a5-106">Ikuti langkah-langkah dalam "skenario 1: AD FS token-penandatanganan sertifikat kadaluarsa" bagian ["Ada masalah mengakses situs" kesalahan dari AD FS ketika pengguna Federasi masuk ke kantor 365, Azure, atau Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="c02a5-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="c02a5-107">Ikuti langkah-langkah bagaimana [untuk memperbarui atau memperbaiki pengaturan domain federasi di Office 365, Azure, atau Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="c02a5-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="c02a5-108">Untuk mempelajari lebih lanjut tentang memperbarui sertifikat Federasi, lihat [Renew Federasi sertifikat untuk Office 365 dan Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="c02a5-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

