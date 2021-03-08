---
title: Mencari dan menghapus pesan email di organisasi Anda
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524285"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Mencari dan menghapus pesan email di organisasi Anda

Ikuti langkah-langkah ini:

1. Jika Anda bukan admin global, untuk mencari pesan yang harus ditambahkan ke **grup peran Manajer eDiscovery** atau **peran manajemen pencarian kepatuhan**. Untuk menghapus pesan, Anda harus bergabung dalam **grup peran manajemen organisasi** atau **peran manajemen pencarian dan** penghapusan. Izin untuk peran ini ditetapkan di [pusat kepatuhan & keamanan.](https://protection.office.com)
2. [Buat pencarian konten](https://docs.microsoft.com/office365/securitycompliance/content-search) untuk menemukan pesan yang akan dihapus.
3. [Sambungkan ke pusat kepatuhan & keamanan PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Jika Anda menggunakan MFA, lihat instruksi berikut: [menyambungkan ke keamanan & pusat kepatuhan PowerShell menggunakan autentikasi multifaktor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Hapus pesan: Jalankan `New-ComplianceSearchAction` cmdlet untuk menghapus pesan. Pesan yang dihapus dipindahkan ke folder Item yang dapat dipulihkan pengguna. Untuk perintah contoh, lihat [langkah 3: Hapus pesan.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
