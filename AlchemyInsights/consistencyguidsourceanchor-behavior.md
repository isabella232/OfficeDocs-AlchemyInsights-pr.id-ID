---
title: Perilaku konsistensi Encyguid/sourceAnchor
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705736"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Perilaku konsistensi Encyguid/sourceAnchor

Azure AD menyambung (versi 1.1.524.0 dan setelah) sekarang memfasilitasi penggunaan msDS-konsistensi Encyguid sebagai sourceAnchor atribut. Saat menggunakan fitur ini, Azure AD menyambung secara otomatis mengkonfigurasi aturan sinkronisasi untuk:
  
- Gunakan msDS-konsistensi Encyguid sebagai sourceAnchor atribut untuk objek pengguna. ObjectGUID digunakan untuk jenis objek lainnya.
    
- Untuk setiap objek pengguna AD lokal yang atribut msDS-Konsistencyguid tidak diisi, Azure AD menyambung menulis objectGUID nilai kembali ke atribut msDS-Konsistencyguid di direktori aktif di tempat. Setelah atribut msDS-Konsistencyguid diisi, Azure AD menyambung kemudian ekspor objek ke Azure AD.
    
 **Catatan:** Setelah objek AD lokal diimpor ke Azure AD menyambung (yaitu, diimpor ke Ruang konektor AD dan diproyeksikan ke metaverse), Anda tidak dapat mengubah nilai sourceAnchor lagi. Untuk menentukan nilai sourceAnchor untuk objek AD lokal tertentu, konfigurasikan atribut msDS-konsistensi Encyguid sebelum diimpor ke Azure AD menyambung. 
  
Untuk informasi lebih lanjut tentang SourceAnchor dan konsistensi Encyguid, lihat berikut ini: [AZURE AD menyambung: konsep desain](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

