---
title: 902 (sync kesalahan karena duplikat objek)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507418"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Galat sinkronisasi karena duplikat objek

Anda mungkin menerima salah satu pesan galat berikut ketika selesai sinkronisasi direktori di Office 365:

- Tidak dapat memperbarui objek ini di Microsoft Online Services karena atribut berikut terkait dengan objek ini memiliki nilai yang sudah mungkin terkait dengan objek lain dalam direktori lokal Anda.

- Sebuah objek disinkronisasi dengan alamat proxy yang sama sudah ada di direktori Layanan Online Microsoft.

- Tidak dapat memperbarui objek ini karena atribut berikut terkait dengan objek ini memiliki nilai-nilai yang sudah mungkin terkait dengan objek lain di layanan direktori lokal Anda: UserPrincipalName.

Untuk mengidentifikasi dan memperbaiki masalah, download dan menjalankan [Alat perbaikan IdFix DirSync kesalahan](https://www.microsoft.com/download/details.aspx?id=36832).

Untuk informasi lebih lanjut, lihat [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
