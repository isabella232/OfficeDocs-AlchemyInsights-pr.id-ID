---
title: Kesalahan AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813763"
---
# <a name="error-attributevaluemustbeunique"></a>Kesalahan: AttributeValueMustBeUnique

Alasan paling umum untuk kesalahan AttributeValueMustBeUnique adalah dua objek dengan atribut SourceAnchor (immutableId) yang berbeda memiliki nilai yang sama untuk atribut ProxyAddresses dan/atau UserPrincipalName. Untuk memperbaiki kesalahan AttributeValueMustBeUnique:
  
1. Identifikasi nilai atribut proxyAddresses, userPrincipalName, atau nilai atribut lainnya yang menyebabkan kesalahan. Juga mengidentifikasi dua (atau beberapa) objek mana yang dilibatkan dalam konflik tersebut. Laporan yang dihasilkan oleh Azure AD Connect Health untuk sinkronisasi dapat membantu Anda mengidentifikasi kedua objek tersebut.
    
2. Identifikasi objek mana yang harus terus mendapatkan nilai duplikat dan objek mana yang tidak boleh.
    
3. Hapus nilai duplikat dari objek yang seharusnya NOT memiliki nilai tersebut. Perhatikan bahwa Anda harus membuat perubahan dalam direktori tempat objek berasal. Dalam beberapa kasus, Anda mungkin perlu menghapus salah satu objek yang berkonflik.
    
4. Jika Anda membuat perubahan di AD lokal, biarkan Azure AD Connect menyinkronkan perubahan agar kesalahan berhasil diperbaiki.
    

