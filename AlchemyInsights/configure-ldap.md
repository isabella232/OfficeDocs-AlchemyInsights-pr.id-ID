---
title: Mengonfigurasi LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885163"
---
# <a name="configure-ldap"></a><span data-ttu-id="511a3-102">Mengonfigurasi LDAP</span><span class="sxs-lookup"><span data-stu-id="511a3-102">Configure LDAP</span></span>

<span data-ttu-id="511a3-103">Untuk mengonfigurasi LDAP, lakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="511a3-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="511a3-104">Periksa kesehatan domain Anda di [portal Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="511a3-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="511a3-105">Pastikan langganan Azure AD yang valid tersedia dan layanan domain AD Azure telah diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="511a3-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="511a3-106">Sertifikat yang diperlukan untuk mengaktifkan LDAP aman harus diperoleh dari otoritas sertifikasi publik tepercaya atau sertifikat yang ditandatangani sendiri.</span><span class="sxs-lookup"><span data-stu-id="511a3-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="511a3-107">Pastikan sertifikat mengikuti [panduan](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)yang diperlukan.</span><span class="sxs-lookup"><span data-stu-id="511a3-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="511a3-108">**Sertifikat tidak valid**</span><span class="sxs-lookup"><span data-stu-id="511a3-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="511a3-109">Untuk memperpanjang sertifikat, ikuti langkah-langkah untuk membuat sertifikat baru dan mengunggah ulang: [MENGONFIGURASI LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="511a3-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="511a3-110">Untuk mengatasi masalah umum dengan peringatan LDAP aman dalam layanan domain Azure Active Directory, lihat [mengatasi pemberitahuan LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="511a3-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>