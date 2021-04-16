---
title: 0x8004de40 saat meluncurkan OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813655"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="f8134-102">0x8004de40 saat meluncurkan OneDrive</span><span class="sxs-lookup"><span data-stu-id="f8134-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="f8134-103">Jika Anda menerima pesan **kesalahan 0x8004de40** masuk ke OneDrive, mulai ulang komputer saat tersambung ke domain kantor atau sekolah Anda.</span><span class="sxs-lookup"><span data-stu-id="f8134-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="f8134-104">Jika Anda menerima kesalahan ini setelah memulai ulang, coba hal ini saat tersambung ke domain kerja atau sekolah Anda:</span><span class="sxs-lookup"><span data-stu-id="f8134-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="f8134-105">Klik Mulai, lalu **ketikkan cmd** atau **prompt perintah**  dalam kotak pencarian, klik kanan aplikasi prompt perintah, lalu pilih Jalankan  **sebagai administrator**.</span><span class="sxs-lookup"><span data-stu-id="f8134-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="f8134-106">Jika Anda dimintai kata sandi administrator atau konfirmasi, ketik kata sandi, atau klik **Perbolehkan.**</span><span class="sxs-lookup"><span data-stu-id="f8134-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="f8134-107">Di jendela Prompt Perintah, ketik **dsregcmd /leave**  dan tunggu perintah selesai.</span><span class="sxs-lookup"><span data-stu-id="f8134-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="f8134-108">Lalu ketik **dsregcmd /join** dan tunggu perintah selesai.</span><span class="sxs-lookup"><span data-stu-id="f8134-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="f8134-109">Me-reboot komputer Anda.</span><span class="sxs-lookup"><span data-stu-id="f8134-109">Reboot your computer.</span></span>
