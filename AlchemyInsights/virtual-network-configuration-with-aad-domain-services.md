---
title: Konfigurasi virtual dengan layanan domain AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885205"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Konfigurasi virtual dengan layanan domain AAD

Konfigurasi virtual dengan layanan domain AAD melibatkan langkah-langkah berikut: 

1. Memeriksa kesehatan domain Anda di portal Azure https://aka.ms/aadds-health
2. Memeriksa NSG Anda untuk aturan yang memblokir port yang diperlukan untuk menyinkronkan di layanan domain Azure AD pada portal https://aka.ms/aadds-networking
3. Memastikan bahwa jaringan virtual Anda disebarkan di kawasan Azure yang sama dengan domain Azure AD domain terkelola layanan Anda.
4. Memastikan Anda tidak memiliki domain yang ada dengan nama domain yang sama yang tersedia di jaringan virtual.

Untuk detail selengkapnya tentang pertimbangan desain pada jaringan virtual Azure untuk mendukung layanan domain AAD, lihat [pertimbangan jaringan virtual](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

