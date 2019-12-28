---
title: Kirim pemberitahuan kustom dengan Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886860"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="cfb07-102">Cara mengirim pemberitahuan kustom ke pengguna perangkat iOS dan Android yang dikelola</span><span class="sxs-lookup"><span data-stu-id="cfb07-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="cfb07-103">Pemberitahuan kustom untuk Intune diproses oleh aplikasi portal perusahaan di perangkat pengguna.</span><span class="sxs-lookup"><span data-stu-id="cfb07-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="cfb07-104">Aplikasi ini kemudian membuat pemberitahuan push pada perangkat tersebut.</span><span class="sxs-lookup"><span data-stu-id="cfb07-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="cfb07-105">Berikut adalah prasyarat perangkat untuk mendukung penerimaan pemberitahuan kustom, dan untuk aplikasi kemudian membuat pemberitahuan push:</span><span class="sxs-lookup"><span data-stu-id="cfb07-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="cfb07-106">Perangkat harus memiliki aplikasi portal perusahaan yang diinstal.</span><span class="sxs-lookup"><span data-stu-id="cfb07-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="cfb07-107">Perangkat harus mengizinkan aplikasi portal perusahaan untuk mengirim pemberitahuan push.</span><span class="sxs-lookup"><span data-stu-id="cfb07-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="cfb07-108">Ketika aplikasi diinstal atau diperbarui, itu akan meminta pengguna untuk mengizinkan pemberitahuan.</span><span class="sxs-lookup"><span data-stu-id="cfb07-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="cfb07-109">Perangkat Android harus memiliki layanan Google Play terinstal.</span><span class="sxs-lookup"><span data-stu-id="cfb07-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="cfb07-110">Perangkat harus terdaftar dengan Intune.</span><span class="sxs-lookup"><span data-stu-id="cfb07-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="cfb07-111">Untuk informasi selengkapnya, termasuk cara mengirim pesan, lihat [dokumentasi fitur](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="cfb07-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
