---
title: 902 (sinkronisasi kesalahan karena duplikat objek)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767131"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Galat sinkronisasi karena duplikat objek

Anda mungkin menerima salah satu pesan galat berikut saat sinkronisasi direktori selesai di Microsoft 365:

- Tidak dapat memutakhirkan objek ini di Microsoft Online Services karena atribut berikut ini yang berkaitan dengan objek ini memiliki nilai yang sudah mungkin terkait dengan objek lain di direktori lokal Anda.

- Objek disinkronkan dengan alamat proksi yang sama yang sudah ada di direktori Microsoft Online Services.

- Tidak dapat memutakhirkan objek ini karena atribut berikut ini yang berkaitan dengan objek ini memiliki nilai yang sudah mungkin terkait dengan objek lain di layanan direktori lokal Anda: UserPrincipalName.

Untuk mengidentifikasi dan memperbaiki masalah, Unduh dan jalankan [alat remediasi galat DirSync idfix](https://www.microsoft.com/download/details.aspx?id=36832).

Untuk informasi selengkapnya, lihat [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
