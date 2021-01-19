---
title: Masalah izin admin
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901132"
---
# <a name="admin-consent-issues"></a>Masalah izin admin

1. Aktifkan [alur kerja izin admin](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) untuk memperbolehkan pengguna meminta persetujuan administrator secara langsung dari layar persetujuan.

1. Jika Anda atau pengguna aplikasi Anda melihat kesalahan yang tidak diharapkan selama proses persetujuan, lihat artikel ini untuk langkah pemecahan masalah: [kesalahan tak terduga saat melakukan persetujuan ke aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Pelajari selengkapnya tentang [persetujuan admin di platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), cara kerja [perintah persetujuan](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) , dan cara [mengevaluasi permintaan untuk persetujuan admin penyewa-lebar](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Aplikasi yang terintegrasi dengan platform Microsoft Identity ikuti model otorisasi yang memberi pengguna dan administrator kontrol atas bagaimana data bisa diakses. Penerapan model otorisasi telah diperbarui pada titik akhir platform identitas Microsoft, dan mengubah cara aplikasi harus berinteraksi dengan platform identitas Microsoft. Lihat [izin dan persetujuan di titik akhir platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) untuk gambaran umum model otorisasi ini, termasuk lingkup, izin, dan persetujuan.