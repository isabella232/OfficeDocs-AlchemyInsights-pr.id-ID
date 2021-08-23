---
title: Pengaturan Outlook label default tidak diterapkan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454752"
---
# <a name="default-outlook-label-setting-not-applied"></a>Pengaturan Outlook label default tidak diterapkan

Jika pengaturan label default Outlook tidak diterapkan dengan benar dan label berbeda atau tidak ada label yang diterapkan, Anda mungkin mengalami masalah yang diketahui (MC277818) dan harus melakukan salah satu dari 2 opsi ini untuk mengatasi masalah tersebut:

**Opsi 1:**

1. Masuk ke Microsoft 365 Pusat Kepatuhan > **Solutions**  >  **Information Protection**.
1. Pilih **Kebijakan label**, dan pilih kebijakan label yang perlu Anda edit ( pengaturan **OutlookDefaultlabel** tidak diatur dengan benar pada kebijakan label yang dimaksud. Jalankan **Get-labelpolicy** untuk melihat pengaturan ini), lalu pilih **Edit kebijakan**.
1. Pilih **Berikutnya** hingga Anda melihat pengaturan Terapkan **label default** ini ke email , yang tersedia jika Anda memilih Haruskan pengguna untuk menerapkan **label** ke email dan dokumen pewarisan di kotak dialog **Pengaturan** kebijakan.
1. Dalam kotak **dialog Terapkan label default ke dokumen,** pilih Tidak **Ada** dari daftar menurun.
1. Pilih **Berikutnya** dan **Kirim** untuk menyimpan pengaturan label Anda.

**Opsi 2:**

Di Powershell Pusat Keamanan dan [Kepatuhan,](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)gunakan commandlet Set-LabelPolicy untuk  mengubah **OutlookDefaultlabel** menjadi Tidak Ada di {OutlookDefaultLabel="None"}.

Jalankan: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Untuk informasi selengkapnya tentang label default Outlook standar, [lihat Mengatur label default lain untuk Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).