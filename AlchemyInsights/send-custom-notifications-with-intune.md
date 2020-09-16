---
title: Mengirim pemberitahuan kustom dengan Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720649"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="e8d97-102">Cara mengirim pemberitahuan kustom kepada pengguna perangkat iOS dan Android yang dikelola</span><span class="sxs-lookup"><span data-stu-id="e8d97-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="e8d97-103">Pemberitahuan kustom untuk Intune diproses oleh aplikasi portal perusahaan di perangkat pengguna.</span><span class="sxs-lookup"><span data-stu-id="e8d97-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="e8d97-104">Aplikasi tersebut membuat pemberitahuan push pada perangkat tersebut.</span><span class="sxs-lookup"><span data-stu-id="e8d97-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="e8d97-105">Berikut ini adalah prasyarat perangkat untuk mendukung penerimaan pemberitahuan kustom, dan untuk aplikasi untuk membuat pemberitahuan push:</span><span class="sxs-lookup"><span data-stu-id="e8d97-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="e8d97-106">Perangkat harus menginstal aplikasi portal perusahaan.</span><span class="sxs-lookup"><span data-stu-id="e8d97-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="e8d97-107">Perangkat harus memperbolehkan aplikasi portal perusahaan mengirimkan pemberitahuan push.</span><span class="sxs-lookup"><span data-stu-id="e8d97-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="e8d97-108">Saat aplikasi terinstal atau diperbarui, aplikasi akan meminta pengguna untuk memperbolehkan pemberitahuan.</span><span class="sxs-lookup"><span data-stu-id="e8d97-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="e8d97-109">Perangkat Android harus menginstal Google Play Services.</span><span class="sxs-lookup"><span data-stu-id="e8d97-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="e8d97-110">Perangkat harus didaftarkan dengan Intune.</span><span class="sxs-lookup"><span data-stu-id="e8d97-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="e8d97-111">Untuk informasi selengkapnya, termasuk cara mengirim pesan, lihat [dokumentasi fitur](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="e8d97-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
