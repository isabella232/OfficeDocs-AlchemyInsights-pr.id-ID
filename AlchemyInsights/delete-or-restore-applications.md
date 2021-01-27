---
title: Menghapus atau memulihkan aplikasi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014902"
---
# <a name="delete-or-restore-applications"></a>Menghapus atau memulihkan aplikasi

**Untuk menghapus aplikasi dari penyewa AZURE AD Anda**:

1. Di **portal AZURE AD**, pilih **aplikasi perusahaan**. Lalu temukan dan pilih aplikasi yang ingin Anda hapus.
2. Di bagian **Kelola** di panel kiri, pilih **properti**.
3. Pilih **Hapus**, lalu pilih **ya** untuk mengonfirmasi bahwa Anda ingin menghapus aplikasi dari penyewa Azure AD Anda.

Untuk informasi selengkapnya tentang cara menghapus aplikasi, lihat [mulai cepat: menghapus aplikasi dari penyewa Azure Active Directory (AZURE AD) Anda](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

Di PowerShell, cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) menghapus konfigurasi proksi aplikasi dari aplikasi tertentu di Azure Active Directory, dan dapat menghapus aplikasi sepenuhnya jika ditentukan.

Anda dapat **memulihkan aplikasi yang dihapus** menggunakan PowerShell. Setelah aplikasi yang ingin dipulihkan telah diidentifikasi, Anda dapat memulihkannya menggunakan [Pulihkan-Azureaddeletedapplikasi](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
