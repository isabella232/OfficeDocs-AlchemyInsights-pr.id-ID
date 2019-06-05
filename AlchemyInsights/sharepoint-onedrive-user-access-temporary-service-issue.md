---
title: Kinerja masalah-SharePoint atau OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719520"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint atau OneDrive lambat, tidak dapat diakses atau tersedia untuk beberapa pengguna

Jika situs OneDrive atau SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya mempunyai akses, mungkin ada masalah sementara layanan. [Periksa layanan kesehatan dashboard](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Tambahkan dan lisensi pengguna

Pastikan bahwa Anda [menetapkan lisensi ke pengguna di Office 365 untuk bisnis](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Memberikan izin

Jika pengguna telah ditetapkan lisensi Sharepoint dan masih menerima Akses ditolak pesan, pastikan mereka memiliki [tingkat izin yang sesuai](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) yang ditetapkan.

## <a name="consider-using-the-access-request-feature"></a>Pertimbangkan untuk menggunakan fitur permintaan akses

[Fitur permintaan akses](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) memungkinkan orang untuk meminta akses ke konten yang mereka saat ini tidak memiliki izin untuk melihat.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Memungkinkan script kustom dapat menyebabkan Akses ditolak masalah

Ada skenario tertentu mana fitur *script kustom Izinkan* mungkin menyajikan Akses ditolak. Untuk daftar fitur yang terpengaruh, pertimbangan keamanan dan kemampuan untuk menonaktifkan fitur. Silahkan kunjungi [Bolehkan atau mencegah script kustom](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

