---
title: Sinkronisasi hash kata sandi untuk layanan domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177488"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Sinkronisasi hash kata sandi untuk layanan domain

**Jika instans Azure AD DS meminta Anda untuk mengaktifkan sinkronisasi hash kata sandi**

Anda menemukan skenario di mana Anda menjalankan lingkungan hibrid dengan pengguna yang melakukan sinkronisasi dari lingkungan Azure Active Directory Domain Services (AD DS) lokal. Skenario ini terjadi meskipun Anda mengalami sinkronisasi hash kata sandi dari AD DS lokal ke penyewa Azure AD Anda.

**Kannya**

Ini terjadi karena Azure AD Connect secara default tidak menyinkronkan warisan baru teknologi LAN Manager (NTLM) dan hash kata sandi Kerberos yang diperlukan untuk Azure AD DS.

**Solusi** 

Anda perlu mengonfigurasi Azure AD Connect untuk menyinkronkan hash kata sandi yang diperlukan untuk autentikasi NTLM dan Kerberos.

Setelah Azure AD Connect dikonfigurasikan, kejadian pembuatan di tempat atau perubahan kata sandi juga akan menyinkronkan hash kata sandi warisan ke Azure AD. Silakan lihat di [sini](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) untuk informasi selengkapnya tentang hal ini dan untuk panduan tentang cara mengaktifkan sinkronisasi kata sandi di lingkungan HIBRID AZURE AD DS.