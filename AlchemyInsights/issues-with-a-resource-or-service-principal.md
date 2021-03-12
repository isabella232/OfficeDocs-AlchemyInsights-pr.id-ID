---
title: Masalah dengan prinsip sumber daya atau layanan
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714077"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Masalah dengan prinsip sumber daya atau layanan

1. Jika Anda baru saja memulai, [objek utama aplikasi dan layanan dalam direktori aktif Azure](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) menjelaskan pendaftaran aplikasi, objek aplikasi, dan prinsip layanan di direktori aktif Azure: apa yang dimaksud dengan mereka, dan bagaimana cara kerjanya, dan bagaimana keduanya terkait satu sama lain. Skenario multi-penyewa juga disajikan untuk mengilustrasikan hubungan antara objek aplikasi aplikasi dan objek utama layanan yang terkait.
2. Anda dapat mempelajari selengkapnya tentang hubungan antara aplikasi dan prinsipal layanan dengan membaca [aplikasi dan objek dasar layanan di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Cara: menggunakan portal untuk membuat akun AZURE AD aplikasi dan prinsip layanan yang bisa mengakses sumber daya](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) memperlihatkan kepada Anda cara membuat pimpinan aplikasi dan layanan Azure Active Directory (Azure AD) yang baru yang bisa digunakan dengan kontrol akses berbasis peran.
4. Dengan [api prinsip Layanan](https://docs.microsoft.com/graph/api/resources/serviceprincipal), Anda bisa secara sistematis mengelola contoh aplikasi dan mengontrol apa yang bisa dilakukan aplikasi dalam penyewa Anda.
5. [tipe sumber daya serviceprincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) mencantumkan semua properti dan metode untuk tipe sumber daya serviceprincipal.
6. [Perbedaan tipe sumber daya antara grafik AZURE AD dan Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) menyoroti perbedaan antara grafik Azure AD dan sumber daya Microsoft graph. Memperlihatkan sumber daya yang memiliki nama berbeda atau tidak tersedia; ini juga menyoroti sumber daya yang tersedia dalam versi beta Microsoft graph tetapi tidak dalam versi v 1.0.

**Masalah dengan pengguna tamu**

- [Mulai cepat: menambahkan pengguna tamu ke direktori Anda di portal Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) memperlihatkan kepada Anda cara menambahkan pengguna tamu baru ke direktori Azure AD Anda melalui portal Azure, mengirim undangan, dan melihat seperti apa proses Penukaran undangan pengguna tamu.
- [Tutorial: membuat aliran pengguna di Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) memperlihatkan kepada Anda cara membuat beberapa aliran pengguna yang dianjurkan dengan menggunakan Azure portal. Jika Anda mencari informasi tentang cara menyiapkan aliran kredensial kata sandi (ROPC) sumber daya di aplikasi Anda, lihat mengonfigurasi alur kredensial kata sandi pemilik sumber daya di Azure AD B2C.
