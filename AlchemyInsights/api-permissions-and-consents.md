---
title: Izin dan izin API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974607"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="6a801-102">Izin dan izin API</span><span class="sxs-lookup"><span data-stu-id="6a801-102">API permissions and consent</span></span>

<span data-ttu-id="6a801-103">Aplikasi yang terintegrasi dengan platform Microsoft Identity ikuti model otorisasi yang memberi pengguna dan administrator kontrol atas bagaimana data bisa diakses.</span><span class="sxs-lookup"><span data-stu-id="6a801-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="6a801-104">Penerapan model otorisasi telah diperbarui pada titik akhir platform identitas Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6a801-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="6a801-105">Mengubah cara aplikasi harus berinteraksi dengan platform identitas Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6a801-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="6a801-106">[Izin dan persetujuan di titik akhir platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) membahas konsep dasar model otorisasi ini, termasuk lingkup, izin, dan persetujuan.</span><span class="sxs-lookup"><span data-stu-id="6a801-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="6a801-107">[Kerangka izin Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) memudahkan untuk mengembangkan multi-penyewa web dan aplikasi klien asli.</span><span class="sxs-lookup"><span data-stu-id="6a801-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="6a801-108">Aplikasi ini memperbolehkan masuk dengan akun pengguna dari penyewa Azure AD yang berbeda dari aplikasi yang didaftarkan.</span><span class="sxs-lookup"><span data-stu-id="6a801-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="6a801-109">Mereka juga mungkin perlu mengakses api web seperti API Microsoft graph (untuk mengakses Azure AD, Intune, dan Services di Microsoft 365) dan api layanan Microsoft lainnya, selain api web Anda sendiri.</span><span class="sxs-lookup"><span data-stu-id="6a801-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

