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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044343"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Perilaku ConsistencyGuid / sourceAnchor

Azure AD Koneksi (versi 1.1.524.0 dan setelahnya) kini memfasilitasi penggunaan atribut msDS-ConsistencyGuid sebagai atribut sourceAnchor. Ketika menggunakan fitur ini, Azure AD Koneksi secara otomatis mengonfigurasi aturan sinkronisasi untuk:
  
- Gunakan msDS-ConsistencyGuid sebagai atribut sourceAnchor untuk objek Pengguna. ObjectGUID digunakan untuk tipe objek lain.
    
- Untuk objek Pengguna AD lokal dengan atribut msDS-ConsistencyGuid yang tidak diisi, Azure AD Koneksi akan menulis nilai objectGUID kembali ke atribut msDS-ConsistencyGuid di Direktori Aktif lokal. Setelah atribut msDS-ConsistencyGuid terisi, Azure AD Koneksi lalu mengekspor objek ke Azure AD.
    
 **Catatan:** Setelah objek AD lokal diimpor ke Azure AD Koneksi (dan diimpor ke Ruang Konektor AD dan diproyeksikan ke Metaverse), Anda tidak dapat mengubah nilai sumbernya lagi. Untuk menentukan nilai sourceAnchor bagi objek AD lokal tertentu, konfigurasi atribut msDS-ConsistencyGuid sebelum diimpor ke Azure AD Koneksi. 
  
Untuk informasi selengkapnya tentang SourceAnchor dan ConsistencyGuid, lihat bagian berikut: [Azure AD Koneksi: Konsep desain](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

