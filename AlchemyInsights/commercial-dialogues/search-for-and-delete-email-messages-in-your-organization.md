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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948886"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Mencari dan menghapus pesan email di organisasi Anda

Ikuti langkah-langkah ini:

1. Jika Anda bukan admin global, untuk mencari pesan, akun Anda harus ditambahkan ke grup **peran Manajer eDiscovery atau** peran manajemen Pencarian **Kepatuhan**. Untuk menghapus pesan, Anda harus bergabung dalam **grup peran Manajemen Organisasi** atau peran manajemen Pencarian dan **Pembersihan**. Izin untuk peran ini ditetapkan di pusat kepatuhan [& keamanan.](https://protection.office.com)
2. [Buat pencarian konten](https://docs.microsoft.com/office365/securitycompliance/content-search) untuk menemukan pesan yang akan dihapus.
3. [Koneksi ke PowerShell Pusat & Security .](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Jika Anda menggunakan MFA, lihat instruksi berikut: Koneksi [Security & Compliance Center PowerShell menggunakan multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Hapus pesan: jalankan `New-ComplianceSearchAction` cmdlet untuk menghapus pesan. Pesan yang dihapus dipindahkan ke folder Item yang Dapat Dipulihkan pengguna. Untuk contoh perintah, lihat [Langkah 3: Menghapus pesan.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
