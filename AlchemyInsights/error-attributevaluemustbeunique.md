---
title: Kesalahan AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499637"
---
# <a name="error-attributevaluemustbeunique"></a>Kesalahan: AttributeValueMustBeUnique

Alasan yang paling umum untuk kesalahan AttributeValueMustBeUnique adalah dua objek dengan berbeda SourceAnchor (immutableId) memiliki nilai yang sama untuk atribut ProxyAddresses dan/atau UserPrincipalName. Untuk memperbaiki kesalahan AttributeValueMustBeUnique:
  
1. Mengidentifikasi proxyAddresses diduplikasi, userPrincipalName atau nilai atribut lainnya yang menyebabkan kesalahan. Juga mengidentifikasi yang dua (atau lebih) objek yang terlibat dalam konflik. Laporan yang dihasilkan oleh kesehatan Azure iklan menyambung sinkronisasi dapat membantu Anda mengidentifikasi dua objek.
    
2. Mengidentifikasi objek yang harus terus memiliki nilai digandakan dan objek yang tidak perlu.
    
3. Menghapus nilai digandakan dari objek yang seharusnya tidak memiliki nilai. Perhatikan bahwa Anda harus membuat perubahan dalam direktori mana objek bersumber dari. Dalam beberapa kasus, Anda mungkin perlu menghapus salah satu objek dalam konflik.
    
4. Jika Anda membuat perubahan lokal di AD, biarkan Azure iklan menyambung sinkronisasi perubahan atas kesalahan untuk mendapatkan tetap.
    

