---
title: Kesalahan AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709154"
---
# <a name="error-attributevaluemustbeunique"></a>Kesalahan: AttributeValueMustBeUnique

Alasan paling umum untuk kesalahan AttributeValueMustBeUnique adalah dua objek dengan SourceAnchor yang berbeda (immutableId) memiliki nilai yang sama untuk atribut ProxyAddresses dan/atau UserPrincipalName. Untuk memperbaiki kesalahan AttributeValueMustBeUnique:
  
1. Identifikasi duplikat proxyAddresses, userPrincipalName atau nilai atribut lainnya yang menyebabkan kesalahan. Juga mengidentifikasi dua objek yang terlibat dalam konflik. Laporan yang dihasilkan oleh kesehatan Azure AD Connect untuk sinkronisasi dapat membantu Anda mengidentifikasi dua objek.
    
2. Mengidentifikasi objek yang akan terus memiliki nilai duplikat dan objek yang seharusnya tidak.
    
3. Hapus nilai duplikat dari objek yang seharusnya tidak memiliki nilai tersebut. Perhatikan bahwa Anda harus membuat perubahan di direktori tempat objek berasal. Dalam beberapa kasus, Anda mungkin perlu menghapus salah satu objek dalam konflik.
    
4. Jika Anda membuat perubahan di iklan lokal, biarkan Azure AD Connect menyinkronkan perubahan untuk kesalahan tersebut untuk diperbaiki.
    

