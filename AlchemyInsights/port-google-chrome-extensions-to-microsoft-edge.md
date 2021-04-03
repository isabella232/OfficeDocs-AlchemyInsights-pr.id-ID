---
title: Port ekstensi Google Chrome ke Microsoft Edge (Chromium)
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
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505287"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Port ekstensi Google Chrome ke Microsoft Edge (Chromium)

Mudah untuk port ekstensi [Google Chrome ke Microsoft Edge (Chromium).](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension) Dalam sebagian besar kasus, hanya perubahan minimal yang diperlukan untuk menjalankan ekstensi ini di Microsoft Edge.

API ekstensi dan tombol manifes yang didukung oleh Google Chrome kompatibel dengan kode dengan Microsoft Edge. Namun, Microsoft Edge tidak mendukung API ekstensi chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, dan chrome.instanceID.