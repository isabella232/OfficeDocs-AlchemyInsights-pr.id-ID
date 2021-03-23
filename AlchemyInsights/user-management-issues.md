---
title: Masalah manajemen pengguna
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036284"
---
# <a name="user-management-issues"></a>Masalah manajemen pengguna

**Apa yang terjadi pada pengguna yang ditetapkan saat ini ke aplikasi jika saya menonaktifkan ' penetapan pengguna yang diperlukan ' (Atur properti ini ke tidak)?**

Penonaktifan **penetapan pengguna yang diperlukan** tidak mempengaruhi pengguna yang saat ini ditetapkan. Menonaktifkan properti ini hanya akan memperbolehkan semua pengguna mengakses aplikasi. Semua pengguna yang tercantum dan pengguna yang ditetapkan ke grup dalam aplikasi masih valid.

- Untuk membatasi aplikasi Anda ke kumpulan pengguna tertentu, lihat- [membatasi aplikasi AZURE AD ke sekumpulan pengguna-platform Microsoft Identity | Dokumen Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Untuk menetapkan pengguna dan grup, ke aplikasi perusahaan di Azure Active Directory (Azure AD), baik dari dalam portal Azure atau dengan menggunakan PowerShell, lihat [mengelola penetapan pengguna untuk aplikasi di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Untuk mendelegasikan izin pembuatan dan manajemen aplikasi, lihat [mendelegasikan izin administrator manajemen aplikasi-AZURE AD | Dokumen Microsoft](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Sembunyikan aplikasi perusahaan tertentu dari pengguna** -gunakan langkah-langkah berikut ini untuk menyembunyikan semua aplikasi Microsoft 365 dari panel **myapps** . Aplikasi masih akan terlihat di Portal Office 365.

 1. Masuk ke Azure Portal sebagai administrator global untuk direktori Anda. 
 2. Pilih **Azure Active Directory**. 
 3. Pilih **pengguna**. 
 4. Pilih **pengaturan pengguna**. 
 5. Di bawah **aplikasi perusahaan**, klik **Kelola bagaimana pengguna akhir meluncurkan dan menampilkan aplikasinya**. 
 6. Untuk **pengguna hanya bisa melihat aplikasi office 365 di portal office 365**, klik **ya**. 
 7. Klik **Simpan**. 
 8. Untuk detail selengkapnya, lihat [menyembunyikan aplikasi perusahaan dari pengalaman pengguna di AZURE AD | Dokumen Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Jika Anda menawarkan aplikasi perangkat lunak sebagai layanan (SaaS) ke banyak organisasi, Anda bisa mengonfigurasi aplikasi Anda untuk menerima masuk dari penyewa Azure Active Directory (Azure AD) apa pun. Konfigurasi ini disebut "membuat multi-penyewa aplikasi Anda". Pengguna dalam penyewa Azure AD akan bisa masuk ke aplikasi Anda setelah setuju untuk menggunakan akunnya dengan aplikasi Anda. Untuk informasi selengkapnya, lihat [aplikasi Build yang masuk ke pengguna AZURE AD-platform Microsoft Identity | Dokumen Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Bagaimana cara pengguna akhir mengakses aplikasi setelah ia ditetapkan ke aplikasi?**

Setiap aplikasi di bilah aplikasi perusahaan memiliki link untuk pengguna akhir untuk mengakses. Pengguna juga bisa mengakses aplikasi melalui portal **Myapps** dengan cara yang mudah.

- **Ingin mengetahui aplikasi dan tipe aplikasi mana yang digunakan oleh pengguna?**

Anda dapat mengunduh laporan masuk untuk 30 hari terakhir dari **portal.azure.com > Azure Active directory> pendaftaran> mengunduh laporan**.

- Pelajari cara [memberikan izin kepada penyewa yang luas ke aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) dan [mengonfigurasi cara pengguna akhir menyetujui aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Pahami [cara kerja persetujuan](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) dan [Kelola persetujuan untuk aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


