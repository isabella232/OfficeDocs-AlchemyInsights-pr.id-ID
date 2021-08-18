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
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326675"
---
# <a name="did-your-users-receive-malicious-email"></a>Apakah pengguna Anda menerima email berbahaya?

Anda kini dapat melaporkan email berbahaya tersebut ke Microsoft [menggunakan Kiriman di portal Pertahanan Microsoft 365 .](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Pesan yang dikirim dalam [pengiriman admin dipindai,](https://security.microsoft.com/reportsubmission?viewid=admin) dan hasil berikut ini diperlihatkan dalam flyout detail:

- Jika terjadi kegagalan dalam autentikasi email pengirim pada saat pengiriman.
- Informasi tentang kebijakan terkait yang mungkin terpengaruh atau tertimpa putusan pesan.
- Hasil detonasi saat ini untuk melihat apakah URL atau file yang ada dalam pesan berbahaya atau tidak.
- Umpan balik dari pemberi nilai

Jika ditemukan timpaan, proses pemindaian ulang akan selesai dalam beberapa menit. Jika tidak ada masalah dalam autentikasi email atau jika pengiriman tidak terpengaruh oleh timpaan, umpan balik dari pemberi nilai dapat memakan waktu hingga satu hari.

Jika Anda tidak setuju dengan keputusan akhir pada pesan, URL atau file (diblokir vs. tidak diblokir), kirimkan pesan lagi setelah satu hari untuk pemindaian ulang. Kemungkinan besar, keputusan akan berubah setelah mengirimkan pesan kembali.

Sementara itu, Anda dapat menghapus email berbahaya dari kotak masuk pengguna dengan mengikuti petunjuk dalam [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Pelanggan dengan Pertahanan Microsoft untuk Office 365 dapat:
  - Menggunakan [Threat Explorer untuk Menemukan dan Menghapus Email mencurigakan](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Menggunakan Brankas Link untuk memblokir akses](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) ke URL berbahaya
  - Melacak pengguna yang mengklik dan mengakses URL berbahaya: [Tampilkan URL pengelabuan dan klik data penelusuran](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Memulai [Investigasi Otomatis secara manual](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Anda juga dapat melindungi dari file dan URL berbahaya dengan mengikuti instruksi dalam [Perlindungan dari URL dan file berbahaya](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
