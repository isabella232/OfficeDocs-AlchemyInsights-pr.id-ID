---
title: Penggunaan aplikasi Win32 Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461871"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="1a090-102">Penggunaan aplikasi Win32 Win32</span><span class="sxs-lookup"><span data-stu-id="1a090-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="1a090-103">Microsoft Intune memperbolehkan aplikasi Win32, termasuk tetapi tidak terbatas pada MSI dan. EXE akan disebarkan ke perangkat Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1a090-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="1a090-104">Mekanisme penyebaran yang digunakan memerlukan ekstensi manajemen Intune (IME) untuk hadir pada perangkat target.</span><span class="sxs-lookup"><span data-stu-id="1a090-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="1a090-105">IME akan diinstal secara otomatis sebagai hasil dari menargetkan skrip PowerShell atau penerapan aplikasi Win32 ke pengguna/perangkat.</span><span class="sxs-lookup"><span data-stu-id="1a090-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="1a090-106">Ada juga rangkaian prasyarat yang harus dipenuhi untuk menyebarkan aplikasi Win32 yang meliputi:</span><span class="sxs-lookup"><span data-stu-id="1a090-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="1a090-107">Platform yang didukung: Windows 10 versi 1607 atau yang lebih baru (versi Enterprise, Pro, dan pendidikan).</span><span class="sxs-lookup"><span data-stu-id="1a090-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="1a090-108">Arsitektur yang didukung: x86 dan x64.</span><span class="sxs-lookup"><span data-stu-id="1a090-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="1a090-109">Manajemen perangkat: AAD bergabung dan didaftarkan secara otomatis (termasuk domain hibrid bergabung dan kebijakan grup didaftarkan secara otomatis).</span><span class="sxs-lookup"><span data-stu-id="1a090-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="1a090-110">Format paket aplikasi:. file **intunewin**  disiapkan oleh [alat penyiapan konten Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="1a090-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="1a090-111">Terbatas</span><span class="sxs-lookup"><span data-stu-id="1a090-111">Limitations:</span></span>
    - <span data-ttu-id="1a090-112">Ukuran maksimum: 8GB.</span><span class="sxs-lookup"><span data-stu-id="1a090-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="1a090-113">Arsitektur tidak didukung: ARMs.</span><span class="sxs-lookup"><span data-stu-id="1a090-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="1a090-114">Tinjau dokumen "[Tambahkan, tetapkan, dan Pantau aplikasi Win32 di Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" untuk informasi yang terkait dengan langkah-langkah tersebut.</span><span class="sxs-lookup"><span data-stu-id="1a090-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="1a090-115">Detail tentang pemecahan masalah penyebaran aplikasi di Windows termasuk aplikasi Win32 dapat ditinjau dalam dokumen berikut</span><span class="sxs-lookup"><span data-stu-id="1a090-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="1a090-116">Memecahkan masalah penginstalan aplikasi</span><span class="sxs-lookup"><span data-stu-id="1a090-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="1a090-117">Memecahkan masalah aplikasi Win32</span><span class="sxs-lookup"><span data-stu-id="1a090-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)