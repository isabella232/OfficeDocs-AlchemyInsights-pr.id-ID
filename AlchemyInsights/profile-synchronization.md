---
title: Sinkronisasi profil
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923647"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kapan perubahan profil saya disinkronkan ke SharePoint Profil Pengguna saya?

SharePoint Online menggunakan pekerjaan pengatur waktu Impor Direktori Aktif (Impor AD) untuk mengimpor pengguna dan grup ke dalam Aplikasi Profil Pengguna. 
  
1. Impor AD menyinkronkan perubahan dari SharePoint Online Directory Store ke Aplikasi Profil Pengguna. Perubahan ini diproses dalam kumpulan.
    
2. Pekerjaan pengatur waktu berjalan hingga perubahan disinkronkan.
    
> [!NOTE]
> Waktu yang dibutuhkan untuk menjalankan pekerjaan bergantung pada jumlah perubahan yang diproses. Perubahan dalam jumlah besar membutuhkan waktu lebih lama. Perjanjian Tingkat Layanan (SLA, Service Level Agreement) menyatakan bahwa perubahan untuk pengguna di Direktori SharePoint Online akan dicerminkan dalam Aplikasi Profil Pengguna dalam 24 jam. 
  
[Info selengkapnya tentang sinkronisasi profil pengguna di SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

