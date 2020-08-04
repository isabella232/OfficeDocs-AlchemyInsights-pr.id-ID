---
title: Pembersihan otomatis perangkat kedaluwarsa di Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555222"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="eaada-102">Pembersihan otomatis perangkat kedaluwarsa di Intune</span><span class="sxs-lookup"><span data-stu-id="eaada-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="eaada-103">Intune memungkinkan admin untuk mengkonfigurasi interval waktu antara 90 dan 270 hari, setelah perangkat kedaluwarsa dihapus dari layanan.</span><span class="sxs-lookup"><span data-stu-id="eaada-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="eaada-104">Pengaturan ini adalah organisasi luas dan sekali diaktifkan berlaku segera.</span><span class="sxs-lookup"><span data-stu-id="eaada-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="eaada-105">Perangkat apa pun yang tidak diperiksa ke server Intune untuk jangka waktu yang melebihi pengaturan akan dihapus secara permanen.</span><span class="sxs-lookup"><span data-stu-id="eaada-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="eaada-106">**Catatan** Hanya objek perangkat MDM yang memenuhi syarat untuk tindakan pembersihan ini.</span><span class="sxs-lookup"><span data-stu-id="eaada-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="eaada-107">EA hanya objek perangkat dikecualikan.</span><span class="sxs-lookup"><span data-stu-id="eaada-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="eaada-108">Untuk informasi tambahan saat perangkat menjadi memenuhi syarat untuk penghapusan berdasarkan pengaturan pembersihan perangkat dan "keadaan":</span><span class="sxs-lookup"><span data-stu-id="eaada-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="eaada-109">Pengaturan: **Hapus perangkat setelah tanggal Check-In terakhir: Ya (beberapa nilai (N) di hari yang ditentukan)**</span><span class="sxs-lookup"><span data-stu-id="eaada-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="eaada-110">Berdasarkan nilai (N) dikonfigurasi dalam pengaturan, Layanan Intune menghapus perangkat dalam beberapa hari setelah terakhir berhasil Check-in.</span><span class="sxs-lookup"><span data-stu-id="eaada-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="eaada-111">Pengaturan: **Hapus perangkat setelah tanggal Check-In terakhir: tidak**</span><span class="sxs-lookup"><span data-stu-id="eaada-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="eaada-112">180 hari setelah sertifikat perangkat kedaluwarsa dan tidak diperbarui, perangkat akan dihapus.</span><span class="sxs-lookup"><span data-stu-id="eaada-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="eaada-113">**Catatan** Dalam kedua kasus, perangkat harus terdaftar berhasil di Intune.</span><span class="sxs-lookup"><span data-stu-id="eaada-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="eaada-114">Pendaftaran terjadi selama checkin perangkat pertama dengan layanan Intune.</span><span class="sxs-lookup"><span data-stu-id="eaada-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="eaada-115">Jika perangkat mendaftar berhasil untuk Intune tetapi tidak menjadi Intune terdaftar, perangkat dihapus 270 hari setelah pendaftaran.</span><span class="sxs-lookup"><span data-stu-id="eaada-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="eaada-116">(90 hari untuk menandai perangkat sebagai dicabut, dan kemudian 180 hari lagi untuk menghapus catatan.)</span><span class="sxs-lookup"><span data-stu-id="eaada-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="eaada-117">Mekanisme tidak ada saat ini di konsol Intune untuk menetapkan tanggal kedaluwarsa sertifikasi perangkat untuk setiap perangkat tertentu.</span><span class="sxs-lookup"><span data-stu-id="eaada-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>