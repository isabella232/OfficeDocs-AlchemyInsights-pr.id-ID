---
title: Mengonfigurasi titik koneksi Layanan (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036144"
---
# <a name="configure-service-connection-point-scp"></a>Mengonfigurasi titik koneksi Layanan (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Alasan**: tidak dapat membaca objek SCP dan mendapatkan informasi penyewa Azure AD
- **Resolusi**: rujuk ke bagian [mengonfigurasi titik koneksi Layanan](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Rencana tindakan**

- Periksa apakah perangkat telah menerima GPO untuk validasi terkendali.
- Pastikan bahwa GPO telah membuat kunci registri.
- Pastikan Anda memiliki 2 tombol yang dibuat dengan ID direktori Anda dan domain onmicrosoft.

**Mengonfigurasi pengaturan registri sisi klien untuk SCP**

Gunakan contoh berikut untuk membuat objek kebijakan grup (GPO) untuk menggunakan pengaturan registri yang mengonfigurasi entri SCP dalam registri perangkat Anda.

1. Buka konsol manajemen kebijakan grup dan buat GPO baru di domain Anda.
     - Berikan nama GPO yang baru Anda buat (misalnya, ClientSideSCP)

2. Edit GPO dan temukan jalur berikut: **pengaturan > konfigurasi komputer > pengaturan Windows > Registry**.

3. Klik kanan **Registry** dan pilih **item baru > Registry**.

4. Pada tab **umum** , konfigurasikan yang berikut ini:
  
- **Tindakan**: Perbarui
    
- **Sarang**: HKEY_LOCAL_MACHINE
    
- **Jalur kunci**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Nama nilai**: tenantid
    
- **Tipe nilai**: REG_SZ
    
- **Data nilai**: id direktori atau GUID dari contoh Azure AD Anda (nilai ini bisa ditemukan di **portal Azure > direktori aktif azure > properti > id direktori**)
 
- Klik **OK**.
 
5. Klik kanan **Registry** dan pilih **item baru > Registry**.

6. Pada tab **umum** , konfigurasikan yang berikut ini:
  
- **Tindakan**: Perbarui
    
- **Sarang**: HKEY_LOCAL_MACHINE
    
- **Jalur kunci**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Nama nilai**: tenantname
    
- **Tipe nilai**: REG_SZ
    
- **Data nilai**: nama domain Anda yang diverifikasi jika Anda menggunakan lingkungan gabungan seperti AD FS. Nama domain Anda yang diverifikasi atau nama domain onmicrosoft.com Anda (misalnya, contoso. onmicrosoft). com jika Anda menggunakan lingkungan terkelola

- Klik **OK**.

7. Tutup editor untuk GPO yang baru dibuat.

8. Tautkan GPO yang baru dibuat ke ou yang diinginkan yang berisi komputer gabungan domain yang menjadi bagian dari populasi peluncuran yang terkontrol.

Untuk informasi selengkapnya, lihat [validasi terkontrol hibrid AZURE AD Join-AZURE AD | Dokumen Microsoft](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) dan  [pemecahan masalah hibrid perangkat gabungan Azure Active Directory | Dokumen Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









