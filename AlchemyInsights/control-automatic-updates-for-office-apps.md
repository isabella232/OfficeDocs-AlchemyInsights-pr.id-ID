---
title: Mengontrol pembaruan otomatis untuk aplikasi Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439334"
---
# <a name="control-automatic-updates-for-office-apps"></a>Mengontrol pembaruan otomatis untuk aplikasi Office

Secara default, pembaruan untuk aplikasi Office diunduh secara otomatis dan diterapkan di latar belakang tanpa campur tangan pengguna. Namun, administrator dapat mengontrol cara pemutakhiran diterapkan dengan menggunakan pengaturan pemutakhiran Office. Pengaturan pembaruan memungkinkan administrator untuk mengaktifkan atau menonaktifkan pembaruan otomatis, menampilkan atau menyembunyikan tombol **Perbarui sekarang** di Office, mengatur tenggat waktu pembaruan, dan banyak lagi. Untuk informasi selengkapnya, lihat:

- [Mengkonfigurasi pengaturan pembaruan untuk Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Pembaruan otomatis untuk Office tidak diaktifkan](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Menentukan bagaimana Office diperbarui setelah diinstal](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Untuk meninjau pengaturan pembaruan yang sudah ada yang diterapkan ke mesin klien, ikuti langkah berikut:

1. Buka Registry Editor dengan pergi untuk **mulai**  >  **menjalankan**  >  **regedit**.
2. Beralih ke lokasi berikut dan Tinjau pengaturan pembaruan Office:  
    J. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    B. ClickToRun\Configuration

**Catatan**  Jika kunci officemgmtcom diatur, Anda mungkin melihat pesan "pembaruan dikelola oleh administrator sistem Anda" di **Office**  >  **account**  >  **Office update**. Untuk informasi lebih lanjut, lihat [mengelola pembaruan untuk microsoft 365 aplikasi dengan Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  