---
title: Batasan label sensitivitas untuk file Office di SharePoint dan OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813158"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Batasan label sensitivitas untuk file Office di SharePoint dan OneDrive

Ketika mengaktifkan label sensitivitas Office file di SharePoint dan OneDrive, berhati-hatilah terhadap persyaratan dan batasan, termasuk:

- SharePoint dan OneDrive tidak dapat memproses beberapa file berlabel dan dienkripsi dari aplikasi desktop Office bila file berisi data PowerQuery, data yang disimpan oleh add-in kustom, atau komponen XML kustom.
- SharePoint dan OneDrive tidak menerapkan label sensitivitas secara otomatis ke file yang sudah ada yang sudah Anda enkripsi menggunakan label Perlindungan Informasi Azure (AIP). Untuk menerapkan label sensitivitas ke file terenkripsi: 
    - Pastikan label AIP telah dimigrasikan dan diterbitkan ke Microsoft 365 Kepatuhan.
    - Unduh file berlabel, lalu unggah ke lokasi SharePoint atau OneDrive aslinya.
- Untuk dokumen terenkripsi, pencetakan tidak didukung.

Untuk detail tambahan tentang batasan, lihat [Mengaktifkan label sensitivitas untuk Office terkait SharePoint dan OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
