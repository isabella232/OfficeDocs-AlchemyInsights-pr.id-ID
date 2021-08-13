---
title: Memecahkan masalah gabungan Hybrid Microsoft Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939274"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Memecahkan masalah gabungan Hybrid Microsoft Azure AD

Sangat Disarankan untuk Memastikan bahwa perangkat dapat mengakses titik akhir Pendaftaran Perangkat di bawah akun sistem dengan menggunakan [skrip Konektivitas Pendaftaran Perangkat Uji](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Jika Anda menyiapkan pendaftaran perangkat untuk pertama kalinya, pastikan untuk meninjau [Pengenalan manajemen perangkat di Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) untuk mempelajari cara mendapatkan perangkat di bawah kontrol Azure AD.
1. Jika Anda mendaftarkan perangkat ke Microsoft Azure AD secara langsung dan mendaftarkannya ke Intune, pastikan Anda telah [mengonfigurasi Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) dan memiliki [lisensinya](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) terlebih dahulu.
1. Pastikan Anda telah mendapatkan izin untuk melakukan operasi di Microsoft Azure AD dan AD lokal. Hanya administrator global di Microsoft Azure AD yang dapat mengelola pengaturan untuk pendaftaran perangkat. Selain itu, jika Anda menyiapkan pendaftaran otomatis di Active Directory lokal, Anda perlu menjadi administrator Active Directory dan AD FS (jika berlaku).

Untuk detail selengkapnya tentang mengatasi potensi masalah dengan gabungan Hibrid, lihat[Mengatasi Masalah Gabungan Hibrid](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) dan untuk menyiapkan hibrid Azure AD yang tergabung serta Mengelola Perangkat menggunakan portal Microsoft Azure AD, lihat[Menyiapkan perangkat gabungan hibrid Microsoft Azure AD (bergabung dengan domain lokal)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) dan [Mengelola perangkat menggunakan portal Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Untuk mengatasi masalah umum dengan gabungan Hibrid Azure Active Directory (AD), lihat [FAQ gabungan Hibrid Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
