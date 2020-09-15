---
title: Menambahkan pengguna eksternal ke grup distribusi
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663516"
---
# <a name="add-external-users-to-a-distribution-group"></a>Menambahkan pengguna eksternal ke grup distribusi

Menambahkan kontak eksternal ke grup distribusi (DG) adalah proses dua langkah:
  
1. Membuat kontak email untuk pengguna eksternal:
    
    1. Di pusat admin, masuk ke halaman kontak **pengguna**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Pilih **Tambahkan kontak**.
    
    3. Ketikkan informasi untuk kontak Anda dan pilih **Tambahkan**.
    
2. Tambahkan kontak email ke DG Anda:
    
    1. Di pusat admin, masuk ke halaman grup **grup**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Temukan DG yang ingin Anda tambahkan ke pengguna eksternal, dan pilih untuk membuka dialog Edit.
    
    3. Pada tab **anggota** , pilih **Tampilkan semua dan Kelola anggota**. 
    
    4. Pilih **Tambahkan anggota**.
    
    5. Pilih kontak email yang Anda buat di langkah sebelumnya, lalu pilih **Simpan**.
    
Jika setelah mengikuti langkah-langkah ini, pengguna eksternal Anda tidak dapat mengirim email ke DG atau tidak menerima email darinya, mungkin DG ditandai agar hanya mengizinkan email dari pengguna internal. Anda dapat memeriksa konfigurasi ini dan memperbaikinya mengikuti petunjuk [di sini](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Catatan:** Instruksi ini tidak berlaku jika Tipe grup Anda adalah "grup Microsoft 365" dan bukan "grup distribusi." Jika demikian, Anda bisa menambahkan pengguna eksternal secara langsung ke grup dari Outlook. Informasi mendetail tentang grup Microsoft 365 serta instruksi untuk menambahkan tamu eksternal bisa ditemukan di [artikel ini](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  