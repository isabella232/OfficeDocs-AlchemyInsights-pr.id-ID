---
title: Memantau akses bersyarat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702906"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Memantau akses bersyarat untuk Exchange

Pengguna yang ditargetkan dengan akses bersyarat akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk mengatasinya, kami menyarankan satu atau beberapa solusi berikut:
  
- Jika perangkat dianggap terdaftar, Anjurkan pengguna untuk masuk ke aplikasi portal perusahaan dan memverifikasi bahwa perangkat tersebut muncul di portal perusahaan. Jika tidak, pengguna harus mendaftarkan perangkat.
    
- Di portal Azure, masuk ke **Intune \> Device Compliance**. Di bawah **monitor** klik **kepatuhan perangkat**. Tampilkan Laporan kepatuhan perangkat Anda untuk memverifikasi bahwa perangkat pengguna ditandai sebagai sesuai. 
    
- Di portal Azure, masuk ke **Intune \> Device Compliance**. Di bawah **Kelola**, klik **kebijakan**. Dalam daftar kebijakan kepatuhan, verifikasi bahwa profil ditetapkan untuk perangkat pengguna Anda. Jika tidak ada profil yang ditetapkan, maka Intune tidak akan dapat mengonfirmasi status kepatuhan perangkat. 
    
- Mengedit penetapan akses bersyarat pengguna.
    
1. Di Azure portal masuk ke ** \> \> kebijakan akses bersyarat Intune**
    
2. Memilih kebijakan dari daftar
    
3. Klik **pengguna dan grup**
    
4. Untuk menargetkan kebijakan tertentu pada seseorang, tambahkan ke daftar **sertakan** . Untuk memastikan bahwa seseorang dihilangkan dari kebijakan, tambahkan ke daftar **Kecualikan** . 
    
Baca selengkapnya: [cara memantau perangkat akses bersyarat](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

