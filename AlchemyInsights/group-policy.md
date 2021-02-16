---
title: Kebijakan grup
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
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256779"
---
# <a name="group-policy"></a>Kebijakan grup

Pengaturan untuk objek pengguna dan komputer di layanan domain direktori aktif Azure (Azure AD DS) sering kali dikelola menggunakan objek kebijakan grup (GPO). Azure AD DS menyertakan GPO bawaan untuk pengguna AADDC dan AADDC. Anda dapat mengustomisasi GPO bawaan ini untuk mengonfigurasi kebijakan grup sebagaimana diperlukan untuk lingkungan Anda. Anggota grup administrator Azure AD DC memiliki hak istimewa administrasi kebijakan grup di domain Azure AD DS, dan juga dapat membuat GPO kustom dan unit organisasi (OU). Untuk informasi selengkapnya tentang kebijakan grup dan cara kerjanya, lihat [gambaran umum kebijakan grup](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Dalam lingkungan hibrid, kebijakan grup yang dikonfigurasi di lingkungan AD DS lokal tidak disinkronkan ke Azure AD DS. Untuk menentukan pengaturan konfigurasi untuk pengguna atau komputer di Azure AD DS, Edit salah satu GPO default atau buat GPO kustom.

Artikel ini [mengelola kebijakan grup](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) memperlihatkan kepada Anda cara menginstal alat manajemen kebijakan grup, bagaimana ton mengedit GPO bawaan, dan cara membuat GPO kustom.



