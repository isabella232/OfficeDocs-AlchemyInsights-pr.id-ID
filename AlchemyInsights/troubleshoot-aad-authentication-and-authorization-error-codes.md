---
title: Memecahkan masalah kode kesalahan autentikasi dan autentikasi Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036508"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="f29bd-102">Memecahkan masalah kode kesalahan autentikasi dan autentikasi Azure AD</span><span class="sxs-lookup"><span data-stu-id="f29bd-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="f29bd-103">Untuk mengatasi kode kesalahan dan autentikasi AAD (AADSTS), lakukan langkah-langkah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="f29bd-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="f29bd-104">**Menangani kode kesalahan dalam aplikasi Anda**</span><span class="sxs-lookup"><span data-stu-id="f29bd-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="f29bd-105">**Spesifikasi OAuth 2.0**, https://tools.ietf.org/html/rfc6749#section-5.2 , memberikan panduan tentang cara menangani kesalahan selama autentikasi menggunakan porsi kesalahan dari respons kesalahan.</span><span class="sxs-lookup"><span data-stu-id="f29bd-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="f29bd-106">**kesalahan**: string kode kesalahan yang bisa digunakan untuk mengelompokkan tipe kesalahan yang terjadi, dan harus digunakan untuk bereaksi terhadap kesalahan.</span><span class="sxs-lookup"><span data-stu-id="f29bd-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="f29bd-107">Bidang **kesalahan** memiliki beberapa nilai yang memungkinkan-Tinjau link dokumentasi protokol dan spesifikasi OAuth 2,0 untuk informasi selengkapnya tentang kesalahan tertentu dan cara bereaksi terhadapnya.</span><span class="sxs-lookup"><span data-stu-id="f29bd-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="f29bd-108">Berikut ini adalah contoh respons kesalahan:</span><span class="sxs-lookup"><span data-stu-id="f29bd-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="f29bd-109">**Informasi kode kesalahan pencarian saat ini**</span><span class="sxs-lookup"><span data-stu-id="f29bd-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="f29bd-110">Kode kesalahan dan pesan dapat berubah.</span><span class="sxs-lookup"><span data-stu-id="f29bd-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="f29bd-111">Untuk informasi terbaru, lihat https://login.microsoftonline.com/error halaman untuk menemukan deskripsi kesalahan, perbaikan, dan beberapa solusi yang disarankan.</span><span class="sxs-lookup"><span data-stu-id="f29bd-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="f29bd-112">Anda juga dapat mencari dan memecahkan masalah [kode kesalahan Aadsts](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) yang tercantum dalam [kode kesalahan pengesahan dan autentikasi Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="f29bd-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="f29bd-113">**Mendapatkan bantuan**</span><span class="sxs-lookup"><span data-stu-id="f29bd-113">**Get Help**</span></span>

- <span data-ttu-id="f29bd-114">[Opsi dukungan dan bantuan untuk pengembang](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) -jika Anda memerlukan jawaban untuk pertanyaan atau bantuan dalam memecahkan masalah yang tidak tercakup dalam dokumentasi kami, mungkin ada waktu untuk menghubungi pakar untuk bantuan.</span><span class="sxs-lookup"><span data-stu-id="f29bd-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="f29bd-115">Artikel ini menyediakan beberapa saran untuk menjawab pertanyaan Anda saat Anda mengembangkan aplikasi yang berintegrasi dengan platform identitas Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f29bd-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








