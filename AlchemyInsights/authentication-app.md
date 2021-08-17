---
title: Aplikasi autentikasi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082945"
---
# <a name="authentication-app"></a>Aplikasi autentikasi

Jika Anda adalah Admin Global, Anda bisa dengan cepat mencari tahu apa yang terjadi atau mendiagnosis masalah yang terkait dengan masuknya pengguna dengan menggunakan Diagnostik [Masuk.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Mulai diagnostik dengan mengklik tombol "[Luncurkan Diagnostik](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)". 
1. Temukan kegiatan yang akan dianalisis dengan memasukkan detail yang Anda miliki tentang pengguna, aplikasi, waktu masuk, ID permintaan, atau ID korelasi.
1. Tinjau hasil diagnostik yang memperlihatkan detail tentang apa yang terjadi dan tindakan apa yang dapat Anda lakukan untuk membuat perubahan, jika diperlukan perubahan.

**Periksa skenario yang berlaku:**

1. Jika pengguna tidak mendapatkan pemberitahuan push di aplikasi Microsoft Authenticator, verifikasi bahwa mereka tidak diperlihatkan di bawah pengguna yang diblokir MFA seperti yang diuraikan dalam Memblokir dan membuka blokir [pengguna.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Jika pengguna tidak diblokir untuk MFA tetapi tidak menerima pemberitahuan push, mereka dapat membuka aplikasi Microsoft Authenticator, yang akan menarik permintaan persetujuan yang tertunda.
1. Sebagai metode masuk alternatif, pengguna juga bisa mengklik Masuk dengan cara lain dan memilih menggunakan kode verifikasi dari aplikasi seluler saya.
1. Aplikasi Microsoft Authenticator adalah satu-satunya metode yang tersedia untuk banyak pengguna. [Pelajari selengkapnya tentang default keamanan](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), lihat Authenticator FAQ [Aplikasi](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) untuk pertanyaan yang sering diajukan dan cara mengatasinya.
 
**Video yang Disarankan**

[Cara menyiapkan aplikasi Authenticator di telepon baru (2 menit).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
