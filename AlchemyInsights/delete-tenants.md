---
title: Hapus penyewa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993896"
---
# <a name="delete-tenant"></a>Hapus penyewa

Untuk menghapus Azure AD, pastikan:
- Anda adalah Administrator Global di direktori.
- Anda TIDAK masuk dengan akun yang memiliki direktori default seperti contoso.onmicrosoft.com masuk, seperti akun admin@contoso.onmicrosoft.com.
- Hapus setiap aplikasi aktif dalam direktori sebelum penghapusan. Untuk menghapus aplikasi aktif, navigasi ke Pendaftaran aplikasi dan hapus aplikasi yang sudah ada.
- Tidak ada langganan aktif untuk Layanan Online Microsoft apa pun, seperti Microsoft Azure, Office 365, atau Azure AD Premium terkait dalam direktori. Transfer langganan Anda atau percepat pembatalan langganan aktif melalui Dukungan dan Tagihan Azure. Pelajari selengkapnya tentang Cara Membatalkan Office 365 dan Azure. Untuk panduan tentang mengaitkan atau menambahkan langganan yang sudah ada ke penyewa, lihat Mengaitkan atau [menambahkan langganan Azure ke penyewa Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Tidak ada lisensi Aktif. Untuk menghapus lisensi, lihat [Cara menghapus Langganan untuk Menghapus lisensi.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Tidak ada pengguna aktif lain di direktori selain Anda sendiri sebagai Administrator Global saat mencoba menghapus Azure AD. Hapus pengguna aktif lainnya, dan dependensi apa pun pada nama domain kustom di penyewa juga harus dihapus, seperti pengguna yang dibuat dengan admin@contoso.com.

Untuk langkah detail selengkapnya tentang cara:
- Hapus "Azure Active Directory" atau "langganan", lihat [Menghapus Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Menghapus aplikasi di direktori, lihat [Menghapus Aplikasi.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
