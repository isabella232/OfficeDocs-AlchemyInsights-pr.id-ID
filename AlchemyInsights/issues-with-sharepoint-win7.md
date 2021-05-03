---
title: Masalah dengan SharePoint di Windows 7 komputer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125123"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="670bc-102">Masalah dengan SharePoint di Windows 7 komputer</span><span class="sxs-lookup"><span data-stu-id="670bc-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="670bc-103">Jika Anda menerima kesalahan Windows 7 komputer saat bekerja di SharePoint atau OneDrive, kesalahan itu mungkin terkait dengan penghentian TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="670bc-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="670bc-104">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="670bc-104">For more information, see:</span></span>

- [<span data-ttu-id="670bc-105">Mempersiapkan TLS 1.2 di Office 365 dan Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="670bc-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="670bc-106">Windows klien SP1/Windows 8 7 harus mengaktifkan TLS1.2.</span><span class="sxs-lookup"><span data-stu-id="670bc-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="670bc-107">Untuk informasi selengkapnya, [lihat Kesalahan autentikasi terjadi saat klien tidak memiliki dukungan TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="670bc-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="670bc-108">Instal KB3140245 dan buat nilai registri.</span><span class="sxs-lookup"><span data-stu-id="670bc-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="670bc-109">Untuk informasi selengkapnya, lihat Memperbarui untuk mengaktifkan [TLS 1.1 dan TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) sebagai protokol aman default di WinHTTP di Windows</span><span class="sxs-lookup"><span data-stu-id="670bc-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="670bc-110">Windows klien SP1/Windows 8 7 harus memastikan bahwa seripher TLS terbaru telah terinstal.</span><span class="sxs-lookup"><span data-stu-id="670bc-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="670bc-111">Untuk informasi selengkapnya, lihat [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="670bc-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


