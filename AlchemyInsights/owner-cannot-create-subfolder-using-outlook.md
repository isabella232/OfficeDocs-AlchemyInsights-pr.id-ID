---
title: Pemilik tidak dapat membuat sub-folder menggunakan Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665721"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="f85b4-102">Pemilik tidak dapat membuat sub-folder menggunakan Outlook</span><span class="sxs-lookup"><span data-stu-id="f85b4-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="f85b4-103">**Ada masalah yang sedang berlangsung dengan pemilik folder publik membuat subfolder menggunakan Outlook. Masalah akan segera diperbaiki.**</span><span class="sxs-lookup"><span data-stu-id="f85b4-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="f85b4-104">Sementara itu, gunakan salah satu solusi berikut:</span><span class="sxs-lookup"><span data-stu-id="f85b4-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="f85b4-105">Menggunakan Outlook untuk MAC untuk membuat subfolder karena masalah hanya memengaruhi Outlook untuk desktop Windows (semua versi)</span><span class="sxs-lookup"><span data-stu-id="f85b4-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="f85b4-106">Membuat admin membuat subfolder menggunakan EXO shell atau EAC</span><span class="sxs-lookup"><span data-stu-id="f85b4-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="f85b4-107">Mengubah DefaultPublicFolderMailbox/EffectivePublicFolderMailbox pada pengguna ke kotak surat lain dari kotak surat konten untuk masalah yang menyebabkan folder</span><span class="sxs-lookup"><span data-stu-id="f85b4-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="f85b4-108">*Set-kotak surat User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="f85b4-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="f85b4-109">Menunggu satu jam, mulai ulang klien Outlook</span><span class="sxs-lookup"><span data-stu-id="f85b4-109">Wait for an hour, restart outlook client</span></span>