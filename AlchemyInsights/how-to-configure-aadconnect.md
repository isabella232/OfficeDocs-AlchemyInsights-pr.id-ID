---
title: 646 cara mengkonfigurasi AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722563"
---
# <a name="configure-sync-features"></a><span data-ttu-id="6c8d5-102">Mengkonfigurasi fitur sinkronisasi</span><span class="sxs-lookup"><span data-stu-id="6c8d5-102">Configure sync features</span></span>

<span data-ttu-id="6c8d5-103">Azure AD menyambung mencakup beberapa fitur yang diaktifkan secara default, atau bahwa Anda dapat mengaktifkan kemudian.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="6c8d5-104">Beberapa fitur memerlukan konfigurasi tambahan di lingkungan tertentu.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="6c8d5-105">[Penyaringan](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) membatasi objek disinkronkan ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="6c8d5-106">Secara default, semua pengguna, kontak, grup, dan akun komputer Windows 10 disinkronkan.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="6c8d5-107">Anda dapat menyertakan atau mengecualikan objek berdasarkan domain, ou, atau atribut lainnya.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="6c8d5-108">[Sinkronisasi hash sandi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) menyinkronkan hash sandi dari Active Directory lokal ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="6c8d5-109">Hal ini memungkinkan pengelolaan sandi di satu lokasi, namun menggunakan sandi yang sama di lingkungan lokal dan Cloud.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="6c8d5-110">Karena Active Directory adalah sumber otoritatif, Anda dapat menggunakan kebijakan sandi Anda sendiri.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="6c8d5-111">[Pengaturan ulang kata sandi layanan mandiri (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) memungkinkan pengguna menyetel ulang sandi mereka di Cloud saat masih menerapkan kebijakan sandi lokal.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="6c8d5-112">[Perangkat tulis balik](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) memungkinkan perangkat terdaftar di Azure AD untuk ditulis kembali ke direktori aktif di tempat sehingga mereka dapat digunakan untuk akses bersyarat.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="6c8d5-113">[Mencegah menghapus disengaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) diaktifkan secara default untuk membantu mencegah terlalu banyak penghapusan objek simultan (lebih dari 500 objek per sinkronisasi).</span><span class="sxs-lookup"><span data-stu-id="6c8d5-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="6c8d5-114">Anda dapat mengubah pengaturan ini untuk memenuhi kebutuhan organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="6c8d5-115">[Peningkatan otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) diaktifkan secara default untuk instalasi Ekspres dan membantu memastikan bahwa versi Azure AD Connect selalu terkini.</span><span class="sxs-lookup"><span data-stu-id="6c8d5-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
