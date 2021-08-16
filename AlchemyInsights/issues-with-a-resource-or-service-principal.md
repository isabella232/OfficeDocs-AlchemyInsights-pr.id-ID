---
title: Masalah dengan Sumber Daya atau Prinsipal Layanan
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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028079"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Masalah dengan Sumber Daya atau Prinsipal Layanan

1. Jika Anda baru saja memulai, Objek prinsipal aplikasi dan layanan di [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) menguraikan pendaftaran aplikasi, objek aplikasi, dan prinsipal layanan di Azure Active Directory: apa itu, cara menggunakannya, dan bagaimana mereka saling terkait. Skenario contoh multi-penyewa juga disajikan untuk menggambarkan hubungan antara objek aplikasi dan objek prinsipal layanan yang terkait.
2. Anda dapat mempelajari selengkapnya tentang hubungan antara aplikasi dan prinsipal layanan dengan membaca aplikasi [dan objek prinsipal layanan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. Caranya: Menggunakan portal untuk membuat prinsipal layanan dan aplikasi [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) yang dapat mengakses sumber daya memperlihatkan cara membuat aplikasi Azure Active Directory (Azure AD) dan prinsipal layanan baru yang dapat digunakan dengan kontrol akses berbasis peran.
4. Dengan [API prinsipal layanan,](https://docs.microsoft.com/graph/api/resources/serviceprincipal)Anda dapat mengelola secara terprogram instans aplikasi dan mengontrol apa yang dapat dilakukan aplikasi dalam penyewa Anda.
5. [tipe sumber daya servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) mencantumkan semua properti dan metode untuk tipe sumber daya servicePrincipal.
6. [Perbedaan tipe sumber daya antara Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) dan Microsoft Graph menyoroti perbedaan antara Azure AD Graph dan Microsoft Graph sumber daya. Ini memperlihatkan sumber daya yang memiliki nama berbeda atau tidak tersedia; Ini juga menyoroti sumber daya yang tersedia di microsoft Graph versi beta tapi tidak di versi v1.0.

**Masalah dengan Pengguna Tamu**

- [Mulai cepat:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Menambahkan pengguna tamu ke direktori Anda di portal Azure memperlihatkan cara menambahkan pengguna tamu baru ke direktori Azure AD melalui portal Azure, mengirimkan undangan, dan melihat seperti apa proses penukaran undangan pengguna tamu.
- [Tutorial: Membuat alur pengguna Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) memperlihatkan cara membuat beberapa saran alur pengguna menggunakan portal Azure. Jika mencari informasi tentang cara menyiapkan aliran kredensial kata sandi pemilik sumber daya (ROPC, Resource Owner Password Credentials) di aplikasi Anda, lihat Mengonfigurasi alur kredensial kata sandi pemilik sumber daya di Azure AD B2C.
