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
ms.openlocfilehash: 0515ead28cdfdbdb9529c269b5170b294ab2b120
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543040"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="00053-102">Kesalahan "Koneksi yang mendasari ditutup" di SharePoint</span><span class="sxs-lookup"><span data-stu-id="00053-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="00053-103">Jika menerima kesalahan "Koneksi yang mendasari ditutup" SharePoint mungkin terkait dengan penghentian TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="00053-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="00053-104">Untuk informasi selengkapnya, lihat artikel berikut ini:</span><span class="sxs-lookup"><span data-stu-id="00053-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="00053-105">Mempersiapkan TLS 1.2 di Office 365 dan Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="00053-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="00053-106">Kesalahan autentikasi terjadi jika klien tidak memiliki dukungan TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="00053-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="00053-107">Pembaruan untuk mengaktifkan TLS 1.1 dan TLS 1.2 sebagai protokol aman default di WinHTTP di Windows</span><span class="sxs-lookup"><span data-stu-id="00053-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="00053-108">Jika pengguna menggunakan Windows 7, pastikan mereka memeriksa [Tls Cipher Suites di Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span><span class="sxs-lookup"><span data-stu-id="00053-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>