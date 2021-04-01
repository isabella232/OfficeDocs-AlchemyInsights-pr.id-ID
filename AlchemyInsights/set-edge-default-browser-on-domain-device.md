---
title: Menetapkan Microsoft Edge sebagai browser default pada perangkat yang bergabung dalam domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491583"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="2cb6a-102">Menetapkan Microsoft Edge sebagai browser default pada perangkat yang bergabung dalam domain</span><span class="sxs-lookup"><span data-stu-id="2cb6a-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="2cb6a-103">Atur Microsoft Edge sebagai browser default:</span><span class="sxs-lookup"><span data-stu-id="2cb6a-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="2cb6a-104">[Buat asosiasi file konfigurasi default dan](https://go.microsoft.com/fwlink/?linkid=2132437) simpan file secara lokal atau di jaringan bersama.</span><span class="sxs-lookup"><span data-stu-id="2cb6a-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="2cb6a-105">Buka editor Kebijakan Grup, lalu masuk ke **Komputer Templat**  >  **Administratif Komponen**  >  **Windows**  >  **File Explorer.**</span><span class="sxs-lookup"><span data-stu-id="2cb6a-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="2cb6a-106">Pilih **Atur file konfigurasi asosiasi default.**</span><span class="sxs-lookup"><span data-stu-id="2cb6a-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="2cb6a-107">Pilih **Pengaturan kebijakan**, lalu pilih **Diaktifkan.**</span><span class="sxs-lookup"><span data-stu-id="2cb6a-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="2cb6a-108">Di **bawah** Opsi, masukkan lokasi asosiasi file konfigurasi default Anda, lalu pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="2cb6a-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
