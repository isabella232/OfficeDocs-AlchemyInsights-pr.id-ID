---
title: Ikon Kalender tidak muncul di klien Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932205"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ikon Kalender tidak muncul di klien Teams

Tab Kalender di Teams memerlukan akses ke kotak surat Exchange melalui Layanan Web Exchange. Kotak surat Exchange bisa Online atau Lokal. Untuk pengguna Online yang tidak melihat Tab Kalender, pastikan mereka [dilisensikan untuk kotak surat Exchange Online dan kotak surat diaktifkan](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Jika pengguna memiliki kotak surat yang valid di Exchange Online, tetapi tetap tidak bisa melihat tab Kalender, Anda mungkin mengalami masalah jaringan. Gunakan [Penganalisis Konektivitas Jarak Jauh Microsoft](https://testconnectivity.microsoft.com/) dan jalankan **Tes Konektivitas Layanan Web Microsoft Exchange** untuk pengguna yang terdampak.

Terakhir, perisa [Aplikasi Teams – Kebijakan penyiapan aplikasi](https://admin.teams.microsoft.com/policies/app-setup) untuk memastikan aplikasi Kalender tidak dihapus dari kebijakan yang diterapkan pada pengguna (kemungkinan besar kebijakan **Global (default skala Organisasi)**.

Jika pengguna Anda di rumah menggunakan Lokal, Anda perlu mengonfirmasi bahwa konfigurasi Hibrid Anda sehat. Gunakan [Panduan Konfigurasi Hibrid](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) untuk memecahkan masalah.

Perhatikan bahwa [Teams membutuhkan Exchange 2016 CU3 atau lebih tinggi](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
