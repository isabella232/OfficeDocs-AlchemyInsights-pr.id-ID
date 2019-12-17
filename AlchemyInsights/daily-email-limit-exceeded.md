---
title: Melebihi batas email harian. Alur kerja ditangguhkan.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053120"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="6c172-103">Melebihi batas email harian.</span><span class="sxs-lookup"><span data-stu-id="6c172-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="6c172-104">Alur kerja ditangguhkan.</span><span class="sxs-lookup"><span data-stu-id="6c172-104">Workflow is suspended.</span></span>

<span data-ttu-id="6c172-105">Galat ini mungkin diterima dalam skenario berikut:</span><span class="sxs-lookup"><span data-stu-id="6c172-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="6c172-106">Anda memiliki alur kerja di SharePoint online yang menggunakan jenis platform alur kerja SharePoint 2010 atau SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="6c172-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="6c172-107">Alur kerja dikonfigurasi untuk mengirim pesan email kustom untuk lebih dari 200 pengguna pada waktu, lebih dari 10.000 Penerima per hari, atau lebih dari 30 pesan per menit.</span><span class="sxs-lookup"><span data-stu-id="6c172-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="6c172-108">Ketika Anda menjalankan alur kerja, pesan email tidak dikirim, dan Anda melihat perilaku berikut ini:</span><span class="sxs-lookup"><span data-stu-id="6c172-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="6c172-109">Untuk alur kerja menggunakan jenis platform SharePoint 2013, menjelajah ke halaman **status alur kerja** .</span><span class="sxs-lookup"><span data-stu-id="6c172-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="6c172-110">Pada halaman status alur kerja, **status internal** diatur untuk **memulai**, dan informasi balon menampilkan **tidak dapat mengirim ke penerima**.</span><span class="sxs-lookup"><span data-stu-id="6c172-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="6c172-111">Untuk mengatasi masalah ini, konfigurasikan alur kerja Anda untuk mengirim pesan email tanpa melebihi [batas pengirim Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="6c172-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="6c172-112">Misalnya, gunakan jeda di alur kerja, mengirim email ke grup 365 Office, grup distribusi atau grup keamanan Surat diaktifkan, atau mengirim pesan ke kurang dari 200 Penerima pada waktu.</span><span class="sxs-lookup"><span data-stu-id="6c172-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="6c172-113">Untuk informasi selengkapnya, lihat [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)berikut ini.</span><span class="sxs-lookup"><span data-stu-id="6c172-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="6c172-114">Topik terkait</span><span class="sxs-lookup"><span data-stu-id="6c172-114">Related topics</span></span>
- [<span data-ttu-id="6c172-115">Membuat Flow</span><span class="sxs-lookup"><span data-stu-id="6c172-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6c172-116">SharePoint dan aliran</span><span class="sxs-lookup"><span data-stu-id="6c172-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 