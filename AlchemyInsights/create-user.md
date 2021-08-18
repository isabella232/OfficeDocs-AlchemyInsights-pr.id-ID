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
ms.openlocfilehash: d86b2dd6d7915f0698cf950cd57f1065cde22219284edbbc0e64f3a5e69ff252
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896718"
---
# <a name="create-user"></a>Buat pengguna

**PENGUMUMAN:**

- [Penghentian dukungan masuk WebView dari Google dimulai 4 Januari 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Uji apakah aplikasi Anda akan terpengaruh oleh [panduan Google tentang](https://go.microsoft.com/fwlink/?linkid=2157323) kompatibilitas pengujian.
- Pastikan Anda menggunakan sistem webview atau browser sistem saat masuk pengguna Anda dengan akun Google konsumen. Untuk informasi selengkapnya, [lihat Masalah saat masuk ke aplikasi menggunakan browser Chrome saja](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Saya tidak dapat membuat pengguna baru di direktori Azure AD**

1. Pastikan bahwa Anda memiliki wewenang untuk membuat pengguna standar baru. Hanya administrator global atau Peran administrator pengguna di Azure Active Directory (AD) yang bisa membuat pengguna standar baru. Jika Anda tidak berada dalam salah satu peran ini, minta administrator untuk menambahkan Anda ke salah satu peran ini atau untuk membuat akun pengguna baru untuk Anda.
1. Pastikan bahwa nama pengguna berada di domain yang diverifikasi di Azure AD Anda. Jika tidak memiliki nama domain kustom terverifikasi di Azure AD, Anda dapat menggunakan domain awal Azure AD, yang diakhiri dengan *.onmicrosoft.com.
1. Pastikan bahwa nama pengguna berada di domain yang tidak t bagian dari Azure AD dari AD lokal Anda. Pengguna tidak bisa ditambahkan di awan dengan nama domain yang di federasinya dari lokal.
1. Pastikan tidak ada pengguna atau kontak lain yang telah memiliki nama pengguna yang ingin Anda tetapkan ke pengguna baru. Nama pengguna harus unik di Azure AD.
1. Lihat [peran dan administrator Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) untuk Azure AD Anda.
1. Lihat nama [domain untuk](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD Anda.
1. Tinjau [Log audit](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) untuk melihat informasi lebih mendetail tentang pengguna yang baru dibuat atau dihapus seperti siapa yang melakukan tindakan dan kapan.
1. Untuk informasi selengkapnya tentang menambahkan pengguna baru, [lihat Menggunakan portal Azure untuk membuat pengguna baru di Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal).
1. [Peran administratif Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Izin peran administrator Azure Active Directory
1. Anda juga dapat [menggunakan Azure AD PowerShell untuk membuat pengguna baru.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
