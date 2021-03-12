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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746735"
---
# <a name="fix-transport-rules"></a>Memperbaiki aturan transpor

Aturan aliran email kustom terpengaruh pesan ini. Untuk meninjau aturan yang tepat, lakukan hal berikut:

1. Dalam hasil pengiriman, di bawah **informasi tambahan**, perhatikan **GUID** atau **nama kebijakan**.
2. Luncurkan Exchange Management Shell. Untuk informasi selengkapnya, lihat [membuka Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Jalankan perintah ini (menggunakan GUID dari pengiriman Anda):  **Get-TransportRule-identitas "GUID" | FL * Deskripsi***
4. Tinjau Deskripsi untuk melihat kondisi yang dikonfigurasi yang mempengaruhi pesan tersebut.

Untuk mempelajari selengkapnya, lihat [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
