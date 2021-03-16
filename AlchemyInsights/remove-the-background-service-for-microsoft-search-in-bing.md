---
title: Menghapus layanan latar belakang untuk Microsoft Search di Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816202"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Menghapus layanan latar belakang untuk Microsoft Search di Bing

Untuk menghapus layanan latar belakang untuk Microsoft Search di Bing, Anda bisa mencoba solusi berikut:

1. Untuk kembali ke pengaturan mesin pencarian asli, lakukan hal berikut:

    untuk. Alihkan tombol **gunakan Bing sebagai mesin pencarian default Anda [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**.

    b. [Masuk ke Pusat admin Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) dan Kosongkan pengaturan yang memengaruhi semua pengguna di organisasi Anda.

2. Untuk menghapus layanan latar belakang dari perangkat individu, lakukan tugas-tugas berikut:

    untuk. Pilih program **> panel kontrol > program dan fitur**.

    b. Klik kanan **pencarian Microsoft di Bing** di bawah daftar program yang terinstal, lalu klik **hapus instalan**.

3. Untuk menghapus layanan latar belakang dari beberapa perangkat di organisasi Anda, masuk sebagai administrator dan jalankan perintah berikut dalam skrip: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
