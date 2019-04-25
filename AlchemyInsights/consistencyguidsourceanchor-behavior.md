---
title: ConsistencyGuid / sourceAnchor perilaku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408111"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor perilaku

Azure iklan Connect (versi 1.1.524.0 dan setelah) sekarang memfasilitasi penggunaan msDS-ConsistencyGuid sebagai atribut sourceAnchor. Bila menggunakan fitur ini, Azure iklan terhubung secara otomatis mengkonfigurasi aturan sinkronisasi untuk:
  
- Menggunakan msDS-ConsistencyGuid sebagai atribut sourceAnchor untuk objek pengguna. ObjectGUID digunakan untuk jenis objek lain.
    
- Untuk setiap lokal pengguna AD objek yang msDS-ConsistencyGuid atribut tidak dihuni, Azure iklan menghubungkan menulis nilainya objectGUID kembali ke atribut msDS-ConsistencyGuid di Active Directory lokal. Setelah atribut msDS-ConsistencyGuid diisi, kemudian Azure iklan menghubungkan ekspor objek Azure iklan.
    
 **Catatan:** Sekali lokal iklan objek diimpor ke Azure iklan terhubung (yang diimpor ke Ruang konektor iklan dan diproyeksikan ke Metaverse), Anda tidak dapat mengubah nilai sourceAnchor lagi. Untuk menentukan nilai sourceAnchor untuk diberikan lokal iklan objek, mengkonfigurasi atribut msDS-ConsistencyGuid yang sebelum itu diimpor ke Azure iklan terhubung. 
  
Untuk informasi lebih lanjut di SourceAnchor dan ConsistencyGuid, lihat berikut: [Azure iklan terhubung: Desain konsep](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

