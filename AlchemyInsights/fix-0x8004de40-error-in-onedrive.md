---
title: Memperbaiki 0x8004de40 di OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649751"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Memperbaiki 0x8004de40 di OneDrive

Jika Anda menjalankan Windows 7 dan menerima kesalahan ini, Perbarui untuk mengaktifkan [TLS 1.1 dan TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)sebagai protokol aman default di WinHTTP di Windows .

Jika menjalankan Windows 10, dan Anda menerima pesan kesalahan 0x8004de40 OneDrive:

- Me-reboot komputer yang terpengaruh saat tersambung ke domain Direktori Acitve Anda.
- Jika mulai ulang tidak memperbaiki masalah, sambungkan kembali dan bergabung kembali ke perangkat Anda dari Azure AD. 

**Catatan:** Anda harus berada di jaringan perusahaan Anda sambil melakukan langkah-langkah ini. Jangan lakukan langkah-langkah ini saat Anda tidak tersambung ke infrastruktur perusahaan (misalnya, saat berpergian). 

1. Buka prompt perintah yang ditinggikan dengan **memilih Mulai**, klik kanan **Prompt Perintah**, lalu pilih Jalankan **sebagai administrator**.

1. Ketik *dsregcmd /leave* dan tekan **Enter**.

1. Bila sudah selesai, *ketik dsregcmd /join* lalu tekan **Enter**.

1. Setelah selesai, tutup prompt perintah.

1. Me-reboot komputer, dan masuk ke OneDrive.