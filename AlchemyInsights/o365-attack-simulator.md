---
title: 2681 serangan Simulator di Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713469"
---
# <a name="attack-simulator-in-microsoft-365"></a>Serangan Simulator di Microsoft 365

- Apakah Anda hilang Attack Simulator? Attack Simulator memerlukan **office 365 Advanced ancaman Protection Plan 2 (ATP rencana 2)** atau **Office 365 Enterprise E5**. Serangan Simulator **tidak** termasuk dalam Office 365 Advanced ancaman perlindungan rencana 1 (ATP rencana 1), Office 365 Enterprise E3, atau Microsoft 365 aplikasi untuk langganan bisnis.

- Account yang Anda gunakan untuk meluncurkan simulasi serangan memerlukan global administrator atau izin administrator keamanan dan otentikasi multi faktor (MFA). Untuk informasi selengkapnya tentang persyaratan Attack Simulator, lihat [topik ini](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Hal penting yang perlu diketahui tentang **Brute Force password** Attack simulasi:

  - Jika akun target memiliki MFA diaktifkan dan sandi ditebak dengan benar, akun tidak akan ditampilkan sebagai terganggu (faktor otentikasi kedua akan tidak lengkap).

  - File sandi tidak boleh lebih dari 10 MB. Gunakan satu kata sandi per baris, dan sertakan baris kosong (carriage return) setelah kata sandi terakhir dalam daftar.

- Hal penting yang perlu diketahui tentang **tombak phishing** melampirkan simulasi:

  - Dengan desain, Anda tidak dapat memberikan nilai kustom untuk **URL server login phishing**.

  - Jika Penerima menggunakan mengaktifkan pesan [laporan Add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) untuk melaporkan pesan sebagai phishing, Anda mungkin tidak menerima peringatan untuk pesan (karena ini adalah serangan simulasi).

- Laporan: setelah serangan simulasi selesai, Anda dapat mengklik **rincian serangan** untuk melihat laporan.

- Untuk petunjuk rinci dan fitur baru dalam serangan Simulator, lihat [serangan Simulator di Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
