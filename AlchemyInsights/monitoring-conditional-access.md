---
title: Pemantauan akses bersyarat
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295601"
---
# <a name="monitoring-conditional-access"></a>Pemantauan akses bersyarat

Pengguna dengan akses bersyarat yang ditargetkan akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk menyelesaikan, kami merekomendasikan satu atau lebih solusi berikut:
  
- Jika perangkat dianggap diterima, menyarankan pengguna untuk pergi ke app Portal perusahaan dan memverifikasi bahwa itu muncul di Portal perusahaan. Jika tidak, pengguna harus mendaftarkan perangkat.
    
- Di Azure portal pergi ke **Intune \> kepatuhan perangkat**. Di bawah **Monitor** klik **perangkat kepatuhan**. Lihat laporan kepatuhan perangkat Anda untuk memverifikasi bahwa perangkat pengguna ditandai sebagai compliant. 
    
- Di Azure portal pergi ke **Intune \> kepatuhan perangkat**. Dalam **mengelola**, klik **kebijakan**. Dalam daftar kebijakan kepatuhan, pastikan bahwa profil yang ditetapkan ke perangkat pengguna Anda. Jika profil tidak ditetapkan, maka Intune tidak akan bisa mengkonfirmasi perangkat kepatuhan status. 
    
- Mengedit tugas bersyarat akses pengguna.
    
1. Di Azure portal pergi ke **Intune \> akses bersyarat \> kebijakan**
    
2. Pilih kebijakan dari daftar
    
3. Klik **pengguna dan grup**
    
4. Untuk menargetkan kebijakan tertentu pada seseorang, menambahkan mereka ke daftar **termasuk** . Untuk memastikan bahwa orang yang dihilangkan dari kebijakan, menambahkannya ke **mengecualikan** daftar. 
    
Baca lebih lanjut: [bagaimana perangkat akses bersyarat Monitor](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

