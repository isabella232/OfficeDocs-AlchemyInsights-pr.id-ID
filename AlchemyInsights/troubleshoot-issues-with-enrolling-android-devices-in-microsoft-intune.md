---
title: Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759623"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="16b7e-102">Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="16b7e-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="16b7e-103">Tinjau sumber daya yang tercantum di bawah ini untuk menyelesaikan masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="16b7e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="16b7e-104">Beberapa masalah umum dan langkah penyelesaian:</span><span class="sxs-lookup"><span data-stu-id="16b7e-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="16b7e-105">**Perangkat tidak dienkripsi kesalahan di portal perusahaan:** Versi Android yang lebih baru, khususnya dimulai dengan v 7.0, memerlukan kode sandi mulai untuk memastikan perangkat Anda dienkripsi sepenuhnya.</span><span class="sxs-lookup"><span data-stu-id="16b7e-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="16b7e-106">Solusi umum adalah untuk mengaktifkan pin startup atau sepenuhnya mengenkripsi perangkat.</span><span class="sxs-lookup"><span data-stu-id="16b7e-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="16b7e-107">Tinjau [dokumen ini](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="16b7e-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="16b7e-108">**Perangkat gagal untuk Check-in dengan layanan Intune atau menampilkan sebagai "tidak sehat" di konsol admin Intune:** Beberapa Samsung 4,4 dan perangkat 5,5 mungkin tidak memeriksa ke dalam layanan.</span><span class="sxs-lookup"><span data-stu-id="16b7e-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="16b7e-109">Ada 3 kemungkinan solusi untuk masalah ini:</span><span class="sxs-lookup"><span data-stu-id="16b7e-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="16b7e-110">Buka aplikasi portal perusahaan Intune secara manual, yang akan memulai sinkronisasi perangkat secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="16b7e-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="16b7e-111">Perbarui perangkat ke Android 6,0 atau versi yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="16b7e-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="16b7e-112">Nonaktifkan Samsung Smart Manager mengelola Intune portal perusahaan.</span><span class="sxs-lookup"><span data-stu-id="16b7e-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="16b7e-113">Tinjau [dokumen ini](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) untuk detail lebih lanjut tentang masalah dan resolusi ini.</span><span class="sxs-lookup"><span data-stu-id="16b7e-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="16b7e-114">**Jenis lisensi pengguna tidak valid** atau **nama pengguna tidak dikenali galat:** pengguna harus ditetapkan lisensi Intune atau EMS.</span><span class="sxs-lookup"><span data-stu-id="16b7e-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="16b7e-115">Tinjau dokumen ini untuk menetapkan lisensi melalui: Pusat admin Office atau Azure portal.</span><span class="sxs-lookup"><span data-stu-id="16b7e-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="16b7e-116">Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="16b7e-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="16b7e-117">Gunakan [Intune pemecahan masalah portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan menyelesaikan umum kegagalan pendaftaran.</span><span class="sxs-lookup"><span data-stu-id="16b7e-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="16b7e-118">Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="16b7e-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="16b7e-119">Tinjau [dokumen ini](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing.</span><span class="sxs-lookup"><span data-stu-id="16b7e-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="16b7e-120">[Pelajari cara mendaftarkan perangkat Android di Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="16b7e-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
