---
title: Pemetaan atribut penyediaan pengguna
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949765"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="73777-102">Pemetaan atribut penyediaan pengguna</span><span class="sxs-lookup"><span data-stu-id="73777-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="73777-103">Untuk memecahkan masalah masalah pemetaan-atribut yang diketahui, lihat [pemetaan atribut](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="73777-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="73777-104">Microsoft Azure Active Directory (AD) menyediakan dukungan untuk penyediaan pengguna ke aplikasi SaaS pihak ketiga seperti Salesforce, G suite dan lainnya.</span><span class="sxs-lookup"><span data-stu-id="73777-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="73777-105">Jika Anda mengaktifkan penyediaan pengguna untuk aplikasi SaaS pihak ketiga, portal Azure mengontrol nilai atributnya melalui pemetaan atribut.</span><span class="sxs-lookup"><span data-stu-id="73777-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="73777-106">Untuk mempelajari cara mengustomisasi pemetaan atribut default, lihat [mengkustomisasi atribut provisioning pengguna-pemetaan untuk aplikasi SaaS di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="73777-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="73777-107">Untuk mempelajari selengkapnya tentang provisioning pengguna aplikasi SaaS, lihat [apa itu provisioning pengguna aplikasi SaaS otomatis di AZURE AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="73777-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="73777-108">Saat mengkustomisasi pemetaan atribut untuk penyediaan pengguna, Anda mungkin menemukan bahwa atribut yang ingin Anda Petakan tidak muncul dalam daftar atribut sumber.</span><span class="sxs-lookup"><span data-stu-id="73777-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="73777-109">[Sinkronisasi atribut dari direktori aktif di tempat Anda ke AZURE AD untuk penyediaan artikel aplikasi](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) memperlihatkan kepada Anda cara menambahkan atribut yang hilang dengan menyinkronkannya dari AD lokal ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="73777-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
