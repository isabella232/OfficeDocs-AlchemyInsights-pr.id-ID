---
title: Melebihi batas email harian. Alur kerja ditangguhkan.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731566"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="13cfb-103">Melebihi batas email harian.</span><span class="sxs-lookup"><span data-stu-id="13cfb-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="13cfb-104">Alur kerja ditangguhkan.</span><span class="sxs-lookup"><span data-stu-id="13cfb-104">Workflow is suspended.</span></span>

<span data-ttu-id="13cfb-105">Kesalahan ini mungkin diterima dalam skenario berikut ini:</span><span class="sxs-lookup"><span data-stu-id="13cfb-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="13cfb-106">Anda memiliki alur kerja di SharePoint online yang menggunakan tipe platform alur kerja SharePoint 2010 atau SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="13cfb-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="13cfb-107">Alur kerja dikonfigurasikan untuk mengirim pesan email kustom kepada lebih dari 200 pengguna dalam satu waktu, lebih dari 10.000 Penerima per hari, atau lebih dari 30 pesan per menit.</span><span class="sxs-lookup"><span data-stu-id="13cfb-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="13cfb-108">Saat Anda menjalankan alur kerja, pesan email tidak terkirim, dan Anda melihat perilaku berikut ini:</span><span class="sxs-lookup"><span data-stu-id="13cfb-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="13cfb-109">Untuk alur kerja menggunakan tipe platform SharePoint 2013, telusuri ke halaman **status alur kerja** .</span><span class="sxs-lookup"><span data-stu-id="13cfb-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="13cfb-110">Pada halaman status alur kerja, **status internal** diatur ke **mulai**, dan balon informasi **tidak dapat dikirim ke penerima**.</span><span class="sxs-lookup"><span data-stu-id="13cfb-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="13cfb-111">Untuk mengatasi masalah ini, konfigurasikan alur kerja Anda untuk mengirim pesan email tanpa melebihi [batas pengirim Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="13cfb-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="13cfb-112">Misalnya, gunakan jeda dalam alur kerja, kirim email ke grup Microsoft 365, grup distribusi atau grup keamanan email aktif, atau kirim pesan ke penerima kurang dari 200 dalam satu waktu.</span><span class="sxs-lookup"><span data-stu-id="13cfb-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="13cfb-113">Untuk informasi selengkapnya, lihat [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)berikut ini.</span><span class="sxs-lookup"><span data-stu-id="13cfb-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="13cfb-114">Topik terkait</span><span class="sxs-lookup"><span data-stu-id="13cfb-114">Related topics</span></span>
- [<span data-ttu-id="13cfb-115">Buat alur</span><span class="sxs-lookup"><span data-stu-id="13cfb-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="13cfb-116">SharePoint dan Flow</span><span class="sxs-lookup"><span data-stu-id="13cfb-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 