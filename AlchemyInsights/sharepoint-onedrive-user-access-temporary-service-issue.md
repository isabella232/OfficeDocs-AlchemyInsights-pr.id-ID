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
ms.openlocfilehash: 9bb18196f38de473e4ee79d77bd43561ad9742e0
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223283"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="ff4d0-102">SharePoint atau OneDrive lambat, tidak dapat diakses atau tersedia untuk beberapa pengguna</span><span class="sxs-lookup"><span data-stu-id="ff4d0-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="ff4d0-103">Jika situs OneDrive atau SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya mempunyai akses, mungkin ada masalah sementara layanan.</span><span class="sxs-lookup"><span data-stu-id="ff4d0-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="ff4d0-104">[Periksa layanan kesehatan dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ff4d0-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="ff4d0-105">**Tambahkan dan lisensi pengguna**</span><span class="sxs-lookup"><span data-stu-id="ff4d0-105">**Add and license the user**</span></span>

<span data-ttu-id="ff4d0-106">Pastikan bahwa Anda [menetapkan lisensi ke pengguna di Office 365 untuk bisnis](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="ff4d0-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="ff4d0-107">**Memberikan izin**</span><span class="sxs-lookup"><span data-stu-id="ff4d0-107">**Assign Permissions**</span></span>

<span data-ttu-id="ff4d0-108">Jika pengguna telah ditetapkan lisensi Sharepoint dan masih menerima Akses ditolak pesan, pastikan mereka memiliki [tingkat izin yang sesuai](https://docs.microsoft.com/sharepoint/understanding-permission-levels) yang ditetapkan.</span><span class="sxs-lookup"><span data-stu-id="ff4d0-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="ff4d0-109">**Pertimbangkan untuk menggunakan fitur permintaan akses**</span><span class="sxs-lookup"><span data-stu-id="ff4d0-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="ff4d0-110">[Fitur permintaan akses](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) memungkinkan orang untuk meminta akses ke konten yang mereka saat ini tidak memiliki izin untuk melihat.</span><span class="sxs-lookup"><span data-stu-id="ff4d0-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="ff4d0-111">**Memungkinkan script kustom dapat menyebabkan Akses ditolak masalah**</span><span class="sxs-lookup"><span data-stu-id="ff4d0-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="ff4d0-112">Ada skenario tertentu mana fitur *script kustom Izinkan* mungkin menyajikan Akses ditolak.</span><span class="sxs-lookup"><span data-stu-id="ff4d0-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="ff4d0-113">Untuk daftar fitur yang terpengaruh, pertimbangan keamanan dan kemampuan untuk menonaktifkan fitur.</span><span class="sxs-lookup"><span data-stu-id="ff4d0-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="ff4d0-114">Silahkan kunjungi [Bolehkan atau mencegah script kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="ff4d0-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

