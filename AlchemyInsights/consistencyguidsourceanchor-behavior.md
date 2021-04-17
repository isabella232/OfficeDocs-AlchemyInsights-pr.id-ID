---
title: Perilaku ConsistencyGuid / sourceAnchor
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816995"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Perilaku ConsistencyGuid / sourceAnchor

Azure AD Connect (versi 1.1.524.0 dan setelahnya) kini memfasilitasi penggunaan atribut msDS-ConsistencyGuid sebagai atribut sourceAnchor. Ketika menggunakan fitur ini, Azure AD Connect secara otomatis mengonfigurasi aturan sinkronisasi untuk:
  
- Gunakan msDS-ConsistencyGuid sebagai atribut sourceAnchor untuk objek Pengguna. ObjectGUID digunakan untuk tipe objek lain.
    
- Untuk objek Pengguna AD lokal dengan atribut msDS-ConsistencyGuid yang tidak diisi, Azure AD Connect akan menulis nilai objectGUID kembali ke atribut msDS-ConsistencyGuid di Direktori Aktif lokal. Setelah atribut msDS-ConsistencyGuid terisi, Azure AD Connect kemudian mengekspor objek ke Azure AD.
    
 **Catatan:** Setelah objek AD lokal diimpor ke Azure AD Connect (yang diimpor ke Ruang Konektor AD dan diproyeksikan ke Metaverse), Anda tidak dapat mengubah nilai sumbernya lagi. Untuk menentukan nilai sourceAnchor bagi objek AD lokal tertentu, konfigurasi atribut msDS-ConsistencyGuid sebelum diimpor ke Azure AD Connect. 
  
Untuk informasi selengkapnya tentang SourceAnchor dan ConsistencyGuid, lihat hal berikut: [Azure AD Connect: Konsep desain](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

