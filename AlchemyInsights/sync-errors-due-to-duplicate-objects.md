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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708065"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="ba403-102">Kesalahan sinkronisasi karena objek duplikat</span><span class="sxs-lookup"><span data-stu-id="ba403-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="ba403-103">Anda mungkin menerima salah satu pesan kesalahan berikut ini saat sinkronisasi direktori selesai di Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="ba403-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="ba403-104">Tidak dapat memperbarui objek ini di layanan online Microsoft karena atribut berikut yang terkait dengan objek ini memiliki nilai yang mungkin terkait dengan objek lain dalam direktori lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="ba403-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="ba403-105">Objek yang disinkronkan dengan alamat proksi yang sama sudah ada di direktori Microsoft Online Services Anda.</span><span class="sxs-lookup"><span data-stu-id="ba403-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="ba403-106">Tidak dapat memperbarui objek ini karena atribut berikut yang terkait dengan objek ini memiliki nilai yang mungkin terkait dengan objek lain di layanan direktori lokal Anda: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="ba403-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="ba403-107">Untuk mengidentifikasi dan memperbaiki masalah, Unduh dan jalankan [alat remediasi kesalahan DirSync Idfix](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="ba403-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="ba403-108">Untuk informasi selengkapnya, lihat [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="ba403-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
