---
title: Menghapus saluran pribadi teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439325"
---
# <a name="delete-a-teams-private-channel"></a>Menghapus saluran pribadi teams

Microsoft telah mengetahui masalah menghapus teams saluran pribadi jika Anda memiliki kebijakan retensi SharePoint diaktifkan untuk situs SharePoint dasar. Microsoft bekerja pada perbaikan. Sementara itu, Anda dapat menggunakan penyelesaian masalah berikut untuk menghapus saluran pribadi.

**Mengecualikan koleksi tim situs dari kebijakan retensi SharePoint.**

1. Buka portal admin Office 365, dan pilih **Tampilkan semua** di panel navigasi kiri.
2. Di **Pusat admin**, buka kebijakan **Security & Compliance**  >  **pencegahan kehilangan data**kepatuhan & keamanan  >  **Policy**.
3. Mengidentifikasi kebijakan yang berlaku untuk situs SharePoint, dan mengubah kebijakan sehingga situs SharePoint untuk tim yang berisi saluran pribadi tidak disertakan dalam kebijakan retensi.
4. Simpan kebijakan.
    Diperlukan waktu hingga 24 jam agar pengaturan kebijakan diterapkan.
    Setelah situs dikecualikan, Anda dapat menghapus saluran pribadi.  
    
Anda ***mungkin*** dapat menghapus saluran pribadi dengan menggunakan Microsoft teams di perangkat Android. 

Untuk informasi terkait SharePoint, lihat [tidak dapat menghapus item di SharePoint online atau OneDrive untuk bisnis](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).