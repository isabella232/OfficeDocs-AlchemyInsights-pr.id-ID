---
title: Aktifkan penyematan dialog lama untuk membuka laporan
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814267"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktifkan penyematan dialog lama untuk membuka laporan

**Gejala**

Pengguna tidak dapat membuka laporan. "Terjadi kesalahan. Periksa detail teknis untuk detail selengkapnya."

**Penyebab**

Laporan gagal dimuat di UCI dengan kesalahan, "Deskriptor formulir null atau tidak ditentukan." Laporan di UCI masih memerlukan dialog lama, sehingga sistem pelanggan harus mengaktifkan *allowlegacydialogsembedding*.

**Solusi**

1. Buka **Pengaturan >Administrasi > Pengaturan Sistem > tab Umum**.

2. Tetapkan "Aktifkan penyematan dialog lama tertentu di klien browser Antarmuka Terpadu" ke **Ya**.
