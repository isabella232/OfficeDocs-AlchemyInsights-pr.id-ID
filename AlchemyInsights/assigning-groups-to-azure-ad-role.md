---
title: Menetapkan grup untuk peran Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036243"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Menetapkan grup untuk peran Azure AD

Untuk menetapkan grup Azure AD dengan sumber otoritas dalam Azure AD ke peran Azure AD, lakukan langkah-langkah berikut ini:

1. Membuat grup baru - Untuk membuat grup baru:

    a. Masuk ke pusat admin Azure AD dengan administrator **peran yang memiliki hak istimewa** atau izin administrator **global.**
    b. Pilih **Azure Active Directory > Baru > Semua > grup Baru.**
    c. Buat grup.

2. Tetapkan peran ke grup baik selama pembuatan grup atau setelah grup dibuat.

    a. Untuk menetapkan peran ke grup pada saat pembuatan grup, aktifkan tombol alih peran Azure AD yang dapat ditetapkan **ke grup dan** buat grup.
    b. Untuk menetapkan peran ke grup setelah dibuat, navigasikan ke **tab** Peran yang ditetapkan untuk grup yang baru dibuat, dan tetapkan peran ke grup.  

**Mengelola keanggotaan grup yang ditetapkan pada peran Azure AD**

Untuk mencegah peningkatan hak istimewa, secara default, hanya administrator peran yang memiliki hak istimewa dan administrator global yang dapat mengubah keanggotaan grup yang ditetapkan menjadi sebuah peran. Namun, mereka bisa memilih untuk menugaskan pemilik untuk grup tersebut dan mendelegasikan tugas ini.

Untuk detail selengkapnya tentang menetapkan grup awan ke peran Azure AD, lihat [Menetapkan peran AD ke Grup Awan.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Untuk detail selengkapnya tentang peran pemecahan masalah yang ditetapkan ke grup awan, lihat [Memecahkan masalah peran yang ditetapkan untuk grup awan.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





