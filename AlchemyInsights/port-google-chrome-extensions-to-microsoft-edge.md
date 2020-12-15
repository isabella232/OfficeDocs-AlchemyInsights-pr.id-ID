---
title: Memindahkan ekstensi Google Chrome ke Microsoft Edge (Kromium)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677878"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="b4195-102">Memindahkan ekstensi Google Chrome ke Microsoft Edge (Kromium)</span><span class="sxs-lookup"><span data-stu-id="b4195-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="b4195-103">Mudah untuk [memindahkan ekstensi Google Chrome ke Microsoft Edge (Kromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="b4195-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="b4195-104">Dalam kebanyakan kasus, hanya sedikit perubahan yang diperlukan untuk menjalankan ekstensi ini di Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b4195-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="b4195-105">Api ekstensi dan tombol manifest yang didukung oleh Google Chrome kompatibel dengan kode Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b4195-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="b4195-106">Namun, Microsoft Edge tidak mendukung ekstensi APIs Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken, dan Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="b4195-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>