---
title: Kirim sebagai grup Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871910"
---
# <a name="send-as-microsoft-365-group"></a>Kirim sebagai grup Microsoft 365

Anda dapat menetapkan izin Kirim sebagai untuk memperbolehkan pengguna tertentu mengirim pesan sebagai grup Microsoft 365:  

1. Menyambungkan ke Exchange Online PowerShell.  

2. Jalankan perintah berikut:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights sendas

Untuk informasi selengkapnya, lihat [memperbolehkan anggota untuk mengirimkan atau mengirim atas nama grup](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).