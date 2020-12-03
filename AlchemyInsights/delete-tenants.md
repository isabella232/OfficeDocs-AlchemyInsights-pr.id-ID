---
title: Menghapus penyewa
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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564618"
---
# <a name="delete-tenant"></a>Menghapus penyewa

Untuk menghapus Azure AD, pastikan:
- Anda adalah administrator global di direktori.
- Anda tidak masuk dengan akun yang memiliki direktori default seperti contoso.onmicrosoft.com dalam akun masuk, seperti admin@contoso.onmicrosoft.com.
- Hapus semua aplikasi aktif dalam direktori sebelum penghapusan. Untuk menghapus aplikasi aktif, navigasikan ke pendaftaran aplikasi dan Hapus aplikasi yang sudah ada.
- Tidak ada langganan aktif untuk layanan online Microsoft apa pun, seperti Microsoft Azure, Office 365 atau Azure AD premium yang terkait pada direktori. Mentransfer langganan atau mempercepat pembatalan langganan aktif melalui dukungan dan tagihan Azure. Pelajari selengkapnya tentang cara membatalkan langganan Office 365 dan Azure. Untuk panduan tentang mengaitkan atau menambahkan langganan yang sudah ada ke penyewa, lihat [mengaitkan atau menambahkan langganan Azure ke penyewa AZURE AD Anda](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Tidak ada lisensi aktif. Untuk menghapus lisensi, lihat [cara menghapus langganan untuk menghapus lisensi](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Tidak ada pengguna aktif lainnya dalam direktori selain diri Anda sebagai administrator global saat mencoba menghapus Azure AD. Menghapus pengguna aktif lainnya, dan setiap dependensi pada nama domain kustom dalam penyewa juga harus dihapus, seperti pengguna yang dibuat dengan admin@contoso.com.

Untuk langkah detail selengkapnya tentang cara:
- Hapus "Azure Active Directory" atau "langganan", lihat [menghapus direktori Azure Active](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Menghapus aplikasi dalam direktori, lihat [menghapus aplikasi](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
