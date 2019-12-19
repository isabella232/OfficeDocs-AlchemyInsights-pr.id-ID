---
title: Ada kesalahan memvalidasi galat token akses selama desktop Analytics on-boarding
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741202"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Galat "ada kesalahan memvalidasi akses token" selama desktop Analytics onboarding

Galat ini biasanya diamati saat token otentikasi kedaluwarsa. Biasanya, menyegarkan halaman menyegarkan Token. Namun, masalah ini dapat bertahan jika ada kebijakan akses bersyarat yang diterapkan ke akun yang digunakan untuk di papan desktop Analytics. Anda dapat meninjau Azure AD masuk log di Azure portal untuk melihat apakah ada kegagalan masuk untuk akun yang digunakan untuk onboarding desktop Analytics.

Untuk informasi lebih lanjut tentang akses bersyarat, kunjungi [rencanakan penyebaran akses bersyarat Anda](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).