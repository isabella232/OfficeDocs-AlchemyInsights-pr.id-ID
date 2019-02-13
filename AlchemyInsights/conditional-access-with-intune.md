---
title: Akses bersyarat dengan Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935941"
---
# <a name="conditional-access-with-intune"></a>Akses bersyarat dengan Intune

Menggunakan **Akses bersyarat** dengan Intune membutuhkan 3 langkah: 
  
- Membuat **Kebijakan akses bersyarat** yang mendefinisikan apa yang sumber daya yang dilindungi, dan kondisi apa yang harus dipenuhi untuk mengakses sumber daya tersebut. Sebagai contoh, perangkat harus memenuhi persyaratan sebelum mengakses email perusahaan. 
    
- Membuat **Kebijakan kepatuhan** untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai. Sebagai contoh, perangkat harus memiliki setidaknya 6 digit pin sebelum itu dianggap sesuai. 
    
- Memastikan **Kepatuhan kebijakan** dan **Kebijakan akses bersyarat** ditargetkan untuk kelompok pengguna yang diinginkan. Ini mungkin membutuhkan menciptakan grup pengguna tertentu di Azure Active Directory. 
    
Baca lebih lanjut:
  
- [Akses bersyarat praktik terbaik](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Memulai dengan akses bersyarat](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

