---
title: Memecahkan masalah SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038961"
---
# <a name="troubleshoot-sspr"></a>Memecahkan masalah SSPR

**Saya mengalami masalah saat mengonfigurasi pengaturan ulang kata sandi**

- Jika Anda administrator dan mencari cara mengaktifkan pengaturan ulang kata sandi mandiri, lihat Tutorial mengaktifkan [SSPR,](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)untuk mengonfigurasi pengaturan ulang kata sandi untuk organisasi Anda. Anda mungkin juga ingin meninjau [persyaratan lisensi.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Anda setidaknya harus memiliki satu lisensi yang ditetapkan di organisasi.
    - **Pengguna awan saja** - Semua Office 365 (O365) berbayar SKU, atau Azure AD Basic
    - **Pengguna lokal dan dan/atau** awan - Azure AD Premium P1 atau P2, Enterprise Mobility + Security (EMS), atau Secure Productive Enterprise (SPE)
- Untuk pertanyaan tambahan tentang pengaturan ulang kata sandi mandiri, tinjau [FAQ kami.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saya mendapatkan pesan kesalahan**

Tinjau artikel ini untuk menemukan kesalahan umum dan solusinya: [Memecahkan masalah pengaturan ulang kata sandi layanan mandiri](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saya mengalami masalah dengan kebijakan atur ulang kata sandi saya**

- Jika kebijakan pengaturan ulang kata sandi Anda tidak seperti yang diharapkan, atau jika Anda memiliki pertanyaan tentang kebijakan reset kata sandi, tinjau artikel ini: Kebijakan dan batasan kata sandi [di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Kebijakan reset kata sandi tidak berlaku untuk administrator. Microsoft memberlakukan kebijakan pengaturan ulang kata sandi dua pintu default yang kuat untuk setiap peran administrator Azure. Pastikan bahwa Anda melakukan pengujian dengan pengguna yang bukan administrator. Untuk informasi selengkapnya tentang kebijakan reset administrator, lihat artikel ini: [Administrator mereset perbedaan kebijakan](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Saya tidak ingin pengguna mendaftarkan informasi keamanan tambahan untuk pengaturan ulang kata sandi**

Anda dapat mengisi data (email dan atribut telepon) terlebih dahulu untuk pengguna menggunakan API, PowerShell, atau Azure AD Koneksi. Untuk mempelajari caranya dibaca:

- [Menyebarkan reset kata sandi tanpa mengharuskan pengguna untuk mendaftar](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Data apa yang digunakan oleh reset kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saya ingin pengguna saya mendaftarkan informasi keamanan tambahan mereka untuk pengaturan ulang kata sandi**

1. Meminta pengguna Anda mendaftarkan info keamanan mereka untuk mereset kata sandi layanan mandiri dengan mengarahkan mereka [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Setelah data diisi untuk pengguna (oleh pengguna atau oleh admin), [](https://passwordreset.microsoftonline.com/) arahkan pengguna Anda ke aka.ms/sspr sehingga pengguna Anda dapat diberdayakan untuk mengatur ulang kata sandi mereka sendiri.
1. Jika pengguna masih mengalami masalah, kemungkinan besar **pengguna** yang disinkronkan adalah pengguna gabungan atau **hash kata** sandi. Ini berarti kemungkinan ada masalah dengan layanan Password Writeback.