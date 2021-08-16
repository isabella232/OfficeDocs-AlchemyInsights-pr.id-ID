---
title: Mengubah pengaturan pembatasan EWS
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968380"
---
# <a name="changing-ews-throttling-settings"></a>Mengubah pengaturan pembatasan EWS

Jalankan uji otomatis kami yang akan memungkinkan Anda mengubah kebijakan pembatasan EWS selama durasi migrasi. Perlu diperhatikan bahwa meskipun proses ini telah dijalankan, impor EWS masih akan dibatasi hingga 150 mb per 5 menit per kotak surat; untuk mencapai kecepatan throughput migrasi yang lebih tinggi, silakan migrasikan lebih banyak pengguna secara bersamaan.

Ingat bahwa perubahan kebijakan pembatasan EWS tidak berpengaruh pada jenis migrasi berikut (menggunakan alat Microsoft): Hibrid, Langsung/Bertahap (RPC/HTTP), Protokol Akses Pesan Internet, G Suite, Folder Publik, atau Layanan Impor PST.