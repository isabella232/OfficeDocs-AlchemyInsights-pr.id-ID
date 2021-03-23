---
title: Mengimpor dan mengekspor dari Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036123"
---
# <a name="import-and-export-from-yammer"></a>Mengimpor dan mengekspor dari Yammer

**Mengimpor**

Opsi impor pengguna berbeda-beda tergantung pada apakah jaringan Yammer Anda berada dalam [mode asli untuk Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), atau tidak.

- **Mode non-asli**: pengguna dapat diimpor ke grup menggunakan [Tambahkan dari buku alamat](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (batas ke pengguna 100) dalam pengaturan grup, atau ke jaringan menggunakan [pembaruan massal](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) dalam admin jaringan.
- **Mode asli**: keanggotaan grup dan operasi keanggotaan jaringan harus dilakukan dari [portal admin Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [portal Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), atau menggunakan opsi lain Azure AD. Jaringan dalam mode asli tidak lagi memiliki akses ke pembaruan sekaligus fitur warisan lainnya.

> [!IMPORTANT]
> Yammer tidak pernah mendukung mengimpor konten dari dalam admin jaringan Meskipun fitur ekspor data digunakan di jaringan lain. Konten dapat diposting ulang oleh solusi mitra atau api REST Yammer.

**Ex**

[Mengekspor data jaringan dalam admin jaringan](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) memperbolehkan ekspor konten dari jaringan Yammer, termasuk pesan dan file. Lampiran bisa sangat besar dan akan menyebabkan ekspor untuk mendapatkan waktu yang signifikan untuk menyelesaikannya. Kami merekomendasikan bahwa jaringan aktif diekspor menggunakan [api ekspor data](https://developer.yammer.com/docs/data-export-api) dalam potongan menurut hari atau minggu. Dukungan Microsoft tidak menyediakan skrip kustom untuk tujuan ini.

[Ekspor GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) terpisah ada untuk mengekspor konten untuk pengguna individual.