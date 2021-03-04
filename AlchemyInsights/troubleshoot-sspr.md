---
title: Memecahkan masalah SSID
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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430211"
---
# <a name="troubleshoot-sspr"></a>Memecahkan masalah SSID

**Saya mengalami masalah saat mengonfigurasi penyetelan ulang kata sandi**

- Jika Anda administrator dan mencari cara untuk mengaktifkan penyetelan ulang kata sandi layanan mandiri, lihat [tutorial mengaktifkan SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), untuk mengonfigurasi pengaturan ulang kata sandi untuk organisasi Anda. Anda mungkin juga ingin meninjau [persyaratan lisensi](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Anda harus memiliki setidaknya satu lisensi yang ditetapkan di organisasi Anda.
    - **Pengguna awan saja** -SKU Office 365 (O365) berbayar apa pun, atau Azure AD Basic
    - **Pengguna awan dan/atau di** tempat-Azure AD Premium P1 atau P2, mobilitas perusahaan + keamanan (EMS), atau mengamankan perusahaan produktif (SPE)
- Untuk pertanyaan tambahan tentang pengaturan ulang kata sandi layanan mandiri, Tinjau [tanya jawab umum kami](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Saya mendapatkan pesan kesalahan**

Tinjau artikel ini untuk menemukan kesalahan umum dan solusinya: [memecahkan masalah penyetelan ulang kata sandi layanan mandiri](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saya mengalami masalah dengan kebijakan penyetelan ulang kata sandi**

- Jika kebijakan penyetelan ulang kata sandi tidak sesuai harapan, atau jika Anda memiliki pertanyaan tentang kebijakan penyetelan ulang kata sandi, lihat artikel ini: [kebijakan dan pembatasan kata sandi di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Kebijakan penyetelan ulang kata sandi tidak berlaku untuk administrator. Microsoft memberlakukan kebijakan penyetelan ulang kata sandi default yang kuat untuk setiap peran administrator Azure. Pastikan bahwa Anda menguji dengan pengguna yang bukan administrator. Untuk informasi selengkapnya tentang kebijakan tata ulang administrator, lihat artikel ini: [perbedaan kebijakan penyetelan ulang administrator](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Saya tidak ingin pengguna saya mendaftarkan Info keamanan tambahan untuk mereset kata sandi**

Anda bisa melakukan pra-isi data (email dan atribut telepon) untuk pengguna Anda menggunakan API, PowerShell, atau Azure AD Connect. Untuk mempelajari cara baca:

- [Menyebarkan penyetelan ulang kata sandi tanpa mengharuskan pengguna untuk mendaftar](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Data apa yang digunakan oleh reset kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saya ingin pengguna saya mendaftarkan Info keamanan tambahan untuk mereset kata sandi**

1. Minta pengguna Anda mendaftarkan Info keamanannya untuk pengaturan ulang kata sandi layanan mandiri dengan mengarahkan mereka ke [AKA.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Setelah data diisi untuk pengguna (oleh pengguna atau oleh admin), arahkan pengguna Anda ke [AKA.ms/sspr](https://passwordreset.microsoftonline.com/) sehingga pengguna Anda dapat diberdayakan untuk mereset kata sandi mereka sendiri.
1. Jika pengguna masih mengalami masalah, **kemungkinan besar pengguna menggabungkan atau** **hash kata sandi** . Ini berarti kemungkinan ada masalah dengan layanan tulis balik kata sandi.