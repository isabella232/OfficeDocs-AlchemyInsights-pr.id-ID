---
title: Sinkronisasi grup
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256794"
---
# <a name="group-sync"></a>Sinkronisasi grup

Artikel ini menyediakan panduan pada sinkronisasi grup.

1. Jika admin global atau pemilik grup tidak dapat mengubah properti grup atau menambahkan anggota atau menetapkan pemilik di portal Azure, pastikan sumber otoritas untuk grup adalah Azure Active Directory (Azure AD) untuk admin global atau pemilik grup untuk mengubah grup.
2. Sebelum mencoba menghapus grup yang disinkronkan di Azure AD, pastikan Anda telah [menghapus semua lisensi yang ditetapkan](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) untuk menghindari kesalahan.

Untuk memahami cara menyinkronkan pengguna, grup, dan kontak, lihat [sinkronisasi AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), dan ikuti [sinkronisasi grup lokal ke AZURE menggunakan Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) untuk menyinkronkan grup pada perm menggunakan AD Connect.

Ikuti panduan ini [pemecahan masalah kesalahan selama sinkronisasi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) untuk memecahkan masalah kesalahan umum selama sinkronisasi.

