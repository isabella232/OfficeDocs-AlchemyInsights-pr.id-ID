---
title: Menambahkan pengguna eksternal ke grup distribusi
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737876"
---
# <a name="add-external-users-to-a-distribution-group"></a>Menambahkan pengguna eksternal ke grup distribusi

Menambahkan kontak eksternal ke grup distribusi (DG) adalah proses dua langkah:
  
1. Membuat kontak E-mail untuk pengguna eksternal:
    
    1. Di pusat admin, buka halaman[kontak](https://admin.microsoft.com/adminportal/home#/Contact) **pengguna** > . 
    
    2. Pilih **Tambah Kontak**.
    
    3. Ketik informasi kontak Anda dan pilih **Tambah**.
    
2. Tambahkan kontak E-mail ke DG Anda:
    
    1. Di pusat admin, buka[](https://admin.microsoft.com/adminportal/home#/groups)  >  **halaman grup grup**. 
    
    2. Temukan DG yang ingin Anda tambahkan pengguna eksternal, dan pilih untuk membuka dialog Edit.
    
    3. Pada tab **anggota** , pilih **Lihat semua dan Kelola anggota**. 
    
    4. Pilih **Tambahkan anggota**.
    
    5. Pilih kontak E-mail yang Anda buat di langkah sebelumnya, lalu pilih **Simpan**.
    
Jika setelah mengikuti langkah ini, pengguna eksternal tidak dapat mengirim email ke DG atau tidak menerima email darinya, bisa jadi DG ditandai hanya untuk mengizinkan email dari pengguna internal. Anda dapat memeriksa konfigurasi ini dan memperbaikinya mengikuti petunjuk [di sini](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Catatan:** Petunjuk ini tidak berlaku jika jenis grup Anda adalah "Office 365 grup" bukannya "grup distribusi." Jika demikian, Anda dapat menambahkan pengguna eksternal langsung ke grup dari Outlook. Informasi rinci tentang kantor 365 kelompok tamu serta petunjuk untuk menambahkan tamu eksternal dapat ditemukan di [artikel ini](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  