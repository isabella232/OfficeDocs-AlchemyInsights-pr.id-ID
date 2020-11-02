---
title: 0x8004de40 kesalahan ketika meluncurkan OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823051"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="c35e7-102">0x8004de40 kesalahan ketika meluncurkan OneDrive</span><span class="sxs-lookup"><span data-stu-id="c35e7-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="c35e7-103">Jika Anda menerima kesalahan **0x8004de40** saat masuk ke OneDrive, reboot komputer saat tersambung ke domain kerja atau sekolah Anda.</span><span class="sxs-lookup"><span data-stu-id="c35e7-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="c35e7-104">Jika Anda menerima kesalahan ini setelah reboot, coba ini saat tersambung ke domain kerja atau sekolah Anda:</span><span class="sxs-lookup"><span data-stu-id="c35e7-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="c35e7-105">Klik mulai, lalu ketikkan **CMD** atau **command prompt**  dalam kotak pencarian, klik kanan pada aplikasi prompt perintah, lalu pilih  **Jalankan sebagai administrator** .</span><span class="sxs-lookup"><span data-stu-id="c35e7-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="c35e7-106">Jika Anda dimintai kata sandi administrator atau untuk konfirmasi, ketikkan kata sandi, atau klik **Perbolehkan** .</span><span class="sxs-lookup"><span data-stu-id="c35e7-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="c35e7-107">Di jendela prompt perintah, ketik **dsregcmd/Leave**  dan tunggu hingga perintah selesai.</span><span class="sxs-lookup"><span data-stu-id="c35e7-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="c35e7-108">Lalu ketikkan **dsregcmd/Join** dan tunggu hingga perintah selesai.</span><span class="sxs-lookup"><span data-stu-id="c35e7-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="c35e7-109">Hidupkan ulang komputer Anda.</span><span class="sxs-lookup"><span data-stu-id="c35e7-109">Reboot your computer.</span></span>
