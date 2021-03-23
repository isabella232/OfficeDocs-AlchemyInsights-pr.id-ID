---
title: Saya mendapatkan diblokir oleh akses bersyarat dengan perangkat gabungan domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036700"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Saya mendapatkan diblokir oleh akses bersyarat dengan perangkat gabungan domain

**Alat yang sangat direkomendasikan**

[Alat pemecah masalah registrasi perangkat](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -alat yang membantu memecahkan masalah pendaftaran perangkat yang paling umum.

[Uji skrip konektivitas pendaftaran perangkat](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -skrip yang membantu memastikan bahwa perangkat bisa mengakses titik akhir pendaftaran perangkat di bawah akun sistem.

[Skrip pembersihan perangkat AZURE AD](https://github.com/mzmaili/AzureADDeviceCleanup) -skrip yang memungkinkan Anda mencari dan mengelola perangkat yang basi di lingkungan Anda.

Berikut adalah beberapa alasan umum mengapa akses bersyarat mungkin gagal menggunakan sebuah perangkat yang telah bergabung dalam domain (hibrid Azure AD).

1. **Tidak ada AZURE AD PRT di perangkat** -Anda harus memastikan bahwa perangkat tersebut memiliki token refresh utama Azure AD (PRT). Untuk informasi selengkapnya tentang PRT, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)ini.

Untuk memverifikasi apakah Anda memiliki Azure AD PRT, Anda bisa menjalankan `dsregcmd/status` perintah pada perangkat dan memverifikasi apakah "AzureAdPrt" sama dengan "ya".

Jika "AzureAdPrt" adalah "tidak", periksalah hal berikut ini:

- **Apakah Anda memiliki lingkungan gabungan dengan AD FS, dan tidak dapat dijangkau dari jaringan rumah pengguna Anda**: dalam hal ini, pastikan bahwa titik akhir "usernamemixhe" dapat diakses dari ekspor. Jika AD FS Anda berada di belakang VPN, pastikan pengguna tersambung ke VPN dan masuk kembali ke perangkat. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)ini.

- **Apakah TPM perangkat rusak dan dengan demikian tidak dapat mengotentikasi perangkat**: centang "TPM. MSC" untuk melihat apakah status TPM "sudah siap". Jika tidak, jalankan `dsregcmd/leave` dan biarkan perangkat bergabung kembali ke AZURE AD. Lalu, coba lagi. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)ini.

- **Anda menggunakan penyedia identitas pihak ketiga, yang tidak mendukung protokol WS-Trust**. Seperti yang diuraikan dalam dokumen kami, perangkat gabungan Azure AD yang digabungkan tidak dapat berfungsi dalam kasus ini. Silakan bekerja dengan penyedia identitas Anda untuk dukungan.

2. **Pengguna menggunakan browser Chrome tanpa akun Windows 10** atau **Chrome ekstensi Office tidak secara otomatis menggunakan PRT pada perangkat yang tergabung dengan AAD atau hibrid-AAD**: hal ini menyebabkan kegagalan setiap kebijakan akses bersyarat berbasis perangkat, dengan pesan kesalahan "perangkat tidak terdaftar" ditampilkan. Untuk menggunakan browser Chrome dengan benar, Anda harus menginstal "Akun Windows 10" atau "ekstensi Office ke browser Chrome pengguna" melalui SCCM atau Intune. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)ini.

Jika tidak memungkinkan untuk mendorong ekstensi dari jarak jauh, beri tahu pengguna untuk menginstal secara manual salah satu ekstensi di atas untuk mengakses aplikasi di balik akses bersyarat berbasis perangkat. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)ini.

3. **Perangkat telah bergabung dengan benar AZURE AD, namun tidak sengaja dihapus atau dinonaktifkan, baik karena sinkronisasi dengan perubahan di AZURE AD Connect atau dari portal Azure**: jika hal ini terjadi, objek perangkat tidak lagi dikenali sebagai perangkat yang bersambungan penuh meskipun status "Azureadjoin" dan "PRT" muncul sebagai valid pada perangkat.

Untuk memperbaiki masalah ini, jalankan `dsregcmd/leave` pada perangkat yang terpengaruh dan biarkan mereka bergabung kembali dengan AZURE AD. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)ini.

> [!NOTE]
> Jika perangkat Anda berada di Windows 10, pembaruan 1809, dengan proksi VPN/awan dan melihat masalah dengan status "AzureAdPrt" atau aplikasi apa pun dengan masalah SSO (Outlook tidak tersambung ke kotak surat meskipun Anda telah memiliki PRT), pastikan Anda memiliki patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) atau pembaruan kumulatif April [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) untuk mencegah kegagalan PRT pada mesin tersebut.

















