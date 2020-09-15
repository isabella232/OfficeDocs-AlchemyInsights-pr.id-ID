---
title: 646 cara mengonfigurasi AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704492"
---
# <a name="configure-sync-features"></a><span data-ttu-id="2b79f-102">Mengonfigurasi fitur sinkronisasi</span><span class="sxs-lookup"><span data-stu-id="2b79f-102">Configure sync features</span></span>

<span data-ttu-id="2b79f-103">Azure AD Connect menyertakan beberapa fitur yang diaktifkan secara default, atau yang dapat Anda Aktifkan nanti.</span><span class="sxs-lookup"><span data-stu-id="2b79f-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="2b79f-104">Beberapa fitur memerlukan konfigurasi tambahan dalam lingkungan tertentu.</span><span class="sxs-lookup"><span data-stu-id="2b79f-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="2b79f-105">[Pemfilteran](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) membatasi objek disinkronkan ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2b79f-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="2b79f-106">Secara default, semua pengguna, kontak, grup, dan akun komputer Windows 10 disinkronisasi.</span><span class="sxs-lookup"><span data-stu-id="2b79f-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="2b79f-107">Anda bisa menyertakan atau mengecualikan objek berdasarkan domain, ou, atau atribut lainnya.</span><span class="sxs-lookup"><span data-stu-id="2b79f-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="2b79f-108">[Sinkronisasi hash kata](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sandi menyinkronkan hash kata sandi dari direktori aktif lokal ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2b79f-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="2b79f-109">Ini memungkinkan manajemen kata sandi dalam satu lokasi, tetapi penggunaan kata sandi yang sama di lingkungan lokal dan awan.</span><span class="sxs-lookup"><span data-stu-id="2b79f-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="2b79f-110">Karena direktori aktif adalah sumber otoritatif, Anda dapat menggunakan kebijakan kata sandi Anda sendiri.</span><span class="sxs-lookup"><span data-stu-id="2b79f-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="2b79f-111">[Reset kata sandi layanan mandiri (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) memungkinkan pengguna untuk mengatur ulang kata sandi mereka sendiri di awan saat masih menerapkan kebijakan kata sandi lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="2b79f-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="2b79f-112">[Alat tulis balik perangkat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) memungkinkan perangkat terdaftar di Azure AD untuk ditulis kembali ke direktori aktif di tempat sehingga dapat digunakan untuk akses bersyarat.</span><span class="sxs-lookup"><span data-stu-id="2b79f-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="2b79f-113">[Mencegah penghapusan disengaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) diaktifkan secara default untuk membantu mencegah terlalu banyak penghapusan objek bersamaan (lebih dari 500 objek per sinkronisasi).</span><span class="sxs-lookup"><span data-stu-id="2b79f-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="2b79f-114">Anda dapat mengubah pengaturan ini untuk memenuhi kebutuhan organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="2b79f-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="2b79f-115">[Pemutakhiran otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) diaktifkan secara default untuk penginstalan kilat dan membantu memastikan versi Azure AD Connect selalu terkini.</span><span class="sxs-lookup"><span data-stu-id="2b79f-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
