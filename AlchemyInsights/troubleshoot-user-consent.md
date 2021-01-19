---
title: Memecahkan masalah izin pengguna
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901189"
---
# <a name="troubleshoot-user-consent"></a>Memecahkan masalah izin pengguna

1. Anda dapat mengonfigurasi cara pengguna akhir menyetujui aplikasi melalui Azure portal atau PowerShell. Lihat [pengaturan persetujuan pengguna](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) untuk informasi selengkapnya.
1. Administrator juga dapat menggunakan [api Microsoft graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) untuk memberikan persetujuan kepada izin delegasi atas nama satu pengguna. Untuk informasi selengkapnya, lihat [mendapatkan akses atas nama pengguna](https://docs.microsoft.com/graph/auth-v2-user).
1. [Kesalahan persetujuan pengguna](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): artikel ini membahas kesalahan yang bisa terjadi selama proses menyetujui aplikasi. Jika Anda memecahkan permintaan persetujuan tidak terduga yang tidak berisi pesan kesalahan, lihat [skenario autentikasi untuk AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).