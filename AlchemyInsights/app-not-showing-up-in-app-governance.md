---
title: Aplikasi saya tidak muncul dalam Tata Kelola Aplikasi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454696"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Aplikasi saya tidak muncul dalam Tata Kelola Aplikasi

Jika aplikasi Anda tidak muncul dalam Tata Kelola Aplikasi, periksa yang berikut ini:

1. Buka [Azure AD](https://aad.portal.azure.com/) dan temukan ID aplikasi untuk aplikasi Anda dengan mencari nama aplikasi di bilah bagian atas halaman Gambaran Umum.

1. Access Graph Explorer dan cari ID aplikasi dalam prinsipal layanan Anda menggunakan kueri ini dan mengganti dengan ID aplikasi yang <appId> relevan: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Jika tidak ada hasil yang dikembalikan, cari ID aplikasi di dalam aplikasi menggunakan kueri ini dan ganti dengan ID aplikasi yang <appId> relevan: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Jika Anda mengalami masalah dengan kueri, lihat [Mendapatkan dukungan](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Untuk informasi atau wawasan selengkapnya tentang Aplikasi di Tata Kelola Aplikasi, [lihat Pelajari tentang visibilitas dan wawasan](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview).

Untuk informasi selengkapnya tentang menampilkan aplikasi Anda, lihat [Menampilkan aplikasi Anda](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
