---
title: Pengontrol domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901026"
---
# <a name="domain-controller"></a>Pengontrol domain

**Tidak dapat mengaktifkan AAD-DS atau Deployment gagal**

Untuk mengatasi masalah layanan domain Azure AD (AAD-DS) yang tidak diaktifkan atau gagal untuk disebarkan, lakukan langkah-langkah berikut:

1. Jika Anda menggunakan jaringan virtual yang sudah ada, periksa NSG Anda untuk aturan yang diperlukan untuk menyinkronkan Port dalam AAD-DS di portal https://aka.ms/aadds-networking .
2. Periksa untuk melihat apakah pesan kesalahan Anda dijawab dalam panduan pemecahan masalah yang tersedia di  https://aka.ms/aadds-troubleshoot-enable .
3. Cobalah menyebarkan layanan domain Azure AD di jaringan virtual baru.
4. Ikuti panduan memulai tentang cara menyebarkan AAD-DS, yang tersedia di [tutorial untuk membuat layanan domain AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Jika Anda mengalami masalah dalam menyebarkan layanan domain Azure AD, lihat [memecahkan masalah layanan domain AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) untuk mengatasi kesalahan umum untuk membantu Anda menyelesaikan pekerjaan. 

**Tidak dapat menonaktifkan AAD-DS**

AAD-DS tidak dapat dihentikan sebentar. Jika ingin berhenti menggunakan domain terkelola, Anda harus dihapus.

Jika Anda mengalami masalah, untuk mengatasi pesan kesalahan umum dan untuk langkah pemecahan masalah terkait untuk membantu Anda menyelesaikan pekerjaan, lihat [memecahkan masalah layanan domain Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
