---
title: 'Peran RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583548"
---
# <a name="rbac-rules"></a>Aturan RBAC

Jika Anda mendapatkan kesalahan izin: 

- **Klien dengan ID objek tidak memiliki otorisasi untuk melakukan tindakan di atas lingkup (kode: Otorisasigagal)**: ketika Anda mencoba membuat sumber daya, periksa apakah saat ini Anda masuk dengan pengguna yang diberi peran yang memiliki izin menulis ke sumber daya di lingkup yang dipilih. Misalnya, untuk mengelola mesin virtual dalam grup sumber daya, Anda harus memiliki peran [kontributor mesin virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) di grup sumber daya (atau lingkup induk). Untuk daftar izin untuk setiap peran bawaan, lihat [peran bawaan untuk sumber daya Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Anda tidak memiliki izin untuk membuat permintaan dukungan**: ketika mencoba membuat atau memperbarui tiket dukungan, periksa apakah Anda saat ini masuk dengan pengguna yang ditetapkan peran yang memiliki izin Microsoft. support/supportticket/Write, seperti [kontributor permintaan dukungan](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Tidak ada lagi penetapan peran yang bisa dibuat (kode: peran Roleassignmentlimitterlamp)**: ketika Anda mencoba menetapkan peran, cobalah untuk mengurangi jumlah penetapan peran dengan menetapkan peran ke grup. Azure mendukung hingga **2000** penetapan peran per langganan.

Untuk detail selengkapnya tentang peran Azure RBAC, lihat [peran AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
