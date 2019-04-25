---
title: 646 cara mengkonfigurasi AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399774"
---
# <a name="configure-sync-features"></a><span data-ttu-id="43847-102">Mengkonfigurasi fitur sinkronisasi</span><span class="sxs-lookup"><span data-stu-id="43847-102">Configure sync features</span></span>

<span data-ttu-id="43847-103">Azure iklan Connect mencakup beberapa fitur yang diaktifkan secara default, atau bahwa Anda dapat mengaktifkan kemudian.</span><span class="sxs-lookup"><span data-stu-id="43847-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="43847-104">Beberapa fitur yang memerlukan konfigurasi tambahan di lingkungan tertentu.</span><span class="sxs-lookup"><span data-stu-id="43847-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="43847-105">Batas [menyaring](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objek disinkronisasi Azure iklan.</span><span class="sxs-lookup"><span data-stu-id="43847-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="43847-106">Secara default, semua pengguna, kontak, grup, dan Windows 10 komputer account disinkronisasi.</span><span class="sxs-lookup"><span data-stu-id="43847-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="43847-107">Anda dapat menyertakan atau mengecualikan benda-benda yang didasarkan pada domain, OUs, atau atribut lainnya.</span><span class="sxs-lookup"><span data-stu-id="43847-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="43847-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinkronisasi password hash dari Active Directory lokal Azure iklan.</span><span class="sxs-lookup"><span data-stu-id="43847-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="43847-109">Hal ini memungkinkan manajemen password di satu lokasi, tetapi menggunakan sandi yang sama di kedua lokal dan awan lingkungan.</span><span class="sxs-lookup"><span data-stu-id="43847-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="43847-110">Karena Active Directory sumber otoritatif, Anda dapat menggunakan kebijakan sandi Anda sendiri.</span><span class="sxs-lookup"><span data-stu-id="43847-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="43847-111">[Reset password swalayan (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) memungkinkan pengguna untuk membuat ulang sandi sendiri di Internet sementara masih menerapkan kebijakan sandi lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="43847-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="43847-112">[Perangkat writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) memungkinkan perangkat terdaftar di Azure iklan ditulis kembali ke Active Directory lokal sehingga mereka dapat digunakan untuk akses bersyarat.</span><span class="sxs-lookup"><span data-stu-id="43847-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="43847-113">[Mencegah disengaja menghapus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) diaktifkan secara default untuk membantu mencegah penghapusan simultan objek terlalu banyak (lebih dari 500 obyek per sinkronisasi).</span><span class="sxs-lookup"><span data-stu-id="43847-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="43847-114">Anda dapat mengubah pengaturan ini untuk memenuhi kebutuhan organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="43847-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="43847-115">[Upgrade otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) diaktifkan secara default untuk instalasi Check dan membantu memastikan Anda versi Azure iklan Connect selalu saat ini.</span><span class="sxs-lookup"><span data-stu-id="43847-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
