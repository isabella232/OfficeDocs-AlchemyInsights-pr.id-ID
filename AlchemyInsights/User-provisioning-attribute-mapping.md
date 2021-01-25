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
# <a name="user-provisioning-attribute-mapping"></a>Pemetaan atribut penyediaan pengguna

1. Untuk memecahkan masalah masalah pemetaan-atribut yang diketahui, lihat [pemetaan atribut](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) menyediakan dukungan untuk penyediaan pengguna ke aplikasi SaaS pihak ketiga seperti Salesforce, G suite dan lainnya. Jika Anda mengaktifkan penyediaan pengguna untuk aplikasi SaaS pihak ketiga, portal Azure mengontrol nilai atributnya melalui pemetaan atribut. Untuk mempelajari cara mengustomisasi pemetaan atribut default, lihat [mengkustomisasi atribut provisioning pengguna-pemetaan untuk aplikasi SaaS di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Untuk mempelajari selengkapnya tentang provisioning pengguna aplikasi SaaS, lihat [apa itu provisioning pengguna aplikasi SaaS otomatis di AZURE AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Saat mengkustomisasi pemetaan atribut untuk penyediaan pengguna, Anda mungkin menemukan bahwa atribut yang ingin Anda Petakan tidak muncul dalam daftar atribut sumber. [Sinkronisasi atribut dari direktori aktif di tempat Anda ke AZURE AD untuk penyediaan artikel aplikasi](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) memperlihatkan kepada Anda cara menambahkan atribut yang hilang dengan menyinkronkannya dari AD lokal ke Azure AD.
