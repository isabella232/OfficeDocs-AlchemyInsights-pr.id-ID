---
title: Terdapat kesalahan validasi kesalahan token akses selama on-boarding Analitik Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946618"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Kesalahan "Terdapat kesalahan memvalidasi token akses" selama onboarding Analitik Desktop

Kesalahan ini biasanya terlihat ketika token autentikasi kedaluwarsa. Biasanya, me-refresh halaman merefresh token. Namun, masalah ini dapat terjadi jika terdapat kebijakan Akses Kondisional apa pun yang diterapkan ke akun yang sedang digunakan untuk Analitik Desktop di papan. Anda dapat meninjau log Masuk Azure AD di Portal Azure untuk melihat apakah ada kegagalan masuk untuk akun yang sedang digunakan untuk onboarding Analitik Desktop.

Untuk informasi selengkapnya tentang Akses Bersyarat, kunjungi [Merencanakan penggunaan Akses Bersyarat Anda.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)