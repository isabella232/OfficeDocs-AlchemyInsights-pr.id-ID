---
title: Salah satu Sertifikat Federation Service lokal Anda akan kedaluwarsa
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810055"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="42426-102">Salah satu Sertifikat Federation Service lokal Anda akan kedaluwarsa</span><span class="sxs-lookup"><span data-stu-id="42426-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="42426-103">Untuk mengatasi masalah ini, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="42426-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="42426-104">Instal Modul Direktori Aktif Microsoft Azure untuk Windows PowerShell di komputer (jika modul belum diinstal).</span><span class="sxs-lookup"><span data-stu-id="42426-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="42426-105">Untuk melakukan hal ini, masuk [ke PowerShell Azure Active Directory untuk Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="42426-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="42426-106">Ikuti langkah-langkah dalam bagian "Skenario 1: Sertifikat token AD FS kedaluwarsa" dari bagian "Terdapat masalah dalam mengakses situs" dari AD FS ketika pengguna gabungan masuk ke [Microsoft 365, Azure, atau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="42426-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="42426-107">Ikuti langkah-langkah dalam Cara memperbarui atau memperbaiki pengaturan domain gabungan di [Microsoft 365, Azure, atau Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="42426-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="42426-108">Untuk informasi selengkapnya tentang memperpanjang sertifikat Federasi, lihat [Perpanjangan sertifikat untuk O365 dan Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="42426-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

