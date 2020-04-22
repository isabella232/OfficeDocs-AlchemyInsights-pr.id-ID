---
title: Akses bersyarat dengan Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706024"
---
# <a name="conditional-access-with-intune"></a>Akses bersyarat dengan Intune

Menggunakan **akses bersyarat** dengan Intune memerlukan 3 langkah: 
  
- Buat **kebijakan akses bersyarat** yang menentukan sumber daya apa yang dilindungi, dan kondisi apa yang perlu dipenuhi untuk mengakses sumber daya tersebut. Misalnya, perangkat harus kompatibel sebelum mengakses email perusahaan. 
    
- Buat **kebijakan kepatuhan** untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai. Misalnya, perangkat harus memiliki PIN minimal 6 digit sebelum dianggap sesuai. 
    
- Memastikan **kebijakan kepatuhan** dan **kebijakan akses bersyarat** ditargetkan ke grup pengguna yang diinginkan. Ini mungkin memerlukan membuat grup pengguna tertentu di Azure Active Directory. 
    
Selengkapnya:
  
- [Praktik terbaik akses bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Memulai dengan akses bersyarat](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

