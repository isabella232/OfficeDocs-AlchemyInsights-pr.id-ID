---
title: Pemilik tidak dapat membuat sub-folder menggunakan Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749148"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="bfa99-102">Pemilik tidak dapat membuat sub-folder menggunakan Outlook</span><span class="sxs-lookup"><span data-stu-id="bfa99-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="bfa99-103">**Ada masalah yang sedang berlangsung dengan pemilik folder publik yang membuat subfolder menggunakan Outlook. Masalah akan segera diperbaiki.**</span><span class="sxs-lookup"><span data-stu-id="bfa99-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="bfa99-104">Sementara itu, gunakan salah satu dari penyelesaian berikut:</span><span class="sxs-lookup"><span data-stu-id="bfa99-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="bfa99-105">Menggunakan Outlook untuk MAC untuk membuat subfolder sebagai masalah dampak hanya Outlook untuk Windows Desktop (semua versi)</span><span class="sxs-lookup"><span data-stu-id="bfa99-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="bfa99-106">Memiliki admin membuat subfolder menggunakan EXO shell atau EAC</span><span class="sxs-lookup"><span data-stu-id="bfa99-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="bfa99-107">Mengubah DefaultPublicFolderMailbox/EffectivePublicFolderMailbox di pengguna ke kotak surat lainnya dari kotak surat konten untuk folder yang menyebabkan masalah</span><span class="sxs-lookup"><span data-stu-id="bfa99-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="bfa99-108">*Set-kotak surat User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="bfa99-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="bfa99-109">Tunggu selama satu jam, mulai ulang klien Outlook</span><span class="sxs-lookup"><span data-stu-id="bfa99-109">Wait for an hour, restart outlook client</span></span>