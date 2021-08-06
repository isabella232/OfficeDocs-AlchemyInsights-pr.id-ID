---
title: Workday to AD User Provisioning goes into quarantine state
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036495"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday to AD User Provisioning goes into quarantine state

**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**

Pekerjaan Hari Kerja ke Pekerjaan Penyediaan Pengguna AD telah masuk ke status karantina dan log audit memperlihatkan kejadian kegagalan ekspor dengan pesan **kesalahan: OperationsError-SvcErr: Terjadi kesalahan operasi. Tidak ada referensi superior yang telah dikonfigurasi untuk layanan direktori. Oleh karena itu, layanan direktori tidak dapat menerbitkan rujukan ke objek di luar hutan ini.** Kesalahan ini biasanya muncul jika Active Directory Container OU tidak diatur dengan benar atau jika ada masalah dengan Pemetaan Ekspresi yang digunakan untuk **parentDistinguishedName**.

Periksa DEFAULT OU untuk **parameter Pengguna Baru** jika terjadi kesalahan ketik. Pastikan bahwa OU yang ditentukan sudah ada di AD Anda. Jika Anda menggunakan **parentDistinguishedName** dalam pemetaan atribut, pastikan bahwa pemetaan itu selalu mengevaluasi ke wadah yang diketahui dalam domain AD. Periksa kejadian Ekspor dalam log audit untuk melihat nilai yang dihasilkan.

Untuk detail selengkapnya tentang mengonfigurasi hari kerja untuk penyediaan otomatis, lihat [Tutorial: Mengonfigurasi Hari Kerja untuk penyediaan pengguna otomatis.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

