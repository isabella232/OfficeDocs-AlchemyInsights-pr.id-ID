---
title: Menguji Konfigurasi IRM untuk kapabilitas OME baru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812438"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Menguji Konfigurasi IRM untuk kapabilitas OME baru

Untuk memverifikasi bahwa Microsoft 365 baru Anda dikonfigurasi untuk menggunakan kapabilitas OME baru, jalankan cmdlet berikut saat tersambung [ke Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell):


1. Periksa konfigurasi IRM penyewa Anda dengan menjalankan `Get-IRMConfiguration` . Pastikan nilai ini diatur ke **True:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Menggunakan domain, alamat pengirim, dan penerima, jalankan `Test-IRMConfiguration` . Jika pengujian tidak berhasil, selidiki konfigurasi IRM Anda.

Untuk informasi selengkapnya tentang cara memverifikasi konfigurasi IRM, lihat [Memverifikasi konfigurasi OME baru Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).