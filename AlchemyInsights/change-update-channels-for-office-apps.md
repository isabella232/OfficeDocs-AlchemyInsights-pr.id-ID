---
title: Mengubah saluran pembaruan untuk aplikasi Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439390"
---
# <a name="change-update-channels-for-office-apps"></a>Mengubah saluran pembaruan untuk aplikasi Office

Untuk penginstalan Office baru, gunakan pengaturan download perangkat lunak Office untuk memilih saluran pemutakhiran yang diinginkan, dan kemudian instal (atau instal ulang) aplikasi Office. Untuk informasi lebih lanjut, lihat [mengelola pengaturan download perangkat lunak di Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Catatan** Saluran pembaruan yang dipilih menggunakan setelan pengunduhan perangkat lunak Office berlaku untuk semua pengguna yang melakukan penginstalan baru menggunakan portal O365. Untuk informasi lebih lanjut, lihat [men-download dan menginstal atau menginstal ulang Microsoft 365 atau 2019 Office di PC atau Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Untuk instalasi Office yang ada, gunakan alat penyebaran Office (ODT) untuk beralih ke saluran pemutakhiran yang berbeda:  

1. Download versi terbaru dari alat penyebaran Office (setup.exe) dari [Microsoft download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Mengidentifikasi nama saluran yang ingin Anda Alihkan. Untuk informasi lebih lanjut, lihat [opsi konfigurasi untuk alat penyebaran Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Membuat file XML konfigurasi yang menentukan nama Channel yang sesuai, misalnya, update.xml.  
    J. <Configuration>  
    B. <pembaruan **saluran = "bulanan"** />  
    C. </Configuration>
4. Dari wantian perintah yang ditinggikan, beralih ke lokasi folder di mana setup.exe berada dan jalankan perintah berikut ini:  
    J. setup.exe/Configure update.xml
5. Mulai aplikasi Office (seperti Excel), dan kemudian pilih **berkas**  >  **akun**. Di bagian informasi produk, pilih pembaruan **opsi**pemutakhiran  >  **sekarang**.

Untuk informasi selengkapnya, lihat [bagaimana cara beralih saluran pembaruan untuk aplikasi Office yang sudah ada](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Untuk mengalihkan saluran pembaruan untuk grup pengguna yang dipilih atau dengan menggunakan Manajer konfigurasi (SCCM), konfigurasikan pengaturan Perbarui saluran menggunakan GPO. Untuk informasi lebih lanjut, lihat [Ikhtisar saluran pembaruan untuk Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Untuk detailnya, lihat [cara mengelola Office 365 ProPlus channels untuk profesional TI](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) dan [mengelola pembaruan untuk Microsoft 365 aplikasi dengan manajer konfigurasi titik akhir Microsoft](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).