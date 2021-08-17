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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102574"
---
# <a name="delete-or-restore-applications"></a>Menghapus atau memulihkan aplikasi

**Untuk menghapus aplikasi dari penyewa Azure AD:**

1. Di **portal Azure AD**, pilih **Aplikasi perusahaan**. Lalu cari dan pilih aplikasi yang ingin Anda hapus.
2. Di **bagian Kelola** di panel kiri, pilih **Properti**.
3. Pilih **Hapus**, lalu pilih **Ya** untuk mengonfirmasi bahwa Anda ingin menghapus aplikasi dari penyewa Azure AD.

Untuk informasi selengkapnya tentang cara menghapus aplikasi, lihat Mulai cepat: Menghapus aplikasi [dari penyewa Azure Active Directory (Azure AD) Anda.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

Di PowerShell, cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) menghapus konfigurasi Proksi Aplikasi dari aplikasi tertentu di Azure Active Directory, dan bisa menghapus aplikasi sepenuhnya jika ditentukan.

Anda bisa **memulihkan aplikasi yang dihapus** menggunakan PowerShell. Setelah aplikasi yang ingin dipulihkan telah diidentifikasi, Anda dapat memulihkannya menggunakan [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
