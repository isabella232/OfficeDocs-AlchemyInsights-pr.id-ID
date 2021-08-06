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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923134"
---
# <a name="rbac-rules"></a>Aturan RBAC

Jika mendapatkan kesalahan izin: 

- Klien dengan id objek tidak memiliki otorisasi untuk melakukan tindakan melalui lingkup **(kode:** Otorisasi Gagal) : ketika Anda mencoba membuat sumber daya, periksa apakah Anda saat ini masuk dengan pengguna yang diberi peran yang memiliki izin menulis ke sumber daya di lingkup yang dipilih. Misalnya, untuk mengelola mesin virtual dalam grup sumber daya, Anda harus memiliki peran [Kontributor Mesin Virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) pada grup sumber daya (atau lingkup induk). Untuk daftar izin untuk setiap peran bawaan, lihat Peran [bawaan untuk sumber daya Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Anda tidak memiliki izin untuk membuat permintaan **dukungan:** ketika Anda mencoba membuat atau memperbarui tiket dukungan, periksa apakah Anda saat ini masuk dengan pengguna yang diberi peran yang memiliki izin Microsoft.Support/supportTickets/write, seperti Kontributor [Permintaan](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)Dukungan.
- Tidak ada lagi penetapan peran yang bisa dibuat **(kode: RoleAssignmentLimitExceeded)**: ketika Anda mencoba untuk menetapkan peran, cobalah untuk mengurangi jumlah penetapan peran dengan menetapkan peran ke grup sebagai gantinya. Azure mendukung hingga **2000** penetapan peran per langganan.

Untuk detail selengkapnya tentang peran Azure RBAC, lihat [peran Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
