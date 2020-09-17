---
title: Ada kesalahan validasi kesalahan token Access selama analitik desktop di dalam pesawat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783554"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Kesalahan "terjadi kesalahan validasi token Access" selama orientasi analitik desktop

Kesalahan ini biasanya diamati ketika token autentikasi kedaluwarsa. Biasanya, refresh halaman me-refresh Token. Namun, masalah ini bisa terjadi jika ada kebijakan akses bersyarat yang diterapkan ke akun yang digunakan untuk analitik desktop di papan. Anda bisa meninjau log masuk Azure AD di Azure portal untuk melihat apakah ada kegagalan masuk untuk akun yang digunakan untuk orientasi analitik desktop.

Untuk informasi selengkapnya tentang akses bersyarat, kunjungi [merencanakan penggunaan akses bersyarat Anda](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).