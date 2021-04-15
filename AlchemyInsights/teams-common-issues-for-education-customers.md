---
title: Masalah umum Teams untuk pelanggan pendidikan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 893c8cacaf089932014ba7a3ea6122d17da38cdd
ms.sourcegitcommit: ef7ec42aba3c06aa8966dfac71cec18c08e7acf8
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/13/2021
ms.locfileid: "51692397"
---
# <a name="teams-common-issues-for-education-customers"></a>Masalah umum Teams untuk pelanggan pendidikan

**Untuk pelanggan pendidikan**:

Jika Anda memerlukan bantuan dalam menyebarkan Teams untuk mendukung pembelajaran jarak jauh, silakan kunjungi [Pusat FastTrack](https://www.microsoft.com/fasttrack) untuk mengajukan permintaan. Lihat masalah umum berikut untuk pelanggan pendidikan Teams:

- Melihat pesan "**Anda tidak dapat masuk!**"? Pastikan untuk [Mengaktifkan Microsoft Teams untuk Sekolah Anda](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Untuk penyewa EDU, Microsoft Teams tidak mengaktifkannya secara default; Anda harus mengaktifkannya terlebih dahulu.

- **Baru menggunakan Teams?** Tinjau [Pengajaran dan pembelajaran jarak jauh di Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) untuk mempelajari panduan terbaru tentang menyiapkan sekolah, rencana pembelajaran, rapat virtual, dan berbagi konten dengan para siswa.

- Setelah diaktifkan, pengguna dapat menjalankan Teams, baik dengan menginstal klien [desktop](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) dan [seluler](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) atau dari browser di https://teams.microsoft.com.

- **Aktifkan akses tamu Teams**: Tinjau [daftar periksa akses tamu Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) dan pastikan semua langkah sudah diselesaikan.
    - [Memahami Akses Tamu di Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Penyiapan – Daftar Periksa Akses Tamu Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Cara tamu bergabung di tim](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Dial-In dan Rapat Teams**: Butuh bantuan mengaktifkan atau menyiapkan Konferensi Audio di Microsoft Teams? Apakah pengguna ini baru dibuat? Jika demikian, Anda perlu menunggu 2 sampai 24 jam agar pengaturan mulai diterapkan. Untuk memverifikasi apakah pengguna memiliki lisensi Konferensi Audio dan memiliki Nomor Tol Default:
    1. Buka Pengguna Aktif lalu pilih pengguna yang dimaksud.
    2. Bergantung pada versi pusat admin, pilih **Lisensi dan Aplikasi** atau klik **Edit** pada **Lisensi produk**.
    3. Pastikan pengguna telah memilih lisensi untuk Konferensi Audio, Microsoft Teams, dan Skype for Business Online (Paket 2).
    4. Pengguna Pusat admin klik **Tampilkan semua** kemudian **Teams**.
    5. Di pusat admin Microsoft Teams, klik **Portal warisan**.
    6. Di pusat admin Skype for Business, klik **konferensi audio** kemudian **pengguna**.
    7. Pilih pengguna yang dimaksud dan verifikasi apakah pengguna tersebut memiliki Nomor Tol Default.

    Untuk informasi lebih lanjut, baca [Paket Panggilan Microsoft Teams](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) atau hubungi tim Penagihan Perniagaan Microsoft untuk mendapatkan bantuan terkait lisensi yang dimaksud.

    Sumber Daya Tambahan

    - [Rapat dan konferensi di Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Konferensi Audio](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Kebijakan Rapat**: Kebijakan rapat digunakan untuk mengontrol fitur yang tersedia bagi peserta rapat untuk rapat yang dijadwalkan oleh pengguna di organisasi Anda. Setelah membuat kebijakan dan perubahan, Anda dapat menetapkan pengguna pada kebijakan tersebut.

    - **Mengubah atau membuat kebijakan rapat**: Untuk mengubah atau membuat kebijakan rapat, buka **pusat admin Microsoft Teams > Rapat > Kebijakan Rapat**. Pilih kebijakan dari daftar atau klik **Tambahkan**. Jika membuat kebijakan baru, tambahkan nama dan deskripsi. Nama tidak boleh berisi karakter khusus atau lebih panjang dari 64 karakter. Pilih pengaturan Anda, lalu klik **Simpan**. 
    
        Misalnya, katakanlah Anda memiliki banyak pengguna dan ingin membatasi bandwidth yang akan diperlukan oleh rapat. Anda dapat membuat kebijakan kustom baru bernama "Bandwidth terbatas" dan menonaktifkan pengaturan berikut:

        Pada **Audio & video**:
        - Nonaktifkan **Izinkan perekaman awan**.
        - Nonaktifkan **Izinkan video IP**.

        Pada **Berbagi konten**:

        - Nonaktifkan mode berbagi layar.
        - Nonaktifkan **Izinkan whiteboard**.
        - Nonaktifkan **Izinkan catatan bersama**.

        Kemudian **tetapkan kebijakan pada pengguna**:

    1. Di navigasi sebelah kiri pusat admin Microsoft Teams, masuk ke **Pengguna**, lalu klik pengguna.
    2. Pilih pengguna dengan mengklik di bagian sebelah kiri nama pengguna, lalu klik **Edit pengaturan**.
    3. Di **Kebijakan rapat**, pilih kebijakan yang ingin Anda tetapkan, lalu klik **Terapkan**.

    Untuk menetapkan kebijakan pada beberapa pengguna sekaligus, lihat [Mengedit pengaturan pengguna Teams secara massal](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Atau Anda dapat melakukan hal berikut:
    1. Di navigasi sebelah kiri pusat admin Microsoft Teams, masuk ke **Rapat > Kebijakan rapat**.
    2. Pilih kebijakan dengan mengklik bagian sebelah kiri dari nama kebijakan.
    3. Klik **Kelola pengguna**.
    4. Di panel **Kelola pengguna**, cari pengguna berdasarkan nama tampilan atau nama pengguna, pilih nama, lalu klik **Tambahkan**. Ulangi langkah ini untuk setiap pengguna yang ingin ditambahkan.
    5. Setelah selesai menambahkan pengguna, klik **Simpan**.

- **Memecahkan masalah terkait tidak adanya papan angka**:
    - Pastikan bahwa pengguna memiliki [lisensi Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses) yang ditetapkan.
    - Pastikan bahwa pengguna memiliki [Paket Panggilan](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) yang ditetapkan.
    - Izinkan pengguna untuk mengakses [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Pemecahan masalah terkait masuk ke Teams**: Pertama, pastikan [layanan Microsoft Teams berfungsi dengan baik](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Kemudian periksa kode kesalahan umum dan tinjau [Mengapa saya mengalami masalah saat masuk ke Microsoft Teams](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)? Anda mungkin juga perlu meninjau [Model identitas dan autentikasi di Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
