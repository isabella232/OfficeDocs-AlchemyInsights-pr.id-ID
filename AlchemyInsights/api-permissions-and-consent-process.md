---
title: Izin API dan Proses Persetujuan
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404872"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="1d904-102">Izin API dan Proses Persetujuan</span><span class="sxs-lookup"><span data-stu-id="1d904-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="1d904-103">Agar aplikasi Anda mengakses data di Microsoft Graph, pengguna atau administrator harus memberikan izin yang tepat melalui proses persetujuan.</span><span class="sxs-lookup"><span data-stu-id="1d904-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="1d904-104">[Referensi izin Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) mencantumkan izin yang terkait dengan setiap rangkaian utama API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d904-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="1d904-105">Panduan juga tentang cara menggunakan izin.</span><span class="sxs-lookup"><span data-stu-id="1d904-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="1d904-106">**Menyetel atau memperbarui prinsipal layanan**</span><span class="sxs-lookup"><span data-stu-id="1d904-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="1d904-107">[Buat serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Artikel ini memperlihatkan cara membuat objek servicePrincipal baru.</span><span class="sxs-lookup"><span data-stu-id="1d904-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="1d904-108">[Membuat prinsipal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) layanan & Azure AD dalam portal - Artikel ini memperlihatkan cara membuat aplikasi Azure Active Directory (Azure AD) dan prinsipal layanan baru yang dapat digunakan dengan kontrol akses berbasis peran.</span><span class="sxs-lookup"><span data-stu-id="1d904-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="1d904-109">[Pokok &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) aplikasi dalam Azure AD - Artikel ini menguraikan pendaftaran aplikasi, objek aplikasi, dan prinsipal layanan dalam Azure Active Directory: apa itu, cara menggunakannya, dan bagaimana aplikasi saling terkait.</span><span class="sxs-lookup"><span data-stu-id="1d904-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="1d904-110">**Menambahkan atau memperbarui pendaftaran aplikasi dan memberikan persetujuan admin**</span><span class="sxs-lookup"><span data-stu-id="1d904-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="1d904-111">[Buat pendaftaran aplikasi](https://docs.microsoft.com/graph/api/application-post-applications) - Artikel ini memperlihatkan pada Anda cara membuat objek aplikasi baru.</span><span class="sxs-lookup"><span data-stu-id="1d904-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="1d904-112">[Memperbarui pendaftaran aplikasi - izin API](https://docs.microsoft.com/graph/api/application-update) - Artikel ini memperlihatkan cara memperbarui properti objek aplikasi.</span><span class="sxs-lookup"><span data-stu-id="1d904-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="1d904-113">[Memberikan izin admin](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Untuk persetujuan dan persetujuan admin secara umum, kami mengharuskan admin secara eksplisit memberikan persetujuan.</span><span class="sxs-lookup"><span data-stu-id="1d904-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="1d904-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Wadah manajemen peran untuk definisi peran terpadu dan penetapan peran untuk penyedia RBAC Microsoft 365 yang mendukung beberapa prinsipal dan beberapa lingkup dalam penugasan peran tunggal.</span><span class="sxs-lookup"><span data-stu-id="1d904-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="1d904-115">Ini berbeda dari *tipe sumber daya aplikasi rbac.*</span><span class="sxs-lookup"><span data-stu-id="1d904-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="1d904-116">Microsoft Intune adalah contoh penyedia RBAC.</span><span class="sxs-lookup"><span data-stu-id="1d904-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="1d904-117">Penugasan peran di Intune dapat memiliki larik pokok dan larik grup lingkup.</span><span class="sxs-lookup"><span data-stu-id="1d904-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="1d904-118">**Dalam versi beta, artinya file masih dalam pengembangan dan tidak direkomendasikan untuk digunakan dalam produksi.**</span><span class="sxs-lookup"><span data-stu-id="1d904-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
