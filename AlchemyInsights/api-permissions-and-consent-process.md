---
title: Izin API dan Proses Persetujuan
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404872"
---
# <a name="api-permissions-and-consent-process"></a>Izin API dan Proses Persetujuan

Agar aplikasi Anda mengakses data di Microsoft Graph, pengguna atau administrator harus memberikan izin yang tepat melalui proses persetujuan. [Referensi izin Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) mencantumkan izin yang terkait dengan setiap rangkaian utama API Microsoft Graph. Panduan juga tentang cara menggunakan izin.

**Menyetel atau memperbarui prinsipal layanan**

- [Buat serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Artikel ini memperlihatkan cara membuat objek servicePrincipal baru.
- [Membuat prinsipal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) layanan & Azure AD dalam portal - Artikel ini memperlihatkan cara membuat aplikasi Azure Active Directory (Azure AD) dan prinsipal layanan baru yang dapat digunakan dengan kontrol akses berbasis peran.
- [Pokok &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) aplikasi dalam Azure AD - Artikel ini menguraikan pendaftaran aplikasi, objek aplikasi, dan prinsipal layanan dalam Azure Active Directory: apa itu, cara menggunakannya, dan bagaimana aplikasi saling terkait.

**Menambahkan atau memperbarui pendaftaran aplikasi dan memberikan persetujuan admin**

- [Buat pendaftaran aplikasi](https://docs.microsoft.com/graph/api/application-post-applications) - Artikel ini memperlihatkan pada Anda cara membuat objek aplikasi baru.
- [Memperbarui pendaftaran aplikasi - izin API](https://docs.microsoft.com/graph/api/application-update) - Artikel ini memperlihatkan cara memperbarui properti objek aplikasi.
- [Memberikan izin admin](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Untuk persetujuan dan persetujuan admin secara umum, kami mengharuskan admin secara eksplisit memberikan persetujuan.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Wadah manajemen peran untuk definisi peran terpadu dan penetapan peran untuk penyedia RBAC Microsoft 365 yang mendukung beberapa prinsipal dan beberapa lingkup dalam penugasan peran tunggal. Ini berbeda dari *tipe sumber daya aplikasi rbac.* Microsoft Intune adalah contoh penyedia RBAC. Penugasan peran di Intune dapat memiliki larik pokok dan larik grup lingkup. **Dalam versi beta, artinya file masih dalam pengembangan dan tidak direkomendasikan untuk digunakan dalam produksi.**
