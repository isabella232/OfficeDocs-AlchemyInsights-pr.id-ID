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
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079453"
---
# <a name="encryption-with-transport-rules"></a>Enkripsi dengan aturan transportasi

Di [Pusat Admin Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), Anda dapat menggunakan kemampuan Enkripsi Pesan Office (OME) di aturan aliran email untuk memicu enkripsi pesan. Pilih opsi **Terapkan Enkripsi Pesan dan perlindungan hak Office 365** pada kondisi Aturan Transportasi.

- Untuk informasi selengkapnya, lihat [Menentukan Aturan aliran email untuk mengenkripsi](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Di PowerShell, gunakan cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) dan atur parameter *ApplyOME* ke $true.
