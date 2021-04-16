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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813691"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Kesalahan "Terdapat kesalahan memvalidasi token akses" selama onboarding Analitik Desktop

Kesalahan ini biasanya terlihat ketika token autentikasi kedaluwarsa. Biasanya, me-refresh halaman merefresh token. Namun, masalah ini dapat terjadi jika terdapat kebijakan Akses Kondisional apa pun yang diterapkan ke akun yang sedang digunakan untuk Analitik Desktop di papan. Anda dapat meninjau log Masuk Azure AD di Portal Azure untuk melihat apakah ada kegagalan masuk untuk akun yang sedang digunakan untuk onboarding Analitik Desktop.

Untuk informasi selengkapnya tentang Akses Bersyarat, kunjungi [Merencanakan penggunaan Akses Bersyarat Anda.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)