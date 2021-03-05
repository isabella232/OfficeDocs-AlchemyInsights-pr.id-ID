---
title: Hari kerja untuk penyediaan pengguna AD masuk ke status karantina
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481877"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Hari kerja untuk penyediaan pengguna AD masuk ke status karantina

**Hari kerja untuk penyediaan pengguna AD masuk ke status karantina dan tidak ada pengguna yang dibuat di AD**

Hari kerja untuk penyediaan pengguna AD Ayub telah masuk ke status karantina dan log audit memperlihatkan kejadian kegagalan ekspor dengan kesalahan pesan kesalahan **: OperationsError-SvcErr: terjadi kesalahan operasi. Tidak ada referensi Superior yang telah dikonfigurasikan untuk layanan direktori. Layanan Direktori oleh karena itu tidak dapat menerbitkan referensi ke objek di luar Forest ini**. Kesalahan ini biasanya muncul jika OU wadah direktori aktif tidak diatur dengan benar atau jika terdapat masalah dengan pemetaan ekspresi yang digunakan untuk **Parenternama**.

Centang OU default untuk parameter **pengguna baru** untuk kesalahan ketik. Pastikan bahwa OU yang ditentukan sudah ada di iklan Anda. Jika Anda menggunakan **Parenternama** dalam pemetaan atribut, pastikan bahwa itu selalu mengevaluasi ke wadah yang diketahui dalam domain AD. Periksa kejadian ekspor dalam log audit untuk melihat nilai yang dihasilkan.

Untuk detail selengkapnya tentang mengonfigurasi workday untuk penyediaan otomatis, lihat [Tutorial: mengonfigurasi workday untuk penyediaan pengguna otomatis](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

