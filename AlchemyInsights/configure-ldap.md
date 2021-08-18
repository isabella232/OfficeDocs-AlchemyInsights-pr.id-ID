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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090415"
---
# <a name="configure-ldap"></a>Mengonfigurasi LDAP

Untuk mengonfigurasi LDAP, lakukan hal berikut ini:

1. Periksa kesehatan domain Anda di [portal Azure.](https://aka.ms/aadds-health)
1. Pastikan langganan Azure AD yang valid tersedia dan Layanan Domain Azure AD telah diaktifkan.
1. Sertifikat yang diperlukan untuk mengaktifkan LDAP aman harus diperoleh dari otoritas sertifikasi publik tepercaya atau menjadi sertifikat yang ditandatangani sendiri.
1. Pastikan sertifikat tersebut mengikuti panduan yang [diperlukan.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Sertifikat Tidak Valid**
1. Untuk memperpanjang sertifikat, ikuti langkah-langkah untuk membuat sertifikat baru dan unggah ulang: [Konfigurasi LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Untuk mengatasi masalah umum dengan pemberitahuan LDAP Aman di Layanan Domain Azure Active directory, lihat [Mengatasi pemberitahuan LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
