---
title: Masalah kinerja-SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771247"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="29b23-102">SharePoint atau OneDrive lambat, tidak dapat diakses, atau tidak tersedia untuk beberapa pengguna</span><span class="sxs-lookup"><span data-stu-id="29b23-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="29b23-103">Jika OneDrive atau situs SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki Access, mungkin ada masalah layanan sementara.</span><span class="sxs-lookup"><span data-stu-id="29b23-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="29b23-104">[Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="29b23-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="29b23-105">**Menambahkan dan melisensikan pengguna**</span><span class="sxs-lookup"><span data-stu-id="29b23-105">**Add and license the user**</span></span>

<span data-ttu-id="29b23-106">Pastikan Anda [menetapkan lisensi kepada pengguna di Microsoft 365 for Business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="29b23-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="29b23-107">**Tetapkan izin**</span><span class="sxs-lookup"><span data-stu-id="29b23-107">**Assign Permissions**</span></span>

<span data-ttu-id="29b23-108">Jika pengguna telah diberi lisensi SharePoint dan masih menerima pesan Akses ditolak, pastikan mereka memiliki [tingkat izin yang sesuai](https://docs.microsoft.com/sharepoint/understanding-permission-levels) yang ditetapkan.</span><span class="sxs-lookup"><span data-stu-id="29b23-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="29b23-109">**Pertimbangkan menggunakan fitur permintaan Access**</span><span class="sxs-lookup"><span data-stu-id="29b23-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="29b23-110">[Fitur permintaan Access](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) memungkinkan orang untuk meminta akses ke konten yang saat ini tidak memiliki izin untuk dilihat.</span><span class="sxs-lookup"><span data-stu-id="29b23-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="29b23-111">**Memperbolehkan skrip kustom mungkin menyebabkan masalah Akses ditolak**</span><span class="sxs-lookup"><span data-stu-id="29b23-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="29b23-112">Ada beberapa skenario di mana fitur *Izinkan skrip kustom* mungkin menyajikan Akses ditolak.</span><span class="sxs-lookup"><span data-stu-id="29b23-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="29b23-113">Untuk daftar fitur yang terpengaruh, pertimbangan keamanan dan kemampuan untuk menonaktifkan fitur.</span><span class="sxs-lookup"><span data-stu-id="29b23-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="29b23-114">Silakan kunjungi [Izinkan atau Cegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="29b23-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

