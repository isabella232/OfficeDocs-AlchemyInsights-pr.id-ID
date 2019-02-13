---
title: Kesalahan AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916527"
---
# <a name="error-attributevaluemustbeunique"></a>Kesalahan: AttributeValueMustBeUnique

Alasan yang paling umum untuk kesalahan AttributeValueMustBeUnique adalah dua objek dengan berbeda SourceAnchor (immutableId) memiliki nilai yang sama untuk atribut ProxyAddresses dan/atau UserPrincipalName. Untuk memperbaiki kesalahan AttributeValueMustBeUnique:
  
1. Mengidentifikasi proxyAddresses diduplikasi, userPrincipalName atau nilai atribut lainnya yang menyebabkan kesalahan. Juga mengidentifikasi yang dua (atau lebih) objek yang terlibat dalam konflik. Laporan yang dihasilkan oleh kesehatan Azure iklan menyambung sinkronisasi dapat membantu Anda mengidentifikasi dua objek.
    
2. Mengidentifikasi objek yang harus terus memiliki nilai digandakan dan objek yang tidak perlu.
    
3. Menghapus nilai digandakan dari objek yang seharusnya tidak memiliki nilai. Perhatikan bahwa Anda harus membuat perubahan dalam direktori mana objek bersumber dari. Dalam beberapa kasus, Anda mungkin perlu menghapus salah satu objek dalam konflik.
    
4. Jika Anda membuat perubahan lokal di AD, biarkan Azure iklan menyambung sinkronisasi perubahan atas kesalahan untuk mendapatkan tetap.
    

