---
title: Sinkronisasi hash kata sandi untuk layanan domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177488"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="25fd3-102">Sinkronisasi hash kata sandi untuk layanan domain</span><span class="sxs-lookup"><span data-stu-id="25fd3-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="25fd3-103">**Jika instans Azure AD DS meminta Anda untuk mengaktifkan sinkronisasi hash kata sandi**</span><span class="sxs-lookup"><span data-stu-id="25fd3-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="25fd3-104">Anda menemukan skenario di mana Anda menjalankan lingkungan hibrid dengan pengguna yang melakukan sinkronisasi dari lingkungan Azure Active Directory Domain Services (AD DS) lokal.</span><span class="sxs-lookup"><span data-stu-id="25fd3-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="25fd3-105">Skenario ini terjadi meskipun Anda mengalami sinkronisasi hash kata sandi dari AD DS lokal ke penyewa Azure AD Anda.</span><span class="sxs-lookup"><span data-stu-id="25fd3-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="25fd3-106">**Kannya**</span><span class="sxs-lookup"><span data-stu-id="25fd3-106">**Cause**</span></span>

<span data-ttu-id="25fd3-107">Ini terjadi karena Azure AD Connect secara default tidak menyinkronkan warisan baru teknologi LAN Manager (NTLM) dan hash kata sandi Kerberos yang diperlukan untuk Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="25fd3-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="25fd3-108">**Solusi**</span><span class="sxs-lookup"><span data-stu-id="25fd3-108">**Workaround**</span></span> 

<span data-ttu-id="25fd3-109">Anda perlu mengonfigurasi Azure AD Connect untuk menyinkronkan hash kata sandi yang diperlukan untuk autentikasi NTLM dan Kerberos.</span><span class="sxs-lookup"><span data-stu-id="25fd3-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="25fd3-110">Setelah Azure AD Connect dikonfigurasikan, kejadian pembuatan di tempat atau perubahan kata sandi juga akan menyinkronkan hash kata sandi warisan ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="25fd3-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="25fd3-111">Silakan lihat di [sini](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) untuk informasi selengkapnya tentang hal ini dan untuk panduan tentang cara mengaktifkan sinkronisasi kata sandi di lingkungan HIBRID AZURE AD DS.</span><span class="sxs-lookup"><span data-stu-id="25fd3-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>