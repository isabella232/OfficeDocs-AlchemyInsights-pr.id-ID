---
title: Masalah izin admin
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901132"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="8d433-102">Masalah izin admin</span><span class="sxs-lookup"><span data-stu-id="8d433-102">Admin consent issues</span></span>

1. <span data-ttu-id="8d433-103">Aktifkan [alur kerja izin admin](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) untuk memperbolehkan pengguna meminta persetujuan administrator secara langsung dari layar persetujuan.</span><span class="sxs-lookup"><span data-stu-id="8d433-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="8d433-104">Jika Anda atau pengguna aplikasi Anda melihat kesalahan yang tidak diharapkan selama proses persetujuan, lihat artikel ini untuk langkah pemecahan masalah: [kesalahan tak terduga saat melakukan persetujuan ke aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="8d433-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="8d433-105">Pelajari selengkapnya tentang [persetujuan admin di platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), cara kerja [perintah persetujuan](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) , dan cara [mengevaluasi permintaan untuk persetujuan admin penyewa-lebar](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="8d433-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="8d433-106">Aplikasi yang terintegrasi dengan platform Microsoft Identity ikuti model otorisasi yang memberi pengguna dan administrator kontrol atas bagaimana data bisa diakses.</span><span class="sxs-lookup"><span data-stu-id="8d433-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="8d433-107">Penerapan model otorisasi telah diperbarui pada titik akhir platform identitas Microsoft, dan mengubah cara aplikasi harus berinteraksi dengan platform identitas Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8d433-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="8d433-108">Lihat [izin dan persetujuan di titik akhir platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) untuk gambaran umum model otorisasi ini, termasuk lingkup, izin, dan persetujuan.</span><span class="sxs-lookup"><span data-stu-id="8d433-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>