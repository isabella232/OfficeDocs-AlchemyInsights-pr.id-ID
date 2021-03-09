---
title: Kesalahan alamat proksi saat membuat kotak surat bersama
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568293"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="76f1b-102">Kesalahan alamat proksi saat membuat kotak surat atau objek diaktifkan email lainnya</span><span class="sxs-lookup"><span data-stu-id="76f1b-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="76f1b-103">Jika Anda mencoba membuat objek yang didukung email (kotak surat, kotak surat bersama, dsb.) dan menerima kesalahan "alamat proksi" SMTP:alias@domain.com "sudah digunakan...", alamat email yang Anda pilih sudah diambil oleh objek yang didukung email lain di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="76f1b-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="76f1b-104">Anda perlu menemukan pengguna, grup, kotak surat bersama atau folder publik yang memiliki alamat email ini dan menghapusnya atau mengubah alamat emailnya.</span><span class="sxs-lookup"><span data-stu-id="76f1b-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="76f1b-105">Lalu Anda dapat membuat objek yang didukung email baru dengan alamat email yang dibebaskan.</span><span class="sxs-lookup"><span data-stu-id="76f1b-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="76f1b-106">Gunakan pencarian di halaman Beranda untuk menemukannya.</span><span class="sxs-lookup"><span data-stu-id="76f1b-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="76f1b-107">Anda juga dapat menggunakan perintah Exchange Online PowerShell berikut ini untuk mencarinya:</span><span class="sxs-lookup"><span data-stu-id="76f1b-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="76f1b-108">Jika Anda tidak ingin menghapus alamat email yang sudah ada, pilih alamat email baru untuk objek baru yang Anda buat.</span><span class="sxs-lookup"><span data-stu-id="76f1b-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  