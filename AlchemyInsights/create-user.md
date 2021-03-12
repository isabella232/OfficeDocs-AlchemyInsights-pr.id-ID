---
title: Buat pengguna
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744976"
---
# <a name="create-user"></a>Buat pengguna

**Pengumuman**

- [Penghentian dukungan masuk WebView dari Google mulai 4 januari 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Uji apakah aplikasi Anda mungkin terpengaruh dengan mengikuti [Panduan Google](https://go.microsoft.com/fwlink/?linkid=2157323) tentang kompatibilitas pengujian.
- Pastikan Anda menggunakan browser sistem WebView atau sistem saat masuk ke pengguna Anda dengan akun Google konsumen. Untuk informasi selengkapnya, lihat [masalah masuk ke aplikasi menggunakan browser Chrome saja](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Saya tidak dapat membuat pengguna baru di direktori Azure AD saya**

1. Pastikan bahwa Anda memiliki wewenang untuk membuat pengguna standar baru. Hanya peran administrator global atau administrator pengguna di Azure Active Directory (AD) yang dapat membuat pengguna standar baru. Jika Anda tidak berada di salah satu peran ini, mintalah administrator untuk menambahkan Anda ke salah satu peran ini atau untuk membuat akun pengguna baru untuk Anda.
1. Pastikan bahwa nama pengguna berada di domain yang diverifikasi di Azure AD Anda. Jika Anda tidak memiliki nama domain kustom yang diverifikasi di Azure AD Anda, Anda bisa menggunakan domain awal Azure AD, yang diakhiri dengan *. onmicrosoft.com.
1. Pastikan bahwa nama pengguna berada di domain yang tidak digabungkan ke Azure AD dari iklan lokal Anda. Pengguna tidak dapat ditambahkan di awan dengan nama domain yang digabungkan dari lokal.
1. Pastikan bahwa tidak ada pengguna atau kontak lain yang sudah memiliki nama pengguna yang ingin Anda tetapkan ke pengguna baru. Nama pengguna harus unik di seluruh Azure AD.
1. Lihat [AZURE AD peran dan administrator](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) untuk Azure AD Anda.
1. Lihat [nama domain](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) untuk Azure AD Anda.
1. Tinjau [log audit](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) untuk melihat informasi mendetail selengkapnya tentang pengguna yang baru dibuat atau dihapus seperti siapa yang melakukan tindakan dan kapan.
1. Untuk informasi selengkapnya tentang menambahkan pengguna baru, lihat [menggunakan Azure portal untuk membuat pengguna baru di AZURE AD Anda](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Peran administratif AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): izin peran administrator di direktori aktif Azure
1. Anda juga bisa [menggunakan AZURE AD PowerShell untuk membuat pengguna baru](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
