---
title: Pemantauan akses bersyarat
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538750"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Pemantauan akses bersyarat untuk Asing

Pengguna dengan akses bersyarat yang ditargetkan akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk menyelesaikan, kami merekomendasikan satu atau lebih solusi berikut:
  
- Jika perangkat dianggap diterima, menyarankan pengguna untuk pergi ke app Portal perusahaan dan memverifikasi bahwa itu muncul di Portal perusahaan. Jika tidak, pengguna harus mendaftarkan perangkat.
    
- Di Azure portal pergi ke **Intune \> kepatuhan perangkat**. Di bawah **Monitor** klik **perangkat kepatuhan**. Lihat laporan kepatuhan perangkat Anda untuk memverifikasi bahwa perangkat pengguna ditandai sebagai compliant. 
    
- Di Azure portal pergi ke **Intune \> kepatuhan perangkat**. Dalam **mengelola**, klik **kebijakan**. Dalam daftar kebijakan kepatuhan, pastikan bahwa profil yang ditetapkan ke perangkat pengguna Anda. Jika profil tidak ditetapkan, maka Intune tidak akan bisa mengkonfirmasi perangkat kepatuhan status. 
    
- Mengedit tugas bersyarat akses pengguna.
    
1. Di Azure portal pergi ke **Intune \> akses bersyarat \> kebijakan**
    
2. Pilih kebijakan dari daftar
    
3. Klik **pengguna dan grup**
    
4. Untuk menargetkan kebijakan tertentu pada seseorang, menambahkan mereka ke daftar **termasuk** . Untuk memastikan bahwa orang yang dihilangkan dari kebijakan, menambahkannya ke **mengecualikan** daftar. 
    
Baca lebih lanjut: [bagaimana perangkat akses bersyarat Monitor](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

