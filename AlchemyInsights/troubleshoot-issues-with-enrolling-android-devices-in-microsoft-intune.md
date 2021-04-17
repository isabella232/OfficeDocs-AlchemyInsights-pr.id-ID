---
title: Memecahkan masalah pendaftaran perangkat Android di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830945"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="bc9ff-102">Memecahkan masalah pendaftaran perangkat Android di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bc9ff-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="bc9ff-103">Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="bc9ff-104">Beberapa masalah umum dan langkah-langkah penyelesaian:</span><span class="sxs-lookup"><span data-stu-id="bc9ff-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="bc9ff-105">**Kesalahan Perangkat tidak Dienkripsi di Portal Perusahaan:** Versi android yang lebih baru, terutama yang dimulai dengan v7.0, memerlukan kode akses mulai untuk memastikan bahwa perangkat Anda dienkripsi sepenuhnya.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="bc9ff-106">Solusi umum adalah mengaktifkan pin mulai atau mengenkripsi perangkat sepenuhnya.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="bc9ff-107">Tinjau [dokumen ini](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="bc9ff-108">**Perangkat tidak dapat masuk dengan layanan Intune atau ditampilkan sebagai "Tidak sehat" di konsol admin Intune:** Beberapa perangkat Samsung 4.4 dan 5.5 mungkin tidak masuk ke layanan.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="bc9ff-109">Ada 3 solusi yang memungkinkan untuk masalah ini:</span><span class="sxs-lookup"><span data-stu-id="bc9ff-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="bc9ff-110">Buka aplikasi Intune Company Portal secara manual, yang akan memulai sinkronisasi perangkat secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="bc9ff-111">Perbarui perangkat ke Android 6.0 atau yang lebih tinggi.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="bc9ff-112">Nonaktifkan Samsung Smart Manager dari mengelola Portal Perusahaan Intune.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="bc9ff-113">Tinjau [dokumen ini](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) untuk detail selengkapnya mengenai masalah dan resolusi ini.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="bc9ff-114">**Kesalahan Tipe Lisensi Pengguna** Tidak Valid atau Nama Pengguna Tidak **Dikenali:** Pengguna perlu diberi lisensi Intune atau EMS.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="bc9ff-115">Tinjau dokumen ini untuk menetapkan lisensi melalui: Pusat Admin Office atau portal Azure.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="bc9ff-116">Sumber daya tambahan untuk membantu mengatasi masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="bc9ff-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bc9ff-117">Gunakan [Portal Pemecahan Masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bc9ff-118">Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="bc9ff-119">Tinjau [dokumen](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing.</span><span class="sxs-lookup"><span data-stu-id="bc9ff-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="bc9ff-120">[Pelajari cara mendaftarkan perangkat Android di Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="bc9ff-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
