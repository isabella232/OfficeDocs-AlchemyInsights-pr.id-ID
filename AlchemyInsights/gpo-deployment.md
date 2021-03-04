---
title: Penyebaran GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427568"
---
# <a name="gpo-deployment"></a>Penyebaran GPO

Pengaturan untuk objek pengguna dan komputer di layanan domain direktori aktif Azure (Azure AD DS) sering kali dikelola menggunakan objek kebijakan grup (GPO). Azure AD DS menyertakan GPO bawaan untuk pengguna AADDC dan AADDC. Anda dapat mengustomisasi GPO bawaan ini untuk mengonfigurasi kebijakan grup sebagaimana diperlukan untuk lingkungan Anda. Anggota grup administrator Azure AD DC memiliki hak istimewa administrasi kebijakan grup di domain Azure AD DS, dan juga dapat membuat GPO kustom dan unit organisasi (OU). Untuk informasi selengkapnya tentang kebijakan grup dan cara kerjanya, lihat [gambaran umum kebijakan grup](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Dalam lingkungan hibrid, kebijakan grup yang dikonfigurasi di lingkungan AD DS lokal tidak disinkronkan ke Azure AD DS. Untuk menentukan pengaturan konfigurasi untuk pengguna atau komputer di Azure AD DS, Edit salah satu GPO default atau buat GPO kustom.

Artikel ini [mengelola kebijakan grup](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) memperlihatkan kepada Anda cara menginstal alat manajemen kebijakan grup, bagaimana ton mengedit GPO bawaan, dan cara membuat GPO kustom.
