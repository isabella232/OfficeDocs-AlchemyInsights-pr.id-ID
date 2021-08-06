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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999243"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Tidak dapat Masuk ke Azure karena masalah browser (Browser mengalami hang, terus berputar, tidak dimuat, dll.)

Anda mungkin terkena dampak pemadaman. Periksa untuk melihat apakah terdapat gangguan yang sedang berlangsung: [Status Azure Health](https://status.azure.com/status/history/).

Silakan keluar dari semua sesi Azure yang aktif. Mulai mode in-private atau incognito di browser web.

Anda juga bisa mencoba untuk Merefresh browser, menggunakan browser lain, menghapus cookie singgahan jika di atas tidak berfungsi.

Pelajari [selengkapnya: Memecahkan masalah Masuk](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Tidak dapat mengakses langganan**

Di [portal Azure,](https://portal.azure.com/)pastikan bahwa direktori Azure yang benar telah dipilih dari akun di bagian kanan atas.

Di Pusat [Akun Azure,](https://account.windowsazure.com/Subscriptions)pastikan bahwa akun yang digunakan adalah admin akun.

Pelajari selengkapnya: [Memecahkan masalah langganan tidak ditemukan](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tidak dapat mengakses riwayat tagihan**

Admin akun harus memastikan bahwa pengguna yang mengakses informasi tagihan ditambahkan di Azure Active directory sebagai pengguna tamu: [Menambahkan atau menghapus pengguna baru.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Lalu pengguna harus diberi peran admin Global: [Menetapkan peran kepada pengguna](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Posting ini, pengguna bisa diberi akses tagihan menggunakan kebijakan RBAC: [Berikan akses ke tagihan.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dokumen yang Disarankan**

-   [Saya tidak dapat masuk untuk mengelola langganan Azure saya](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)