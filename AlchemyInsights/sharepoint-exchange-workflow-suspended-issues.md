---
title: Memulai dengan SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051644"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="d9b47-102">Alur kerja di SharePoint</span><span class="sxs-lookup"><span data-stu-id="d9b47-102">Workflows in SharePoint</span></span>

<span data-ttu-id="d9b47-103">Jika alur kerja SharePoint tidak mengirim email, organisasi Anda mungkin mengalami batas pengirim Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="d9b47-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="d9b47-104">Pesan galat ' alur kerja ditangguhkan ' dapat terjadi jika Anda memiliki salah satu item berikut ini:</span><span class="sxs-lookup"><span data-stu-id="d9b47-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="d9b47-105">Anda memiliki alur kerja di SharePoint online yang menggunakan jenis platform alur kerja SharePoint 2010 atau SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="d9b47-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="d9b47-106">Alur kerja dikonfigurasi untuk mengirim pesan email kustom untuk lebih dari 200 pengguna pada waktu, lebih dari 10.000 Penerima per hari, atau lebih dari 30 pesan per menit.</span><span class="sxs-lookup"><span data-stu-id="d9b47-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="d9b47-107">Ketika Anda menjalankan alur kerja, pesan email tidak dikirim, dan Anda melihat pesan galat, status internal diatur ke ditangguhkan atau tidak dapat mengirim ke penerima akan ditampilkan.</span><span class="sxs-lookup"><span data-stu-id="d9b47-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="d9b47-108">Untuk informasi lebih lanjut, silakan lihat [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)berikut.</span><span class="sxs-lookup"><span data-stu-id="d9b47-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

