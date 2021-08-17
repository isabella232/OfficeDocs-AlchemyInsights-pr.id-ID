---
title: Kebijakan kata sandi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040833"
---
# <a name="password-policies"></a>Kebijakan kata sandi

**Saya mengalami masalah dengan kebijakan kata sandi untuk pengguna**

- Kebijakan kata sandi untuk pengguna bergantung pada apakah pengguna hanya awan atau lokal.
- Hanya pengguna cloud saja yang harus memilih kata sandi yang memenuhi persyaratan dalam artikel ini: [Kebijakan kata sandi yang hanya berlaku untuk akun pengguna awan](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Pengguna di tempat harus memilih kata sandi yang memenuhi persyaratan lokal. Jika pengguna lokal tidak dapat mengatur kata sandinya, periksa persyaratan lokal Anda.

**Saya tidak tahu cara mengatur atau memeriksa kebijakan kedaluwarsa kata sandi**

- Anda bisa mengatur dan memeriksa kebijakan kedaluwarsa untuk pengguna awan di penyewa Anda dengan menggunakan PowerShell. Ikuti instruksi dalam artikel ini: [Mengatur atau memeriksa kebijakan kata sandi menggunakan PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Kebijakan kedaluwarsa kata sandi untuk pengguna di tempat diatur di AD lokal Anda.

**Link Berguna Lainnya:**
- [Mulai Menggunakan Pengaturan Ulang Kata Sandi](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Pemecahan masalah Pengaturan Ulang Kata Sandi yang dimulai administrator](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
