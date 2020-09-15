---
title: Cara menonaktifkan grup eksternal
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704131"
---
# <a name="how-to-disable-external-groups"></a>Cara menonaktifkan grup eksternal

Pesan eksternal Yammer menerapkan Exchange Transport Rules (ETRs), sekumpulan kontrol proaktif untuk mencegah agar informasi perusahaan tidak dibagikan. Untuk membatasi pengguna dari membuat grup eksternal, Anda perlu mengonfigurasi aturan transpor Exchange (ETR), lalu mengonfigurasi Yammer untuk menggunakan aturan transpor Exchange untuk memblokir pesan eksternal.
  
Setelah Anda membuat aturan di pusat admin Exchange Online, ikuti langkah-langkah ini untuk mengatur ETR untuk diterapkan di Yammer:
  
- Masuk ke Yammer sebagai admin terverifikasi, dan di **Pusat admin Yammer**, masuk ke **konten C dan \> pengaturan keamanan keamanan.**

- Di bawah **pesan eksternal**, pilih **Terapkan aturan transpor Exchange Online Exchange (etrs) di Yammer.**

- Pilih **Simpan**.

Untuk informasi selengkapnya, lihat [menonaktifkan pesan eksternal di jaringan Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  