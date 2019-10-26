---
title: Cara menonaktifkan eksternal grup
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739496"
---
# <a name="how-to-disable-external-groups"></a>Cara menonaktifkan eksternal grup

Pesan eksternal Yammer berlaku Exchange Transport Rules (ETRs), seperangkat kontrol proaktif untuk mencegah berbagi informasi perusahaan. Untuk membatasi pengguna membuat grup eksternal, Anda harus mengkonfigurasi aturan transpor Exchange (ETR), dan kemudian mengkonfigurasi heboh menggunakan aturan Exchange Transport untuk memblokir pesan eksternal.
  
Setelah Anda membuat aturan di Exchange Online Admin Center, ikuti langkah berikut untuk menetapkan ETR untuk menerapkan di heboh:
  
- Log on ke heboh sebagai admin diverifikasi, dan di **Pusat admin heboh**, pergi ke C **konten dan pengaturan keamanan keamanan \> .**

- Di bawah **pesan eksternal**, pilih **menerapkan Exchange Online Exchange Transport Rules (etrs) di Yammer.**

- Pilih **Simpan**.

Untuk informasi selengkapnya, lihat [menonaktifkan pesan eksternal di jaringan heboh](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  