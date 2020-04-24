---
title: Duplikat catatan perangkat di portal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789865"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="f1a1a-102">Duplikat catatan perangkat di portal</span><span class="sxs-lookup"><span data-stu-id="f1a1a-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="f1a1a-103">Anda mungkin melihat 2 catatan untuk sebuah perangkat di portal jika perangkat tersebut tidak melaporkan status pengelolaan bersama dengan benar ke situs Pengelola Konfigurasi.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="f1a1a-104">Untuk memeriksa status pengelolaan bersama perangkat, tinjau kolom **Dikelola Bersama** untuk perangkat di konsol Pengelola Konfigurasi.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="f1a1a-105">Jika kolom tidak terlihat, Anda dapat menambahkannya dengan mengklik kanan header kolom mana saja, lalu memilihnya dari daftar.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="f1a1a-106">Nilai Dikelola Bersama harus **Ya**.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="f1a1a-107">Jika nilainya **Tidak**, buka applet klien Pengelola Konfigurasi di perangkat klien dan periksa properti **Pengelolaan Bersama** di tab Umum.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="f1a1a-108">Jika nilainya **Diaktifkan**, ini menunjukkan masalah ada pada komunikasi klien dengan Titik Pengelolaan.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="f1a1a-109">Tinjau **CcmMessaging.log** pada perangkat untuk menyelidiki potensi masalah konektivitas.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="f1a1a-110">Jika nilainya **Dinonaktifkan** dan perangkat terdaftar di Intune, pastikan bahwa perangkat telah menerima kebijakan Pengelolaan Bersama dengan meninjau **CoManagementHandler.log** di perangkat.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
