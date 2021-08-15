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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023525"
---
# <a name="turn-on-ndi-technology"></a>Mengaktifkan teknologi NDI

Teknologi NDI memerlukan dua langkah untuk diaktifkan bagi pengguna:

1. Admin penyewa harus mengaktifkan properti 'AllowNDIStreaming' di CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Setelah perubahan ini diisi, pengguna akhir harus mengaktifkan teknologi NDI® untuk klien tertentu dari Pengaturan > **Lokal.**

Untuk informasi selengkapnya, lihat [Menggunakan teknologi NDI Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
