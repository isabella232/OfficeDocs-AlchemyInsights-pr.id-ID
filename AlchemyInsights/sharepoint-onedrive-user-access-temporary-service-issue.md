---
title: Masalah kinerja-SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511151"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="ce2e1-102">SharePoint atau OneDrive lambat, tidak dapat diakses atau tidak tersedia untuk banyak pengguna</span><span class="sxs-lookup"><span data-stu-id="ce2e1-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="ce2e1-103">Jika OneDrive atau situs SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki akses, mungkin ada masalah layanan sementara.</span><span class="sxs-lookup"><span data-stu-id="ce2e1-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="ce2e1-104">[Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ce2e1-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="ce2e1-105">**Menambahkan dan melisensikan pengguna**</span><span class="sxs-lookup"><span data-stu-id="ce2e1-105">**Add and license the user**</span></span>

<span data-ttu-id="ce2e1-106">Pastikan bahwa Anda [menetapkan lisensi untuk pengguna di Microsoft 365 untuk bisnis](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="ce2e1-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="ce2e1-107">**Menetapkan izin**</span><span class="sxs-lookup"><span data-stu-id="ce2e1-107">**Assign Permissions**</span></span>

<span data-ttu-id="ce2e1-108">Jika pengguna telah ditetapkan lisensi SharePoint dan masih menerima pesan Akses ditolak, pastikan mereka memiliki [tingkat izin yang sesuai](https://docs.microsoft.com/sharepoint/understanding-permission-levels) yang ditetapkan.</span><span class="sxs-lookup"><span data-stu-id="ce2e1-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="ce2e1-109">**Pertimbangkan untuk menggunakan fitur permintaan akses**</span><span class="sxs-lookup"><span data-stu-id="ce2e1-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="ce2e1-110">[Fitur permintaan akses](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) memungkinkan orang untuk meminta akses ke konten yang saat ini tidak diizinkan untuk dilihat.</span><span class="sxs-lookup"><span data-stu-id="ce2e1-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="ce2e1-111">**Memungkinkan skrip kustom dapat menyebabkan masalah Akses ditolak**</span><span class="sxs-lookup"><span data-stu-id="ce2e1-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="ce2e1-112">Ada skenario tertentu mana fitur *memungkinkan kustom skrip* mungkin menyajikan Akses ditolak.</span><span class="sxs-lookup"><span data-stu-id="ce2e1-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="ce2e1-113">Untuk daftar fitur yang terpengaruh, pertimbangan keamanan dan kemampuan untuk menonaktifkan fitur.</span><span class="sxs-lookup"><span data-stu-id="ce2e1-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="ce2e1-114">Silakan kunjungi [Izinkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="ce2e1-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

