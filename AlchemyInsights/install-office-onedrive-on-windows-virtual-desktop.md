---
title: Menginstal Office dan OneDrive di Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595848"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Menginstal Office dan OneDrive di Windows Virtual Desktop

1. [Mempersiapkan dan mengustomisasi gambar VHD master](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Buat mesin virtual (VM) jika belum dibuat.

1. [Menginstal Office dalam mode aktivasi komputer bersama.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Aktivasi komputer bersama memungkinkan beberapa pengguna mengakses Office.

1. [Instal OneDrive dalam mode per komputer.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) Biasanya OneDrive diinstal per pengguna, namun di sini, OneDrive harus diinstal per komputer.