---
title: Mengatur Microsoft Edge sebagai browser default di perangkat macOS
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
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491556"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="6759c-102">Mengatur Microsoft Edge sebagai browser default di perangkat macOS</span><span class="sxs-lookup"><span data-stu-id="6759c-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="6759c-103">Gunakan salah satu dari dua metode ini untuk mengatur Microsoft Edge sebagai browser default:</span><span class="sxs-lookup"><span data-stu-id="6759c-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="6759c-104">Metode 1: Menge flash perangkat dengan gambar macOS tempat Microsoft Edge telah diatur sebagai browser default.</span><span class="sxs-lookup"><span data-stu-id="6759c-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="6759c-105">Metode 2: Atur kebijakan DefaultBrowserSettingEnabled untuk meminta pengguna mengatur Microsoft Edge sebagai browser default.</span><span class="sxs-lookup"><span data-stu-id="6759c-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="6759c-106">Metode ini memungkinkan pengguna mengubah browser default.</span><span class="sxs-lookup"><span data-stu-id="6759c-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="6759c-107">Untuk alasan ini, kami menyarankan agar Anda menggunakan kebijakan DefaultBrowserSettingEnabled meskipun Anda menggunakan metode 1.</span><span class="sxs-lookup"><span data-stu-id="6759c-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="6759c-108">Jika pengguna mengubah browser default setelah kebijakan disebarkan, kebijakan meminta pengguna untuk mengatur browser default kembali ke Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="6759c-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
