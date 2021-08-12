---
title: Izin DAN Persetujuan API
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932100"
---
# <a name="api-permissions-and-consent"></a>Izin dan persetujuan API

Aplikasi yang berintegrasi dengan platform identitas Microsoft mengikuti model otorisasi yang memberikan kontrol kepada pengguna dan administrator tentang bagaimana data dapat diakses. Implementasi model otorisasi telah diperbarui pada platform identitas Microsoft akhir. Ini mengubah cara aplikasi harus berinteraksi dengan platform identitas Microsoft. [Izin dan persetujuan di platform identitas Microsoft titik akhir](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) mencakup konsep dasar model otorisasi ini, termasuk lingkup, izin, dan persetujuan.

Kerangka [kerja Azure Active Directory persetujuan (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) memudahkan untuk mengembangkan aplikasi klien asli dan web multi-penyewa. Aplikasi tersebut memungkinkan akses masuk menurut akun pengguna dari penyewa Azure AD yang berbeda dengan tempat aplikasi didaftarkan. Mereka mungkin juga perlu mengakses API web seperti API Microsoft Graph (untuk mengakses Azure AD, Intune, dan layanan di Microsoft 365) dan API layanan Microsoft lainnya, selain API web Anda sendiri.

