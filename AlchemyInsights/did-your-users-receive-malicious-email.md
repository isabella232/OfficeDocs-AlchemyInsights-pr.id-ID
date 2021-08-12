---
title: Apakah pengguna Anda menerima email berbahaya
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929200"
---
# <a name="did-your-users-receive-malicious-email"></a>Apakah pengguna Anda menerima email berbahaya?

- Sekarang Anda dapat melaporkan email berbahaya tersebut ke Microsoft menggunakan [Pengumpulan Admin di Pusat Keamanan & Kepatuhan](https://sip.protection.office.com/reportsubmission).

Pesan yang dikirimkan di [pengumpulan admin](https://sip.protection.office.com/reportsubmission) dipindai, dan hasilnya akan ditampilkan di flyout **detail**:

- Jika terjadi kegagalan dalam autentikasi email pengirim pada saat pengiriman.
- Informasi tentang kebijakan terkait yang mungkin terpengaruh atau tertimpa putusan pesan.
- Hasil detonasi saat ini untuk melihat apakah URL atau file yang ada dalam pesan berbahaya atau tidak.
- Umpan balik dari pemberi nilai

Jika ditemukan timpaan, proses pemindaian ulang akan selesai dalam beberapa menit. Jika tidak ada masalah dalam autentikasi email atau jika pengiriman tidak terpengaruh oleh timpaan, umpan balik dari pemberi nilai dapat memakan waktu hingga satu hari.

Jika Anda tidak setuju dengan keputusan akhir pada pesan, URL atau file (diblokir vs. tidak diblokir), kirimkan pesan lagi setelah satu hari untuk pemindaian ulang. Kemungkinan besar, keputusan akan berubah setelah mengirimkan pesan kembali.

Sementara itu, Anda dapat menghapus email berbahaya dari kotak masuk pengguna dengan mengikuti petunjuk dalam [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Pelanggan dengan Pertahanan Microsoft untuk Office 365 dapat:
    - gunakan [Penjelajah Ancaman untuk Menemukan dan Menghapus email Berbahaya](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [menggunakan Link Aman untuk memblokir akses ](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) ke URL berbahaya
    - melacak pengguna yang mengklik dan mengakses URL berbahaya: [Menampilkan URL pengelabuan dan mengklik data keputusan](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - secara manual [mulai Penyelidikan Otomatis](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Anda juga dapat melindungi dari file dan URL berbahaya dengan mengikuti instruksi dalam [Perlindungan dari URL dan file berbahaya](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).