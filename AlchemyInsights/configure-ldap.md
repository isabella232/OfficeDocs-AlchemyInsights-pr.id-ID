---
title: Mengonfigurasi LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885163"
---
# <a name="configure-ldap"></a>Mengonfigurasi LDAP

Untuk mengonfigurasi LDAP, lakukan hal berikut:

1. Periksa kesehatan domain Anda di [portal Azure](https://aka.ms/aadds-health).
1. Pastikan langganan Azure AD yang valid tersedia dan layanan domain AD Azure telah diaktifkan.
1. Sertifikat yang diperlukan untuk mengaktifkan LDAP aman harus diperoleh dari otoritas sertifikasi publik tepercaya atau sertifikat yang ditandatangani sendiri.
1. Pastikan sertifikat mengikuti [panduan](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)yang diperlukan.

**Sertifikat tidak valid**
1. Untuk memperpanjang sertifikat, ikuti langkah-langkah untuk membuat sertifikat baru dan mengunggah ulang: [MENGONFIGURASI LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Untuk mengatasi masalah umum dengan peringatan LDAP aman dalam layanan domain Azure Active Directory, lihat [mengatasi pemberitahuan LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
