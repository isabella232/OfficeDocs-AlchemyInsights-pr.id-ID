---
title: Izin dan izin API
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
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974607"
---
# <a name="api-permissions-and-consent"></a>Izin dan izin API

Aplikasi yang terintegrasi dengan platform Microsoft Identity ikuti model otorisasi yang memberi pengguna dan administrator kontrol atas bagaimana data bisa diakses. Penerapan model otorisasi telah diperbarui pada titik akhir platform identitas Microsoft. Mengubah cara aplikasi harus berinteraksi dengan platform identitas Microsoft. [Izin dan persetujuan di titik akhir platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) membahas konsep dasar model otorisasi ini, termasuk lingkup, izin, dan persetujuan.

[Kerangka izin Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) memudahkan untuk mengembangkan multi-penyewa web dan aplikasi klien asli. Aplikasi ini memperbolehkan masuk dengan akun pengguna dari penyewa Azure AD yang berbeda dari aplikasi yang didaftarkan. Mereka juga mungkin perlu mengakses api web seperti API Microsoft graph (untuk mengakses Azure AD, Intune, dan Services di Microsoft 365) dan api layanan Microsoft lainnya, selain api web Anda sendiri.

