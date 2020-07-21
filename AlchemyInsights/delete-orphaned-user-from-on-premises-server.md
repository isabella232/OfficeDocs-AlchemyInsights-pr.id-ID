---
title: Menghapus pengguna yatim piatu dari server lokal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198182"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Menghapus pengguna yatim piatu dari server lokal

Untuk menghapus pengguna yang ditinggalkan, ikuti langkah berikut:

1. Memaksa sinkronisasi direktori dengan mengikuti petunjuk dalam [apa yang hibrid identitas dengan Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Untuk memverifikasi sinkronisasi direktori, lihat [apa yang dimaksud dengan identitas hibrid dengan Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Jika fungsi sinkronisasi dengan benar tetapi penghapusan objek direktori aktif tidak dialihkan ke Azure AD, secara manual menghapus objek ditinggalkan dengan menggunakan salah satu dari cmdlets Azure Active Directory modul untuk Windows PowerShell berikut ini:

    Hapus-MsolContact  
    Hapus-MsolGroup  
    Hapus-MsolUser

    Misalnya, untuk menghapus ditinggalkan ID pengguna john.smith@contoso.com, awalnya dibuat dengan menggunakan sinkronisasi direktori, Jalankan cmdlet:

    Hapus-MsolUser-UserPrincipalName John.Smith@Contoso.com