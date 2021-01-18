---
title: Mengonfigurasi layanan domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885220"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Tidak dapat mengaktifkan AAD-DS atau Deployment gagal

Untuk mengatasi masalah layanan domain Azure AD (AAD-DS) yang tidak diaktifkan atau gagal untuk disebarkan, lakukan langkah-langkah berikut:

1. Jika Anda menggunakan jaringan virtual yang sudah ada, periksa NSG Anda untuk aturan yang diperlukan untuk menyinkronkan Port dalam AAD-DS di portal https://aka.ms/aadds-networking .
2. Periksa untuk melihat apakah pesan kesalahan Anda dijawab dalam panduan pemecahan masalah yang tersedia di  https://aka.ms/aadds-troubleshoot-enable .
3. Cobalah menyebarkan layanan domain Azure AD di jaringan virtual baru.
4. Ikuti panduan memulai tentang cara menggunakan AAD-DS: [membuat dan mengonfigurasi layanan domain AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Jika Anda mengalami masalah dalam menyebarkan layanan domain Azure AD, lihat [memecahkan masalah layanan domain AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) untuk mengatasi kesalahan umum untuk membantu Anda menyelesaikan pekerjaan. 

**Tidak dapat menonaktifkan AAD-DS**

AAD-DS tidak dapat dihentikan sebentar. Jika ingin berhenti menggunakan domain terkelola, Anda harus dihapus.
Untuk menghapus domain terkelola Anda, lihat [menghapus layanan domain AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



