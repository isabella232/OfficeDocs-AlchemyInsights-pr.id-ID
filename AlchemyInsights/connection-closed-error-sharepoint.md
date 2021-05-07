---
title: Koneksi yang mendasarinya ditutup di SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233429"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="92b19-102">Kesalahan "Koneksi yang mendasari ditutup" di SharePoint</span><span class="sxs-lookup"><span data-stu-id="92b19-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="92b19-103">Jika menerima kesalahan "Koneksi yang mendasari ditutup" SharePoint mungkin terkait dengan penghentian TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="92b19-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="92b19-104">Untuk informasi selengkapnya, lihat artikel berikut ini:</span><span class="sxs-lookup"><span data-stu-id="92b19-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="92b19-105">Mempersiapkan TLS 1.2 di Office 365 dan Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="92b19-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [<span data-ttu-id="92b19-106">Kesalahan autentikasi terjadi jika klien tidak memiliki dukungan TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="92b19-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="92b19-107">Jika pengguna menggunakan Windows 7, pastikan mereka memeriksa [Tls Cipher Suites di Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span><span class="sxs-lookup"><span data-stu-id="92b19-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>