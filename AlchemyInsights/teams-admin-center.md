---
title: Pusat Admin Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049347"
---
# <a name="teams-admin-center"></a>Pusat Admin Teams

Pelajari tentang mengelola Teams dengan [Pusat Admin Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Jika tidak dapat mengakses Pusat Admin Teams, lihat item berikut:

- Verifikasikan bahwa Anda telah memperbolehkan [alamat IP dan URL Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) yang sesuai pada perangkat perimeter apa pun (firewall, dll.) atau di aturan firewall pada komputer lokal.
- Verifikasikan bahwa data masuk yang Anda gunakan untuk mengakses Portal Admin Teams sesuai dengan nama pengguna yang tercantum di [portal Admin Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Jika pengguna tidak muncul di Pusat Admin Teams, lihat item berikut:

- Apakah Anda membuat pengguna atau menetapkan lisensi dalam 24 jam terakhir? Pastikan Anda menunggu setidaknya 24 jam sebelum membuka tiket dukungan.
- Pastikan Anda menetapkan lisensi yang sesuai?
- Jika memiliki Direktori Aktif lokal, verifikasi bahwa nilai [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) atau alamat SIP di bidang ProxyAddresses dalam Direktori Aktif lokal berformat unik dan formatnya sesuai dengan **sip:** Nama pengguna dari [pusat admin Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Jika ingin mempertahankan Skype for Business Server dan mengatur pengguna agar berada di tempat dan Online: ikuti "Menyiapkan hibrid dengan Teams dan **Skype for Business Online"** di Panel Kontrol Skype for Business Server dan memindahkan pengguna Secara Online.
