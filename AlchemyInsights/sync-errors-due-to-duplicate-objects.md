---
title: 902 (Kesalahan sinkronisasi karena objek duplikat)
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
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998797"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Menyinkronkan kesalahan karena objek duplikat

Anda mungkin menerima salah satu pesan kesalahan berikut ini saat sinkronisasi direktori selesai Microsoft 365:

- Tidak dapat memperbarui objek ini di Microsoft Online Services karena atribut berikut yang terkait dengan objek ini memiliki nilai yang mungkin sudah terkait dengan objek lain dalam direktori lokal Anda.

- Objek yang disinkronkan dengan alamat proksi yang sama sudah ada di direktori Microsoft Online Services Anda.

- Tidak dapat memperbarui objek ini karena atribut berikut yang terkait dengan objek ini memiliki nilai yang mungkin sudah terkait dengan objek lain di layanan direktori lokal Anda: UserPrincipalName.

Untuk mengidentifikasi dan memperbaiki masalah tersebut, unduh dan jalankan [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).

Untuk informasi selengkapnya, lihat [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
