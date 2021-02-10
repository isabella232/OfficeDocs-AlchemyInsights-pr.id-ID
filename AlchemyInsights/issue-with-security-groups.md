---
title: Masalah dengan grup keamanan
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177497"
---
# <a name="issue-with-security-groups"></a>Masalah dengan grup keamanan

**Jika Anda mendapatkan kesalahan jaringan AADDS104**

Aturan grup keamanan jaringan tidak valid adalah penyebab paling umum kesalahan jaringan untuk layanan domain Azure Active Directory (AD DS). Grup keamanan jaringan untuk jaringan virtual harus mengizinkan akses ke Port dan protokol tertentu. Jika port tersebut diblokir, platform Azure tidak bisa memantau atau memperbarui domain terkelola. Sinkronisasi antara Azure AD dan Azure AD DS juga terpengaruh. Pastikan port default tetap terbuka untuk menghindari gangguan dalam layanan.

Untuk memahami dan mengatasi masalah umum untuk masalah konfigurasi grup keamanan jaringan, lihat [menambahkan dan memverifikasi grup keamanan](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
