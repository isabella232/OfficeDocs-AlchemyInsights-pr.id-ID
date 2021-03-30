---
title: Masalah rahasia klien pendaftaran aplikasi atau Sertifikat
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
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404785"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="ed2ee-102">Masalah rahasia klien pendaftaran aplikasi atau Sertifikat</span><span class="sxs-lookup"><span data-stu-id="ed2ee-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="ed2ee-103">Rahasia klien aplikasi kedaluwarsa?</span><span class="sxs-lookup"><span data-stu-id="ed2ee-103">Application client secret expiring?</span></span>

<span data-ttu-id="ed2ee-104">Terlepas dari bagaimana aplikasi terdaftar dibuat, baik melalui proses pendaftaran standar di portal Registrasi Aplikasi atau jika Prinsipal Layanan dibuat di penyewa Anda dengan menggunakan persetujuan aplikasi, Rahasia Klien baru harus dibuat sebelum kedaluwarsanya Aplikasi saat ini dan diperbarui dalam kode aplikasi yang terkait.</span><span class="sxs-lookup"><span data-stu-id="ed2ee-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="ed2ee-105">Periode validitas maksimum adalah 2 tahun.</span><span class="sxs-lookup"><span data-stu-id="ed2ee-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="ed2ee-106">Sebagai pengingat, nilai rahasia harus direkam karena tidak akan terlihat lagi setelah meninggalkan halaman Pendaftaran aplikasi di portal.</span><span class="sxs-lookup"><span data-stu-id="ed2ee-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="ed2ee-107">Untuk informasi selengkapnya, [lihat Mulai cepat: Mendaftarkan aplikasi di platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) dan Praktik terbaik untuk platform identitas [Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="ed2ee-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="ed2ee-108">Untuk mempelajari selengkapnya, [lihat Membuat aplikasi Azure AD & prinsipal layanan di portal - platform identitas Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="ed2ee-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
