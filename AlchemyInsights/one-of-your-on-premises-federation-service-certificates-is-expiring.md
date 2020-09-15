---
title: Salah satu sertifikat Layanan Federasi lokal Anda akan kedaluwarsa
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673500"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="de84b-102">Salah satu sertifikat Layanan Federasi lokal Anda akan kedaluwarsa</span><span class="sxs-lookup"><span data-stu-id="de84b-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="de84b-103">Untuk mengatasi masalah ini, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="de84b-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="de84b-104">Instal modul Microsoft Azure Active Directory untuk Windows PowerShell di komputer (jika modul belum terinstal).</span><span class="sxs-lookup"><span data-stu-id="de84b-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="de84b-105">Untuk melakukan ini, masuk ke [PowerShell direktori aktif Azure untuk graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="de84b-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="de84b-106">Ikuti langkah-langkah dalam "skenario 1: sertifikat penandatanganan token AD FS kedaluwarsa" dari ["ada masalah saat mengakses situs" dari AD FS ketika pengguna gabungan masuk ke Microsoft 365, Azure, atau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="de84b-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="de84b-107">Ikuti langkah-langkah dalam [cara memperbarui atau memperbaiki pengaturan domain gabungan di Microsoft 365, Azure, atau Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="de84b-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="de84b-108">Untuk informasi selengkapnya tentang sertifikat Federasi yang diperpanjang, lihat [pembaruan sertifikat untuk O365 dan AZURE AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="de84b-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

