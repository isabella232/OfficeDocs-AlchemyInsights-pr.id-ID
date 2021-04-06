---
title: Identifikasi masalah Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595851"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identifikasi masalah Windows Virtual Desktop

Diagnostik Desktop Virtual Windows hanya menggunakan satu cmdlet PowerShell tetapi berisi banyak parameter opsional untuk membantu mempersempit dan mengisolasi masalah. Untuk memulai: 

1. Unduh dan impor modul Windows Virtual Desktop PowerShell. Untuk detailnya, [lihat Cmdlet Desktop Virtual Windows untuk Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Jalankan cmdlet berikut untuk masuk ke akun Anda:
    
    Contoh: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**CATATAN:** Semua kueri yang menggunakan PowerShell harus menyertakan parameter -UserName atau -ActivityID. Untuk kemampuan pemantauan, lihat [Menggunakan Analitik Log untuk fitur diagnostik](https://go.microsoft.com/fwlink/?linkid=2126847).

Untuk memfilter aktivitas diagnostik menurut pengguna, jalankan cmdlet berikut:

Contoh: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Terdapat daftar filter yang dapat Anda jalankan untuk mendiagnosis masalah. Untuk mempelajari selengkapnya tentang mendiagnosis masalah, lihat [Mengidentifikasi dan mendiagnosis masalah Windows Virtual Desktop](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Untuk mempelajari selengkapnya tentang kesalahan umum, [lihat Kesalahan umum sens](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
