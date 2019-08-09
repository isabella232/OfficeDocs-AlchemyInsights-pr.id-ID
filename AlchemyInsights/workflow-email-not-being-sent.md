---
title: Alur kerja email tidak dikirim
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270675"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="7e07c-102">Alur kerja email tidak dikirim</span><span class="sxs-lookup"><span data-stu-id="7e07c-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="7e07c-103">Email dari alur kerja tidak dikirim ke semua pengguna atau hanya pengguna tertentu, atau Anda melihat kesalahan **pesan e-mail tidak dapat dikirim. Pastikan e-mail memiliki Penerima berlaku**.</span><span class="sxs-lookup"><span data-stu-id="7e07c-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="7e07c-104">Periksa jika pengguna yang ada di grup izin **Semua orang** (daftar informasi pengguna) untuk koleksi situs itu.</span><span class="sxs-lookup"><span data-stu-id="7e07c-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="7e07c-105">Contoh URL langsung: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="7e07c-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="7e07c-106">Jika pengguna tidak ada, pastikan pengguna masuk ke halaman.</span><span class="sxs-lookup"><span data-stu-id="7e07c-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="7e07c-107">Jika pengguna eksternal, pastikan bahwa undangan telah diterima.</span><span class="sxs-lookup"><span data-stu-id="7e07c-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="7e07c-108">Jika pengguna ada di kelompok izin, pastikan alamat email benar.</span><span class="sxs-lookup"><span data-stu-id="7e07c-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="7e07c-109">Jika alamat email pengguna yang tidak diatur di sini, kemudian membuat lansiran sampel untuk pengguna yang yang pasukan sync account pengguna tersebut dari profil pengguna SharePoint untuk koleksi situs ini.</span><span class="sxs-lookup"><span data-stu-id="7e07c-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="7e07c-110">Email dari alur kerja akan dikirim ke administrator koleksi situs tapi tidak untuk pengguna lain dan melihat kesalahan \*\*HTTP terlarang untuk <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="7e07c-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="7e07c-111">Lihat [Akses ditolak ketika email yang dikirim ke grup](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="7e07c-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="7e07c-112">Juga, pastikan **akses terbatas pengguna izin kuncian modus** situs koleksi fitur tidak aktif.</span><span class="sxs-lookup"><span data-stu-id="7e07c-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="7e07c-113">Topik terkait</span><span class="sxs-lookup"><span data-stu-id="7e07c-113">Related topics</span></span>
<span data-ttu-id="7e07c-114">Ingin mencoba Microsoft Flow di SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="7e07c-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="7e07c-115">Menciptakan aliran</span><span class="sxs-lookup"><span data-stu-id="7e07c-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="7e07c-116">SharePoint dan aliran</span><span class="sxs-lookup"><span data-stu-id="7e07c-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


