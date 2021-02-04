---
title: Mengubah pengaturan pembatasan EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075900"
---
# <a name="changing-ews-throttling-settings"></a>Mengubah pengaturan pembatasan EWS

Jalankan uji otomatis kami yang akan memungkinkan Anda mengubah kebijakan pembatasan EWS selama durasi migrasi. Perlu diperhatikan bahwa meskipun proses ini telah dijalankan, impor EWS masih akan dibatasi hingga 150 mb per 5 menit per kotak surat; untuk mencapai kecepatan throughput migrasi yang lebih tinggi, silakan migrasikan lebih banyak pengguna secara bersamaan.

Ingat bahwa perubahan kebijakan pembatasan EWS tidak berpengaruh pada jenis migrasi berikut (menggunakan alat Microsoft): Hibrid, Langsung/Bertahap (RPC/HTTP), Protokol Akses Pesan Internet, G Suite, Folder Publik, atau Layanan Impor PST.