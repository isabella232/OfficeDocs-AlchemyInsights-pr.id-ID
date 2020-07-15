---
title: Masalah dengan mesin onboarding
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141652"
---
# <a name="issues-with-onboarding-machines"></a>Masalah dengan mesin onboarding

Anda mungkin memiliki masalah dengan mesin onboarding untuk layanan MDATP. Jika Anda dapat mengakses mesin pengguna akhir, ikuti langkah berikut:

1. Unduh alat diagnostik [Penganalisis konektivitas klien](https://aka.ms/mdatpanalyzer) .
2. Ekstrak dan jalankan MDATPAnalyzer. CMD.
3. Temukan log diagnostik di folder yang disebut MDATPClientAnalyzerResult, folder yang sama di mana alat Analyzer diunduh.
4. Tinjau file log, MDATPClientAnalyzer.txt, untuk menemukan masalah konektivitas atau pengaturan proxy Internet.