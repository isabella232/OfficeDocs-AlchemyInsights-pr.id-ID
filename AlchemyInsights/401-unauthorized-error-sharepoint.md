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
ms.openlocfilehash: 3b81bab22c9deb6498827b01f54fac0be2f7c35b6f912d729b44ddc4f45598cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919030"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Kesalahan tidak sah di SharePoint

Jika Anda menerima kesalahan "(401) Tidak Sah" di SharePoint mungkin terkait dengan penghentian TLS 1.0/1.1. Untuk informasi selengkapnya, lihat:

- [Mempersiapkan TLS 1.2 di Office 365 dan Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Kesalahan autentikasi terjadi jika klien tidak memiliki dukungan TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Pembaruan untuk mengaktifkan TLS 1.1 dan TLS 1.2 sebagai protokol aman default di WinHTTP di Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Jika pengguna menggunakan Windows 7, pastikan mereka memeriksa [Tls Cipher Suites di Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).