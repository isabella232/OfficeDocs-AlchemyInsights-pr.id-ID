---
title: Alur kerja email tidak sedang dikirim
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748992"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="ce5a9-102">Alur kerja email tidak sedang dikirim untuk daftar atau pustaka SharePoint</span><span class="sxs-lookup"><span data-stu-id="ce5a9-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="ce5a9-103">Email dari alur kerja tidak dikirim ke semua pengguna atau pengguna tertentu saja, atau Anda melihat kesalahan **pesan email tidak dapat dikirim. pastikan email memiliki penerima yang valid**.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="ce5a9-104">Periksa apakah pengguna ada di grup izin **semua orang** (daftar informasi pengguna) untuk kumpulan situs tersebut.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="ce5a9-105">URL langsung sampel: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="ce5a9-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="ce5a9-106">Jika pengguna tidak ada, pastikan pengguna masuk ke halaman.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="ce5a9-107">Jika merupakan pengguna eksternal, pastikan bahwa undangan mereka telah diterima.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="ce5a9-108">Jika pengguna tidak ada di grup izin, pastikan alamat email sudah benar.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="ce5a9-109">Jika alamat email pengguna tidak diatur di sini, maka buat pemberitahuan sampel untuk pengguna tersebut yang memaksa sinkronisasi akun pengguna tersebut dari profil pengguna SharePoint ke kumpulan situs ini.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="ce5a9-110">Email dari alur kerja dikirim ke administrator kumpulan situs tetapi tidak untuk pengguna lain dan melihat kesalahan yang **dilarang <span>https:</span>//\Url/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="ce5a9-111">Lihat [Akses ditolak saat Anda mengirim email ke grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="ce5a9-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="ce5a9-112">Selain itu, verifikasi bahwa fitur kumpulan situs **mode penguncian izin akses terbatas pengguna** tidak aktif.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="ce5a9-113">Topik terkait</span><span class="sxs-lookup"><span data-stu-id="ce5a9-113">Related topics</span></span>
<span data-ttu-id="ce5a9-114">Ingin mencoba Microsoft Flow di SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="ce5a9-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="ce5a9-115">Buat alur</span><span class="sxs-lookup"><span data-stu-id="ce5a9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ce5a9-116">SharePoint dan Flow</span><span class="sxs-lookup"><span data-stu-id="ce5a9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


