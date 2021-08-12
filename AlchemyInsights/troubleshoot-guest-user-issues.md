---
title: Memecahkan masalah pengguna tamu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939382"
---
# <a name="troubleshoot-guest-user-issues"></a>Memecahkan masalah pengguna tamu

1. Untuk panduan tentang mengelola akses tamu ke aplikasi, lihat [Mengelola akses tamu dengan ulasan akses Azure AD.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Menambahkan pengguna tamu ke direktori Anda di [portal Azure:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)Di mulai cepat ini, Anda akan menambahkan pengguna tamu baru ke direktori Azure AD Anda melalui portal Azure, mengirim undangan, dan melihat seperti apa proses penukaran undangan pengguna tamu itu.
1. [Menambahkan pengguna tamu dengan PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)Di mulai cepat ini, Anda akan menggunakan perintah New-AzureADMSInvitation untuk menambahkan satu pengguna tamu ke penyewa Azure.
1. Untuk mempelajari cara menetapkan pengguna, dan grup, ke aplikasi perusahaan di Azure Active Directory (Azure AD), baik dari dalam portal Azure atau dengan menggunakan PowerShell, lihat Mengelola penetapan pengguna untuk aplikasi [di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory B2B (Azure AD) berfungsi dengan sebagian besar aplikasi yang terintegrasi dengan Azure AD. Dalam artikel [ini,](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)kami akan memandu instruksi untuk mengonfigurasi beberapa aplikasi SaaS yang populer untuk digunakan dengan Azure AD B2B.
1. Sebagai organisasi yang menggunakan kemampuan kolaborasi B2B Azure Active Directory (Azure AD) untuk mengundang pengguna tamu dari organisasi mitra ke Azure AD, Anda kini dapat menyediakan akses pengguna B2B ini ke aplikasi lokal. Aplikasi lokal ini dapat menggunakan autentikasi berbasis SAML atau Integrated Windows Authentication (IWA) dengan delegasi terbatas Kerberos (KCD). Untuk informasi selengkapnya, [lihat Memberikan pengguna B2B dalam akses Azure AD ke aplikasi lokal Anda.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Pelajari cara memberikan [akses akun mitra yang dikelola secara lokal ke sumber daya awan menggunakan kolaborasi B2B Azure AD.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)