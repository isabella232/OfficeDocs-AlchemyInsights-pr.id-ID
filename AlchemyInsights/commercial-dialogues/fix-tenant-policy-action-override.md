---
title: Memperbaiki kebijakan Penyewa (penggantian tindakan)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326800"
---
# <a name="fix-tenant-policy-action-override"></a>Memperbaiki kebijakan Penyewa (penggantian tindakan)

Salah satu kebijakan anti spam Anda mempengaruhi pesan ini. Untuk meninjau kebijakan, lakukan langkah-langkah berikut ini:

1. Di portal Pertahanan Microsoft 365, masuk ke Email & Kebijakan Kolaborasi & aturan kebijakan <https://security.microsoft.com/>  \>  \>  \> **Ancaman Anti spam** di **bagian** Kebijakan.

   Untuk langsung masuk ke **halaman Kebijakan anti spam,** gunakan <https://security.microsoft.com/antispam> .

2. Pada halaman Kebijakan **anti spam,** pilih kebijakan dengan mengklik nama kebijakan ( Tipe adalah  Kebijakan **anti spam** kustom atau Nama adalah Kebijakan masuk **Anti Spam (Default)**).
3. Di flyout detail yang muncul, pilih **Edit tindakan** di **bagian** Tindakan.
4. Di bagian Tindakan **pesan,** tinjau putusan untuk **Spam,** **Spam**  kepercayaan **tinggi,** Pengelabuan , dan Pengelabuan kepercayaan tinggi untuk melihat apakah salah satu nilai berikut ini dipilih:
   - **Tambahkan header X**
   - **Menambahkan baris subjek dengan teks**
   - **Alihkan pesan ke alamat email**
   - **Menghapus pesan**
   - **Tidak ada tindakan**

   Pengaturan Standar mungkin diterapkan **ke semua** pelanggan Exchange Online Protection dampak pesan.

Untuk informasi selengkapnya, [lihat Mengonfigurasi kebijakan anti spam di EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
