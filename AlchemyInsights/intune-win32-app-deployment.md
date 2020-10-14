---
title: Penggunaan aplikasi Win32 Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461871"
---
# <a name="intune-win32-app-deployment"></a>Penggunaan aplikasi Win32 Win32

Microsoft Intune memperbolehkan aplikasi Win32, termasuk tetapi tidak terbatas pada MSI dan. EXE akan disebarkan ke perangkat Windows 10. Mekanisme penyebaran yang digunakan memerlukan ekstensi manajemen Intune (IME) untuk hadir pada perangkat target. IME akan diinstal secara otomatis sebagai hasil dari menargetkan skrip PowerShell atau penerapan aplikasi Win32 ke pengguna/perangkat.

Ada juga rangkaian prasyarat yang harus dipenuhi untuk menyebarkan aplikasi Win32 yang meliputi:

- Platform yang didukung: Windows 10 versi 1607 atau yang lebih baru (versi Enterprise, Pro, dan pendidikan).
- Arsitektur yang didukung: x86 dan x64.
- Manajemen perangkat: AAD bergabung dan didaftarkan secara otomatis (termasuk domain hibrid bergabung dan kebijakan grup didaftarkan secara otomatis).
- Format paket aplikasi:. file **intunewin**  disiapkan oleh [alat penyiapan konten Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Terbatas
    - Ukuran maksimum: 8GB.
    - Arsitektur tidak didukung: ARMs.

Tinjau dokumen "[Tambahkan, tetapkan, dan Pantau aplikasi Win32 di Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" untuk informasi yang terkait dengan langkah-langkah tersebut.

Detail tentang pemecahan masalah penyebaran aplikasi di Windows termasuk aplikasi Win32 dapat ditinjau dalam dokumen berikut

- [Memecahkan masalah penginstalan aplikasi](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Memecahkan masalah aplikasi Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)