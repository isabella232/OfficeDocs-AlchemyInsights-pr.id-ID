---
title: Mengaktifkan teknologi NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935130"
---
# <a name="turn-on-ndi-technology"></a>Mengaktifkan teknologi NDI

Teknologi NDI memerlukan dua langkah untuk diaktifkan untuk pengguna:

1. Admin penyewa harus mengaktifkan properti ' AllowNDIStreaming ' di CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Setelah perubahan ini diisi, pengguna akhir harus mengaktifkan teknologi® NDI untuk klien tertentu dari **pengaturan > izin**.

Untuk informasi selengkapnya, lihat [menggunakan teknologi NDI di Microsoft teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
