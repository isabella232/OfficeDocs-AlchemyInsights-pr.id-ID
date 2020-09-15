---
title: ATP untuk SharePoint, OneDrive, dan Microsoft teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715564"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP untuk SharePoint, OneDrive, dan Microsoft teams

Ikuti langkah-langkah ini untuk mengaktifkan proteksi ancaman tingkat lanjut:

1. Masuk ke [https://protection.office.com](https://protection.office.com) dan masuk dengan akun administrator global atau administrator keamanan.

2. Di panel navigasi kiri di bawah **manajemen ancaman**, pilih **Policy** \> **lampiran aman**kebijakan.

3. Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft teams**.

4. [Membuat kebijakan pemberitahuan aktivitas](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) untuk menerima pemberitahuan ketika kami mendeteksi file berbahaya.

Untuk instruksi lengkap, lihat [topik](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)ini.

**Catatan**: berdasarkan desain, ATP tidak memindai setiap file di SharePoint online, OneDrive for Business, atau Microsoft teams. File dipindai secara asinkron dengan proses yang menggunakan aktivitas berbagi, aktivitas tamu, dan sinyal ancaman untuk mengidentifikasi file berbahaya. Untuk informasi selengkapnya, lihat [topik](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)ini.
