---
title: Pemantauan akses bersyarat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713721"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Pemantauan akses bersyarat untuk Exchange

Pengguna yang ditargetkan dengan akses bersyarat akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk menyelesaikan, kami merekomendasikan satu atau lebih solusi berikut:
  
- Jika perangkat diduga terdaftar, menyarankan pengguna untuk pergi ke aplikasi portal perusahaan dan verifikasi bahwa ditampilkan di portal perusahaan. Jika tidak, pengguna harus mendaftarkan perangkat.
    
- Di portal Azure pergi ke ** \> Intune kepatuhan perangkat**. Di bawah **monitor** , klik **perangkat kepatuhan**. Lihat laporan kepatuhan perangkat untuk memverifikasi bahwa perangkat pengguna ditandai sebagai sesuai. 
    
- Di portal Azure pergi ke ** \> Intune kepatuhan perangkat**. Di bawah **Kelola**, klik **kebijakan**. Dalam daftar kebijakan kepatuhan, Verifikasikan bahwa profil ditetapkan ke perangkat pengguna Anda. Jika tidak ada profil yang ditetapkan, maka Intune tidak akan dapat mengkonfirmasi status kepatuhan perangkat. 
    
- Mengedit penetapan akses bersyarat pengguna.
    
1. Di portal Azure pergi ke **Intune \> kebijakan akses \> bersyarat**
    
2. Pilih kebijakan dari daftar
    
3. Klik **pengguna dan grup**
    
4. Untuk menargetkan kebijakan tertentu pada seseorang, menambahkannya ke daftar **sertakan** . Untuk memastikan seseorang diabaikan dari kebijakan, tambahkan ke daftar **Kecualikan** . 
    
Baca lebih lanjut: [Bagaimana memonitor perangkat akses bersyarat](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

