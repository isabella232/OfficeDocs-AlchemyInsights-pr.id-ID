---
title: Memperbaiki aturan transpor
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034757"
---
# <a name="fix-transport-rules"></a>Memperbaiki aturan transpor

Aturan aliran email kustom memengaruhi pesan ini. Untuk meninjau aturan yang tepat, lakukan hal berikut:

1. Dalam hasil pengiriman, di **bawah Informasi tambahan,** perhatikan **GUID** atau **Nama Kebijakan**.
2. Luncurkan Exchange Shell Manajemen. Untuk informasi selengkapnya, [lihat Membuka Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Jalankan perintah ini (menggunakan GUID dari pengiriman  **Anda): Get-TransportRule -identity "GUID" | fl * Deskripsi***
4. Tinjau deskripsi untuk melihat kondisi yang dikonfigurasi yang memengaruhi pesan tersebut.

Untuk mempelajari selengkapnya, lihat [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
