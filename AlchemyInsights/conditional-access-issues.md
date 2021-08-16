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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069967"
---
# <a name="conditional-access-issues"></a>Masalah akses bersyarat

**Mengatasi masalah dengan Diagnostik Masuk**

Anda bisa dengan cepat mencari tahu apa yang terjadi atau mendiagnosis masalah yang terkait dengan masuknya [pengguna dengan menggunakan Diagnostik Masuk:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Luncurkan Diagnostik Masuk.
1. Temukan kegiatan yang akan dianalisis dengan memasukkan detail yang Anda miliki tentang pengguna, aplikasi, waktu masuk, ID permintaan, atau ID korelasi.
1. Tinjau hasil diagnostik yang memperlihatkan detail tentang apa yang terjadi dan tindakan apa yang dapat Anda lakukan untuk membuat perubahan (jika diperlukan perubahan).

**Langkah-langkah untuk Memecahkan Masalah Masuk** 

1. Navigasi ke halaman Masuk Azure AD.
1. Memfilter masuk menurut pengguna, rentang waktu, aplikasi, status, aplikasi klien, dan sebagainya.
1. Pilih acara masuk dan lihat tab Akses Kondisional untuk melihat kebijakan mana yang dievaluasi.
1. Klik baris kebijakan untuk menampilkan detail kebijakan dan memahami mengapa kebijakan tersebut diterapkan.

**Alat untuk memecahkan masalah kebijakan Akses Kondisional**

- Mode laporan saja memungkinkan Anda mengevaluasi kebijakan tanpa memengaruhi pengguna.
- Alat bagaimana-jika memungkinkan Anda mensimulasikan acara masuk dan melihat kebijakan mana yang berlaku.
- Insights kerja pelaporan dan pelaporan menampilkan dampak real-time dari setiap kebijakan.

**Kebijakan Proteksi Garis Dasar**

Kebijakan Proteksi Garis Dasar telah ditolak. Fitur tersebut tidak lagi diterapkan dan akan segera dihapus dari portal Azure. Kami menyarankan untuk [mengaktifkan default keamanan](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Untuk informasi selengkapnya tentang Akses Bersyarat, lihat:

[Praktik terbaik untuk akses bersyarat di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kondisi dalam Akses Bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrol dalam Akses Bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Lokasi dalam Akses Bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
