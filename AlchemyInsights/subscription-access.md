---
title: Akses langganan
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807435"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Tidak dapat masuk ke Azure karena masalah browser (Hang browser, tetap berputar, tidak dimuat, dsb.)

Anda mungkin terpengaruh oleh gangguan. Silakan periksa untuk melihat apakah ada pemutusan yang sedang berlangsung: [status kesehatan Azure](https://status.azure.com/status/history/).

Keluar dari semua sesi Azure aktif. Mulai mode privat atau penyamaran di browser web Anda.

Anda juga dapat mencoba untuk me-refresh browser, menggunakan browser lain, menghapus cookie tembolok jika di atas tidak berfungsi.

Pelajari selengkapnya: [memecahkan masalah saat masuk](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Tidak dapat mengakses metode berlangganan**

Di [portal Azure](https://portal.azure.com/), pastikan bahwa direktori Azure yang benar telah dipilih dari akun di bagian kanan atas.

Di [pusat akun Azure](https://account.windowsazure.com/Subscriptions), pastikan jika akun yang digunakan adalah admin akun.

Pelajari selengkapnya: [memecahkan masalah langganan tidak ditemukan](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tidak dapat mengakses Riwayat tagihan**

Admin akun harus memastikan pengguna yang mengakses informasi tagihan ditambahkan di direktori Azure Active sebagai pengguna tamu: [menambahkan atau menghapus pengguna baru](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Pengguna tersebut harus diberi peran admin global: [menetapkan peran kepada pengguna](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Posting ini, pengguna bisa diberi akses tagihan menggunakan kebijakan RBAC: [memberi akses ke tagihan](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Dokumen yang direkomendasikan**

-   [Saya tidak dapat masuk untuk mengelola langganan Azure saya](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)