---
title: Enkripsi dengan aturan transportasi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813871"
---
# <a name="encryption-with-transport-rules"></a>Enkripsi dengan aturan transportasi

Di [Pusat Admin Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), Anda dapat menggunakan kemampuan Enkripsi Pesan Office (OME) di aturan aliran email untuk memicu enkripsi pesan. Pilih opsi **Terapkan Enkripsi Pesan dan perlindungan hak Office 365** pada kondisi Aturan Transportasi.

- Untuk informasi selengkapnya, lihat [Menentukan Aturan aliran email untuk mengenkripsi](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Di PowerShell, gunakan cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) dan atur parameter *ApplyOME* ke $true.
