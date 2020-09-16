---
title: Perilaku konsistensi GUID/sourceAnchor
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756286"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Perilaku konsistensi GUID/sourceAnchor

Azure AD Connect (versi 1.1.524.0 dan setelahnya) kini memfasilitasi penggunaan msDS-Konsistencyguid sebagai atribut sourceAnchor. Saat menggunakan fitur ini, Azure AD Connect mengonfigurasi aturan sinkronisasi secara otomatis untuk:
  
- Gunakan msDS-Konsistencyguid sebagai atribut sourceAnchor untuk objek pengguna. ObjectGUID digunakan untuk tipe objek lainnya.
    
- Untuk objek pengguna AD lokal yang diberikan yang msDS-Konsistencyguid atribut tidak terisi, Azure AD Connect menulis nilai objectGUID kembali ke atribut msDS-Konsistencyguid dalam direktori aktif di tempat. Setelah atribut msDS-Konsistencyguid diisi, maka Azure AD Connect lalu mengekspor objek ke Azure AD.
    
 **Catatan:** Setelah objek AD di tempat diimpor ke Azure AD Connect (yang diimpor ke dalam ruang konektor AD dan diproyeksikan ke dalam metaverse), Anda tidak bisa mengubah nilai penghitungnya lagi. Untuk menentukan nilai sourceAnchor untuk objek AD di tempat yang diberikan, konfigurasikan atribut msDS-Konsistencyguid sebelum diimpor ke Azure AD Connect. 
  
Untuk informasi selengkapnya tentang SourceAnchor dan Konsistencyguid, lihat yang berikut ini: [AZURE AD Connect: konsep desain](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

