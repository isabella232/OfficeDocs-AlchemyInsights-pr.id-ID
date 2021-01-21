---
title: Mengonfigurasi dan memperpanjang masa berlaku token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917003"
---
# <a name="configure-and-extend-token-lifetimes"></a>Mengonfigurasi dan memperpanjang masa berlaku token

Anda dapat menentukan seumur hidup dari token Access, SAML, atau ID yang diterbitkan oleh Microsoft Identity platform. Anda dapat mengatur masa pakai token untuk semua aplikasi di organisasi Anda, untuk aplikasi multi-penyewa (multi-organisasi), atau untuk prinsip layanan tertentu di organisasi Anda. Untuk informasi selengkapnya, baca [masa hidup token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)yang dapat dikonfigurasi.

Sebagai contoh, baca [contoh cara mengonfigurasi masa hidup token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Untuk mempelajari cara mengonfigurasi seumur hidup dan kompatibilitas Token di Azure Active Directory B2C (Azure AD B2C), lihat [mengonfigurasi Token di B2C direktori aktif Azure](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Artikel [mengonfigurasi perilaku sesi di Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) menguraikan metode masuk tunggal (SSO) yang digunakan di AZURE AD B2C dan membantu Anda memilih metode SSO yang paling tepat saat mengonfigurasi kebijakan Anda.

**Berapa lama token bertahan? Berapa lama waktu yang mereka miliki?**

Masa pakai Token adalah 1 jam dan seumur hidup dalam sesi 24 jam. Ini berarti bahwa jika tidak ada permintaan yang dilakukan dalam 24 Jam, Anda perlu masuk lagi sebelum meminta token baru.

> [!NOTE]
> Setelah 30 Mei 2020, tidak ada penyewa baru yang dapat menggunakan kebijakan seumur hidup untuk mengonfigurasi token sesi dan refresh. Penghentian akan terjadi dalam beberapa bulan setelah itu, yang berarti bahwa kami akan menghentikan menghormati tata sesi dan me-refresh Token yang sudah ada. Anda masih bisa mengonfigurasi masa berlaku token Access setelah penghentian.






