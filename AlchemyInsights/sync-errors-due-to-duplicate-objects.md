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
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="3cf2c-102">Galat sinkronisasi karena duplikat objek</span><span class="sxs-lookup"><span data-stu-id="3cf2c-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="3cf2c-103">Anda mungkin menerima salah satu pesan galat berikut ketika selesai sinkronisasi direktori di Office 365:</span><span class="sxs-lookup"><span data-stu-id="3cf2c-103">You might receive one of the following error messages when directory synchronization finishes in Office 365:</span></span>

- <span data-ttu-id="3cf2c-104">Tidak dapat memperbarui objek ini di Microsoft Online Services karena atribut berikut terkait dengan objek ini memiliki nilai yang sudah mungkin terkait dengan objek lain dalam direktori lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="3cf2c-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="3cf2c-105">Sebuah objek disinkronisasi dengan alamat proxy yang sama sudah ada di direktori Layanan Online Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3cf2c-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="3cf2c-106">Tidak dapat memperbarui objek ini karena atribut berikut terkait dengan objek ini memiliki nilai-nilai yang sudah mungkin terkait dengan objek lain di layanan direktori lokal Anda: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3cf2c-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="3cf2c-107">Untuk mengidentifikasi dan memperbaiki masalah, download dan menjalankan [Alat perbaikan IdFix DirSync kesalahan](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="3cf2c-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="3cf2c-108">Untuk informasi lebih lanjut, lihat [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="3cf2c-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
