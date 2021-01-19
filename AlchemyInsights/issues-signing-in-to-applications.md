---
title: Masalah saat masuk ke aplikasi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901031"
---
# <a name="issues-signing-in-to-applications"></a>Masalah saat masuk ke aplikasi

Untuk mendeteksi penyebab atau mendiagnosis masalah yang terkait dengan masuk pengguna, lakukan langkah-langkah berikut:

1. Luncurkan [diagnostik masuk](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Temukan acara untuk dianalisis dengan memasukkan detail yang Anda miliki tentang pengguna, aplikasi, waktu masuk, meminta id, atau id korelasi.
3. Tinjau hasil diagnostik yang memperlihatkan detail tentang apa yang terjadi dan tindakan apa yang bisa Anda lakukan untuk membuat perubahan, jika ada perubahan yang diperlukan.

Berikut ini adalah beberapa masalah umum yang mungkin Anda alami saat masuk ke aplikasi:

1. Anda atau pengguna **telah menyelesaikan masuk AZURE AD, tapi melihat prompt yang tidak diharapkan** -Lihat artikel permintaan persetujuan yang tidak [diharapkan saat masuk ke aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) dan kesalahan yang tidak [terduga saat melakukan persetujuan ke aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Anda atau pengguna **telah masuk ke aplikasi secara langsung, namun tidak dapat masuk ke aplikasi tersebut dari deeplink pada portal kustom atau panel akses**: Lihat [memecahkan masalah masuk ke aplikasi dari Azure AD aplikasi saya](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Anda atau pengguna **telah menyelesaikan masuk AZURE AD, tetapi aplikasi menampilkan pesan kesalahan dan tidak memperbolehkan pengguna menyelesaikan aliran masuk**: masalahnya adalah aplikasi tidak menerima respons yang dikeluarkan oleh Azure AD. Ikuti [langkah-langkah ini](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) untuk memecahkan masalah.
4. Anda atau pengguna **tidak bisa masuk ke aplikasi non-galeri yang dikonfigurasi untuk masuk tunggal kata sandi**: ikuti panduan dalam [langkah-langkah ini](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) untuk memecahkan masalah.
5. Anda atau pengguna **tidak bisa masuk ke aplikasi Galeri AZURE AD yang dikonfigurasikan untuk masuk tunggal kata sandi**: Ikuti langkah- [langkah ini](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) untuk memecahkan masalah.
6. Anda atau pengguna **tidak bisa masuk ke aplikasi Microsoft**: Ikuti [langkah-langkah ini](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) untuk memecahkan masalah.
7. Anda atau pengguna **tidak bisa masuk ke aplikasi non-galeri yang dikonfigurasi untuk gabungan Single masuk**: Ikuti [langkah-langkah ini](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) untuk memecahkan masalah.
8. Anda atau pengguna **tidak bisa masuk ke aplikasi Galeri AZURE AD yang dikonfigurasikan untuk masuk tunggal gabungan**: Ikuti [langkah-langkah ini](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) untuk memecahkan masalah.
9. Anda atau pengguna **tidak bisa masuk ke aplikasi yang dikembangkan kustom**: Ikuti langkah- [langkah ini](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) untuk memecahkan masalah.
10. Anda atau pengguna **tidak dapat masuk ke aplikasi lokal menggunakan proksi aplikasi AZURE AD**: Ikuti [langkah-langkah ini](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) untuk memecahkan masalah.

