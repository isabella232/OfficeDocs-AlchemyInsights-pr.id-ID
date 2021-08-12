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
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932064"
---
# <a name="api-permissions-and-consent-process"></a>Izin API dan Proses Persetujuan

Agar aplikasi Anda mengakses data di Microsoft Graph, pengguna atau administrator harus memberikan izin yang tepat melalui proses persetujuan. [Referensi Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference) mencantumkan izin yang terkait dengan setiap rangkaian utama API Microsoft Graph. Panduan juga tentang cara menggunakan izin.

**Menyetel atau memperbarui prinsipal layanan**

- [Buat serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Artikel ini memperlihatkan cara membuat objek servicePrincipal baru.
- Membuat [prinsipal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) layanan & azure AD dalam portal - Artikel ini memperlihatkan pada Anda cara membuat aplikasi Azure Active Directory (Azure AD) dan prinsipal layanan baru yang bisa digunakan dengan kontrol akses berbasis peran.
- [Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - Artikel ini menguraikan pendaftaran aplikasi, objek aplikasi, dan prinsipal layanan di Azure Active Directory: apa itu, cara menggunakannya, dan bagaimana aplikasi saling terkait.

**Menambahkan atau memperbarui pendaftaran aplikasi dan memberikan persetujuan admin**

- [Buat pendaftaran aplikasi](https://docs.microsoft.com/graph/api/application-post-applications) - Artikel ini memperlihatkan pada Anda cara membuat objek aplikasi baru.
- [Memperbarui pendaftaran aplikasi - izin API](https://docs.microsoft.com/graph/api/application-update) - Artikel ini memperlihatkan cara memperbarui properti objek aplikasi.
- [Memberikan izin admin](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Untuk persetujuan dan persetujuan admin secara umum, kami mengharuskan admin secara eksplisit memberikan persetujuan.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Wadah manajemen peran untuk definisi peran terpadu dan penetapan peran untuk penyedia Microsoft 365 RBAC yang mendukung beberapa prinsipal dan beberapa lingkup dalam penugasan peran tunggal. Ini berbeda dari *tipe sumber daya aplikasi rbac.* Microsoft Intune adalah contoh dari penyedia RBAC seperti itu. Penugasan peran di Intune dapat memiliki larik pokok dan larik grup lingkup. **Dalam versi beta, artinya file masih dalam pengembangan dan tidak direkomendasikan untuk digunakan dalam produksi.**
