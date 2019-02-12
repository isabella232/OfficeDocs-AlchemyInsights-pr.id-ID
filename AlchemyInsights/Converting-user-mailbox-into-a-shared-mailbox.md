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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906735"
---
<span data-ttu-id="d1ca7-p101">Anda hanya dapat mengkonversi kotak pesan pengguna ke kotak pesan bersama jika pengguna memiliki lisensi asing. Setelah kotak pesan yang diubah, itu akan terus muncul di daftar pengguna aktif karena daftar itu mencakup kotak pesan bersama. Namun, kotak pesan yang dikonversi akan juga muncul dalam daftar kotak pesan bersama.</span><span class="sxs-lookup"><span data-stu-id="d1ca7-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="d1ca7-p102">Jika Anda mencoba untuk mengkonversi kotak pesan di Exchange Admin Console dan konversi gagal, membersihkan tembolok peramban dan kuki dan coba lagi. Jika itu masih tidak bekerja, coba mengkonversi kotak pesan di Exchange Management Shell dengan menjalankan perintah berikut:</span><span class="sxs-lookup"><span data-stu-id="d1ca7-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="d1ca7-107">Selengkapnya konversi kotak pesan ini tersedia dalam [mengkonversi pesan pengguna ke kotak pesan bersama](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="d1ca7-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
