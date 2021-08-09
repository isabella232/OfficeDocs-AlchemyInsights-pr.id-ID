---
title: Menambahkan pengguna eksternal ke Grup Distribusi
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934836"
---
# <a name="add-external-users-to-a-distribution-group"></a>Menambahkan pengguna eksternal ke Grup Distribusi

Proses menambahkan kontak eksternal ke Grup Distribusi (DG) adalah dua langkah:
  
1. Membuat Kontak Email untuk pengguna eksternal:
    
    1. Di pusat admin, masuk ke **halaman**  >  [Kontak](https://admin.microsoft.com/adminportal/home#/Contact) Pengguna. 
    
    2. Pilih **Tambahkan kontak.**
    
    3. Ketikkan informasi untuk kontak Anda dan pilih **Tambahkan.**
    
2. Menambahkan Kontak Email ke DG Anda:
    
    1. Di pusat admin, masuk ke **halaman**  >  [Grup](https://admin.microsoft.com/adminportal/home#/groups) Grup. 
    
    2. Temukan DG tempat Anda ingin menambahkan pengguna eksternal, dan pilih untuk membuka dialog edit.
    
    3. Pada tab **Anggota,** pilih Tampilkan **semua dan kelola anggota**. 
    
    4. Pilih **Tambahkan anggota.**
    
    5. Pilih Kontak Email yang telah Anda buat pada langkah sebelumnya, lalu pilih **Simpan**.
    
Jika setelah mengikuti langkah-langkah ini pengguna eksternal tidak dapat mengirim email ke DG atau tidak menerima email, mungkin DG ditandai untuk hanya mengizinkan email dari pengguna internal. Anda dapat memeriksa konfigurasi ini dan memperbaikinya dengan mengikuti petunjuk di [sini](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Catatan:** Instruksi ini tidak berlaku jika tipe grup Anda adalah "grup Microsoft 365" bukan "Grup distribusi." Jika demikian, Anda bisa menambahkan pengguna eksternal secara langsung ke grup dari Outlook. Informasi mendetail tentang Microsoft 365 Grup Grup serta instruksi untuk menambahkan tamu eksternal dapat ditemukan di [artikel ini.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  