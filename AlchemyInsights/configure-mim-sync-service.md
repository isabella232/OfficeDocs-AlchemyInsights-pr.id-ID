---
title: Mengonfigurasi Layanan Sinkronisasi MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481872"
---
# <a name="configure-mim-sync-service"></a>Mengonfigurasi Layanan Sinkronisasi MIM

Layanan Sinkronisasi Microsoft Identity Manager (MIM) adalah komponen MIM. Ini adalah layanan terpusat di tempat yang menyimpan dan mengintegrasikan informasi untuk organisasi yang memiliki beberapa direktori dan database di tempat. Anda mungkin dapat mengatasi masalah dengan sinkronisasi MIM jika masalah telah diatasi dalam pembaruan terbaru untuk MIM atau merupakan salah satu masalah lain yang disebutkan di bawah ini.

**Langkah yang direkomendasikan**

1. Pastikan bahwa Anda menggunakan pembaruan terbaru MIM Sync dan periksa [catatan rilis MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) untuk menentukan apakah masalah telah diatasi dalam pembaruan.
2. Jika masalahnya dengan generik LDAP, Generic SQL, Lotus Domino atau Web Services Connector, pastikan bahwa Anda menggunakan pembaruan terbaru dari [konektor generik](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Jika MIM Sync-Run berhenti dengan kesalahan, lihat tabel [kode kesalahan Jalankan](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) untuk menentukan penyebab potensial.
4. Jika Jalankan perhentian dengan **ekstensi-dll-pengecualian**, lalu klik kata tersebut untuk membuka jendela **properti objek Ruang konektor** , dan klik pada **pelacakan stack...** untuk melihat informasi selengkapnya tentang penyebab utama, seperti yang diuraikan dalam [ekstensi-dll-pengecualian](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Jika komponen Layanan pemberitahuan Ubah kata sandi (PCNS) melaporkan **kesalahan 6025** dalam log kejadian selama sinkronisasi kata sandi, lihat panduan pemecahan masalah [pelaporan pcns kesalahan 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Jika sinkronisasi penuh dengan agen manajemen layanan FIM lambat, periksa pengaturan **otomatis tumbuh** untuk Code, seperti yang diuraikan dalam [pemecahan masalah sinkronisasi penuh Slow atau Hanging](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Jika Anda mengalami kesalahan server berhenti-dengan pembuatan yang gagal-melalui-Web-Services menggunakan agen manajemen layanan FIM, lihat [dukungan-Info: pembuatan gagal-melalui-web-layanan](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) untuk gambaran umum penyebab.

