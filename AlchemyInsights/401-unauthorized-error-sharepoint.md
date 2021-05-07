---
title: 401 Kesalahan tidak sah di SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233506"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="88db6-102">401 Kesalahan tidak sah di SharePoint</span><span class="sxs-lookup"><span data-stu-id="88db6-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="88db6-103">Jika Anda menerima kesalahan "(401) Tidak Sah" di SharePoint mungkin terkait dengan penghentian TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="88db6-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="88db6-104">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="88db6-104">For more info, see:</span></span>

[<span data-ttu-id="88db6-105">Mempersiapkan TLS 1.2 di Office 365 dan Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="88db6-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[<span data-ttu-id="88db6-106">Kesalahan autentikasi terjadi jika klien tidak memiliki dukungan TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="88db6-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="88db6-107">Jika pengguna menggunakan Windows 7, pastikan mereka memeriksa [Tls Cipher Suites di Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span><span class="sxs-lookup"><span data-stu-id="88db6-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>