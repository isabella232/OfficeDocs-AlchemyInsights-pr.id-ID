---
title: Galat AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703177"
---
# <a name="error-attributevaluemustbeunique"></a>Galat: AttributeValueMustBeUnique

Alasan paling umum untuk galat AttributeValueMustBeUnique adalah dua objek dengan SourceAnchor berbeda (immutableId) memiliki nilai yang sama untuk atribut ProxyAddresses dan/atau UserPrincipalName. Untuk memperbaiki galat AttributeValueMustBeUnique:
  
1. Identifikasi proxyAddresses duplikat, userPrincipalName atau nilai atribut lain yang menyebabkan galat. Juga mengidentifikasi dua (atau lebih) objek yang terlibat dalam konflik. Laporan yang dihasilkan oleh Azure AD menyambung kesehatan untuk sinkronisasi dapat membantu Anda mengidentifikasi dua objek.
    
2. Mengidentifikasi objek yang harus terus memiliki nilai duplikat dan objek yang seharusnya tidak.
    
3. Hapus nilai duplikat dari objek yang seharusnya tidak memiliki nilai tersebut. Perhatikan bahwa Anda harus membuat perubahan dalam direktori tempat objek bersumber dari. Dalam beberapa kasus, Anda mungkin perlu menghapus salah satu objek dalam konflik.
    
4. Jika Anda membuat perubahan di lokal AD, biarkan Azure AD menyambung menyinkronkan perubahan kesalahan untuk mendapatkan diperbaiki.
    

