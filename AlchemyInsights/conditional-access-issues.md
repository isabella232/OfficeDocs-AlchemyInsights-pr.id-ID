---
title: Masalah akses bersyarat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014884"
---
# <a name="conditional-access-issues"></a>Masalah akses bersyarat

**Mengatasi masalah dengan diagnostik masuk**

Anda dapat dengan cepat menemukan apa yang terjadi atau mendiagnosis masalah terkait masuk pengguna dengan menggunakan [diagnostik masuk](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Luncurkan diagnostik masuk.
1. Temukan acara untuk dianalisis dengan memasukkan detail yang Anda miliki tentang pengguna, aplikasi, waktu masuk, id permintaan, atau id korelasi.
1. Tinjau hasil diagnostik yang memperlihatkan detail tentang apa yang terjadi dan tindakan apa yang bisa Anda lakukan untuk membuat perubahan (jika ada perubahan yang diperlukan).

**Langkah-langkah untuk memecahkan masalah masuk** 

1. Navigasikan ke halaman masuk Azure AD.
1. Memfilter masuk menurut pengguna, rentang waktu, aplikasi, status, aplikasi klien, dan seterusnya.
1. Pilih acara masuk dan Tampilkan Tab akses bersyarat untuk melihat kebijakan mana yang dievaluasi.
1. Klik pada baris kebijakan untuk menampilkan detail kebijakan dan memahami alasannya.

**Alat untuk memecahkan masalah kebijakan akses bersyarat**

- Mode hanya-laporan memungkinkan Anda mengevaluasi kebijakan tanpa memengaruhi pengguna.
- Alat apa-jika memungkinkan Anda mensimulasikan acara masuk dan melihat kebijakan mana yang berlaku.
- Insight dan buku kerja pelaporan menampilkan dampak waktu nyata dari setiap kebijakan.

**Kebijakan perlindungan garis dasar**

Kebijakan perlindungan garis dasar telah usang. Mereka tidak lagi diberlakukan dan akan segera dihapus dari Azure portal. Kami menyarankan untuk mengaktifkan [keamanan default](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Untuk informasi selengkapnya tentang akses bersyarat Lihat:

[Praktik terbaik untuk akses bersyarat di direktori](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 aktif Azure [Kondisi dalam akses bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrol dalam akses bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Lokasi dalam akses bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
