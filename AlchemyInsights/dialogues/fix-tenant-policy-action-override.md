---
title: Memperbaiki kebijakan penyewa (menimpa tindakan)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694061"
---
# <a name="fix-tenant-policy-action-override"></a>Memperbaiki kebijakan penyewa (menimpa tindakan)

Kebijakan anti spam di penyewa Anda mempengaruhi pesan ini. Untuk meninjau kebijakan, lakukan hal berikut:

1. Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), lalu masuk ke kebijakan **manajemen ancaman**  >    >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Periksa untuk melihat apakah **sumber kebijakan** menunjukkan hal berikut:  **Add-Xheader/Modifysubject/redirect/Delete/No Action/Bcc message**

    Jika demikian, pada tab **kustom** , periksa pengaturan kebijakan yang mempengaruhi pesan. Ada kemungkinan bahwa **pengaturan standar** yang diterapkan ke semua pelanggan Exchange Online Protection mempengaruhi pesan tersebut.

Untuk informasi selengkapnya tentang mengonfigurasi kebijakan filter spam, lihat [mengonfigurasi kebijakan filter spam Anda](https://go.microsoft.com/fwlink/?linkid=2101431).
