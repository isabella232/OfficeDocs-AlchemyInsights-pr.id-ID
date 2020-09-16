---
title: 902 (kesalahan sinkronisasi karena duplikat objek)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737344"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Kesalahan sinkronisasi karena objek duplikat

Anda mungkin menerima salah satu pesan kesalahan berikut ini saat sinkronisasi direktori selesai di Microsoft 365:

- Tidak dapat memperbarui objek ini di layanan online Microsoft karena atribut berikut yang terkait dengan objek ini memiliki nilai yang mungkin terkait dengan objek lain dalam direktori lokal Anda.

- Objek yang disinkronkan dengan alamat proksi yang sama sudah ada di direktori Microsoft Online Services Anda.

- Tidak dapat memperbarui objek ini karena atribut berikut yang terkait dengan objek ini memiliki nilai yang mungkin terkait dengan objek lain di layanan direktori lokal Anda: UserPrincipalName.

Untuk mengidentifikasi dan memperbaiki masalah, Unduh dan jalankan [alat remediasi kesalahan DirSync Idfix](https://www.microsoft.com/download/details.aspx?id=36832).

Untuk informasi selengkapnya, lihat [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
