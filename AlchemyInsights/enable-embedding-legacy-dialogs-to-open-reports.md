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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003392"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktifkan penyematan dialog lama untuk membuka laporan

**Gejala**

Pengguna tidak dapat membuka laporan. "Terjadi kesalahan. Periksa detail teknis untuk detail selengkapnya."

**Penyebab**

Laporan gagal dimuat di UCI dengan kesalahan, "Deskriptor formulir null atau tidak ditentukan." Laporan di UCI masih memerlukan dialog lama, sehingga sistem pelanggan harus mengaktifkan *allowlegacydialogsembedding*.

**Solusi**

1. Buka **Pengaturan >Administrasi > Pengaturan Sistem > tab Umum**.

2. Tetapkan "Aktifkan penyematan dialog lama tertentu di klien browser Antarmuka Terpadu" ke **Ya**.
