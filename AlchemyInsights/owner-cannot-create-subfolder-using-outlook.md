---
title: Pemilik tidak dapat membuat sub-folder menggunakan Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836138"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="7478b-102">Pemilik tidak dapat membuat sub-folder menggunakan Outlook</span><span class="sxs-lookup"><span data-stu-id="7478b-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="7478b-103">**Masih terdapat masalah dengan pemilik folder publik yang membuat subfolder menggunakan Outlook. Masalah akan segera diperbaiki.**</span><span class="sxs-lookup"><span data-stu-id="7478b-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="7478b-104">Sementara itu, gunakan salah satu solusi berikut:</span><span class="sxs-lookup"><span data-stu-id="7478b-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="7478b-105">Menggunakan Outlook untuk MAC untuk membuat subfolder karena masalah hanya memengaruhi Outlook untuk jendela desktop (semua versi)</span><span class="sxs-lookup"><span data-stu-id="7478b-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="7478b-106">Buat admin membuat subfolder menggunakan EXO Shell atau EAC</span><span class="sxs-lookup"><span data-stu-id="7478b-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="7478b-107">Mengubah DefaultPublicFolderMailbox/EffectivePublicFolderMailbox pada pengguna ke kotak surat lain dari Kotak Surat Konten untuk folder yang menyebabkan masalah</span><span class="sxs-lookup"><span data-stu-id="7478b-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="7478b-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="7478b-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="7478b-109">Tunggu satu jam, mulai ulang klien outlook</span><span class="sxs-lookup"><span data-stu-id="7478b-109">Wait for an hour, restart outlook client</span></span>