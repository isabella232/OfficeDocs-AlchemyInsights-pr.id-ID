---
title: Masalah Pemilik Pendaftaran Aplikasi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951136"
---
# <a name="app-registration-owner-issues"></a>Masalah Pemilik Pendaftaran Aplikasi

Berikut adalah metode yang tersedia untuk menambahkan prinsipal sebagai pemilik bagi pendaftaran aplikasi:

- Menggunakan Modul PowerShell Azure AD -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referensi: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Menggunakan Azure CLI - `az ad app owner add`

    Referensi: [pemilik aplikasi az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Menggunakan MS Graph -

    Referensi: [Tambahkan pemilik - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Menggunakan Portal Azure AD - Navigasikan [ke portal.azure.com](https://portal.azure.com/) > Azure Active directory > Pendaftaran Aplikasi > Pilih aplikasi Anda > Pemilik > Tambahkan Pemilik

**Tidak dapat menampilkan aplikasi Anda di App Registrations blade meskipun Anda adalah pemilik aplikasi tersebut?**

Pemilik aplikasi bukanlah peran administratif. Jika pengaturan [Batasi akses ke portal administrasi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) diaktifkan, maka hanya admin yang dapat menampilkan aplikasi di portal Pendaftaran Aplikasi. Agar pemilik dapat menampilkan aplikasi, nonaktifkan pengaturan ini (Atur ke TIDAK) atau tetapkan peran admin ke pemilik hanya untuk aplikasi tertentu. Namun untuk hal ini, Anda akan memerlukan Azure AD Premium P2 baru dan mengaktifkan [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
