---
title: Memecahkan masalah persetujuan pengguna
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007901"
---
# <a name="troubleshoot-user-consent"></a>Memecahkan masalah persetujuan pengguna

1. Anda dapat mengonfigurasi cara pengguna akhir menyetujui aplikasi melalui Portal Azure atau PowerShell. Lihat [Pengaturan persetujuan pengguna](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) untuk informasi selengkapnya.
1. Administrator juga dapat menggunakan [API Graph Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) untuk memberikan izin yang didelegasikan atas nama pengguna tunggal. Untuk informasi selengkapnya, [lihat Mendapatkan akses atas nama pengguna.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Kesalahan Persetujuan Pengguna:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)artikel ini membahas kesalahan yang dapat terjadi selama proses persetujuan pada aplikasi. Jika Anda memecahkan masalah permintaan persetujuan yang tidak diharapkan yang tidak berisi pesan kesalahan apa pun, lihat [Skenario Autentikasi untuk Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).