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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504997"
---
# <a name="conditional-access-with-intune"></a>Akses bersyarat dengan Intune

Menggunakan **Akses bersyarat** dengan Intune membutuhkan 3 langkah: 
  
- Membuat **Kebijakan akses bersyarat** yang mendefinisikan apa yang sumber daya yang dilindungi, dan kondisi apa yang harus dipenuhi untuk mengakses sumber daya tersebut. Sebagai contoh, perangkat harus memenuhi persyaratan sebelum mengakses email perusahaan. 
    
- Membuat **Kebijakan kepatuhan** untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai. Sebagai contoh, perangkat harus memiliki setidaknya 6 digit pin sebelum itu dianggap sesuai. 
    
- Memastikan **Kepatuhan kebijakan** dan **Kebijakan akses bersyarat** ditargetkan untuk kelompok pengguna yang diinginkan. Ini mungkin membutuhkan menciptakan grup pengguna tertentu di Azure Active Directory. 
    
Baca lebih lanjut:
  
- [Akses bersyarat praktik terbaik](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Memulai dengan akses bersyarat](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

