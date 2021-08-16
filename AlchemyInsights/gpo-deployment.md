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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067843"
---
# <a name="gpo-deployment"></a>Penyebaran GPO

Pengaturan untuk pengguna dan objek komputer di Azure Active Directory Domain Services (Azure AD DS) sering dikelola menggunakan Objek Kebijakan Grup (GPOS). Azure AD DS menyertakan GPOS bawaan untuk wadah Pengguna AADDC dan Komputer AADDC. Anda bisa mengkustomisasi GPOS bawaan ini untuk mengonfigurasi kebijakan grup sesuai kebutuhan untuk lingkungan Anda. Anggota grup administrator Azure AD DC memiliki hak istimewa administrasi kebijakan grup di domain Azure AD DS, dan juga dapat membuat GPOS kustom dan unit organisasi (OU). Untuk informasi selengkapnya tentang kebijakan grup apa itu dan cara kerjanya, lihat [Gambaran Umum Kebijakan Grup.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Dalam lingkungan hibrid, kebijakan grup yang dikonfigurasi di lingkungan AD DS lokal tidak disinkronkan ke Azure AD DS. Untuk menentukan pengaturan konfigurasi bagi pengguna atau komputer di Azure AD DS, edit salah satu GPOS default atau buat GPO kustom.

Artikel ini [Kelola Kebijakan](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) Grup memperlihatkan pada Anda cara menginstal alat Manajemen Kebijakan Grup, cara mengedit GPOS bawaan, dan cara membuat GPOS kustom.
