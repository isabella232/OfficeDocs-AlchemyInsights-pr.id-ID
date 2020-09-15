---
title: Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689957"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="c39b4-102">Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c39b4-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="c39b4-103">Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="c39b4-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="c39b4-104">Beberapa masalah umum dan langkah pemecahan masalah:</span><span class="sxs-lookup"><span data-stu-id="c39b4-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="c39b4-105">**Kesalahan perangkat tidak dienkripsi di portal perusahaan:** Versi Android yang lebih baru, terutama diawali dengan v 7.0, memerlukan kode akses untuk memastikan bahwa perangkat Anda dienkripsi penuh.</span><span class="sxs-lookup"><span data-stu-id="c39b4-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="c39b4-106">Solusi umum adalah untuk mengaktifkan pin startup atau mengenkripsi penuh perangkat.</span><span class="sxs-lookup"><span data-stu-id="c39b4-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="c39b4-107">Tinjau [dokumen ini](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="c39b4-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="c39b4-108">**Perangkat gagal Check-in dengan layanan Intune atau ditampilkan sebagai "tidak sehat" di konsol admin Intune:** Beberapa perangkat Samsung 4,4 dan 5,5 mungkin tidak memeriksa layanan.</span><span class="sxs-lookup"><span data-stu-id="c39b4-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="c39b4-109">Ada 3 solusi yang memungkinkan untuk masalah ini:</span><span class="sxs-lookup"><span data-stu-id="c39b4-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="c39b4-110">Buka aplikasi Intune Company portal secara manual, yang akan memulai sinkronisasi perangkat secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="c39b4-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="c39b4-111">Perbarui perangkat ke Android 6,0 atau yang lebih tinggi.</span><span class="sxs-lookup"><span data-stu-id="c39b4-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="c39b4-112">Nonaktifkan Samsung Smart Manager dari mengelola portal perusahaan Intune.</span><span class="sxs-lookup"><span data-stu-id="c39b4-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="c39b4-113">Tinjau [dokumen ini](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) untuk detail lebih lanjut tentang masalah dan resolusi ini.</span><span class="sxs-lookup"><span data-stu-id="c39b4-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="c39b4-114">**Lisensi pengguna ketik** **nama pengguna tidak valid atau tidak dikenali kesalahan:** pengguna harus diberi lisensi Intune atau EMS.</span><span class="sxs-lookup"><span data-stu-id="c39b4-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c39b4-115">Tinjau dokumen ini untuk menetapkan lisensi melalui: Pusat admin Office atau Azure portal.</span><span class="sxs-lookup"><span data-stu-id="c39b4-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="c39b4-116">Sumber daya tambahan untuk membantu mengatasi masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="c39b4-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c39b4-117">Gunakan [portal pemecahan masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum.</span><span class="sxs-lookup"><span data-stu-id="c39b4-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c39b4-118">Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="c39b4-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="c39b4-119">Tinjau [dokumen ini](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing.</span><span class="sxs-lookup"><span data-stu-id="c39b4-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="c39b4-120">[Pelajari cara mendaftarkan perangkat Android di Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="c39b4-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
