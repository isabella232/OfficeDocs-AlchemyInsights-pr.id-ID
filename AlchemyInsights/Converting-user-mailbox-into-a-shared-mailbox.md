---
title: Mengkonversi kotak pesan pengguna ke kotak pesan bersama?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496402"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="c606c-102">Mengkonversi kotak pesan pengguna ke kotak pesan bersama</span><span class="sxs-lookup"><span data-stu-id="c606c-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="c606c-103">Anda hanya dapat mengkonversi kotak pesan pengguna ke kotak pesan bersama jika pengguna memiliki lisensi asing.</span><span class="sxs-lookup"><span data-stu-id="c606c-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="c606c-104">Setelah kotak pesan yang diubah, itu akan terus muncul di daftar pengguna aktif karena daftar itu mencakup kotak pesan bersama.</span><span class="sxs-lookup"><span data-stu-id="c606c-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="c606c-105">Namun, kotak pesan yang dikonversi akan juga muncul dalam daftar kotak pesan bersama.</span><span class="sxs-lookup"><span data-stu-id="c606c-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="c606c-106">Jika Anda mencoba untuk mengkonversi kotak pesan di Exchange Admin Console dan konversi gagal, membersihkan tembolok peramban dan kuki dan coba lagi.</span><span class="sxs-lookup"><span data-stu-id="c606c-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="c606c-107">Jika itu masih tidak bekerja, coba mengkonversi kotak pesan di Exchange Management Shell dengan menjalankan perintah berikut:</span><span class="sxs-lookup"><span data-stu-id="c606c-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="c606c-108">Selengkapnya konversi kotak pesan ini tersedia dalam [mengkonversi pesan pengguna ke kotak pesan bersama](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c606c-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
