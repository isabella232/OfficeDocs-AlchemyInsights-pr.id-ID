---
title: Menghapus layanan latar belakang untuk Microsoft Search di Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816202"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="dc9b4-102">Menghapus layanan latar belakang untuk Microsoft Search di Bing</span><span class="sxs-lookup"><span data-stu-id="dc9b4-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="dc9b4-103">Untuk menghapus layanan latar belakang untuk Microsoft Search di Bing, Anda bisa mencoba solusi berikut:</span><span class="sxs-lookup"><span data-stu-id="dc9b4-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="dc9b4-104">Untuk kembali ke pengaturan mesin pencarian asli, lakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="dc9b4-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="dc9b4-105">untuk.</span><span class="sxs-lookup"><span data-stu-id="dc9b4-105">a.</span></span> <span data-ttu-id="dc9b4-106">Alihkan tombol **gunakan Bing sebagai mesin pencarian default Anda [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**.</span><span class="sxs-lookup"><span data-stu-id="dc9b4-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="dc9b4-107">b.</span><span class="sxs-lookup"><span data-stu-id="dc9b4-107">b.</span></span> <span data-ttu-id="dc9b4-108">[Masuk ke Pusat admin Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) dan Kosongkan pengaturan yang memengaruhi semua pengguna di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="dc9b4-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="dc9b4-109">Untuk menghapus layanan latar belakang dari perangkat individu, lakukan tugas-tugas berikut:</span><span class="sxs-lookup"><span data-stu-id="dc9b4-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="dc9b4-110">untuk.</span><span class="sxs-lookup"><span data-stu-id="dc9b4-110">a.</span></span> <span data-ttu-id="dc9b4-111">Pilih program **> panel kontrol > program dan fitur**.</span><span class="sxs-lookup"><span data-stu-id="dc9b4-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="dc9b4-112">b.</span><span class="sxs-lookup"><span data-stu-id="dc9b4-112">b.</span></span> <span data-ttu-id="dc9b4-113">Klik kanan **pencarian Microsoft di Bing** di bawah daftar program yang terinstal, lalu klik **hapus instalan**.</span><span class="sxs-lookup"><span data-stu-id="dc9b4-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="dc9b4-114">Untuk menghapus layanan latar belakang dari beberapa perangkat di organisasi Anda, masuk sebagai administrator dan jalankan perintah berikut dalam skrip:</span><span class="sxs-lookup"><span data-stu-id="dc9b4-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
