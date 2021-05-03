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
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Masalah dengan SharePoint di Windows 7 komputer

Jika Anda menerima kesalahan Windows 7 komputer saat bekerja di SharePoint atau OneDrive, kesalahan itu mungkin terkait dengan penghentian TLS 1.0/1.1. Untuk informasi selengkapnya, lihat:

- [Mempersiapkan TLS 1.2 di Office 365 dan Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows klien SP1/Windows 8 7 harus mengaktifkan TLS1.2. Untuk informasi selengkapnya, [lihat Kesalahan autentikasi terjadi saat klien tidak memiliki dukungan TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Instal KB3140245 dan buat nilai registri. Untuk informasi selengkapnya, lihat Memperbarui untuk mengaktifkan [TLS 1.1 dan TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) sebagai protokol aman default di WinHTTP di Windows

- Windows klien SP1/Windows 8 7 harus memastikan bahwa seripher TLS terbaru telah terinstal. Untuk informasi selengkapnya, lihat [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


