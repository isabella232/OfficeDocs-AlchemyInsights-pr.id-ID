---
title: Mulai menggunakan SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700710"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="a2d96-102">Alur kerja di SharePoint</span><span class="sxs-lookup"><span data-stu-id="a2d96-102">Workflows in SharePoint</span></span>

<span data-ttu-id="a2d96-103">Jika alur kerja SharePoint tidak mengirim email, organisasi Anda mungkin mengalami batas pengirim Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a2d96-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="a2d96-104">Pesan kesalahan ' alur kerja ditangguhkan ' dapat terjadi jika Anda memiliki salah satu item berikut:</span><span class="sxs-lookup"><span data-stu-id="a2d96-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="a2d96-105">Anda memiliki alur kerja di SharePoint online yang menggunakan tipe platform alur kerja SharePoint 2010 atau SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="a2d96-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="a2d96-106">Alur kerja dikonfigurasikan untuk mengirim pesan email kustom kepada lebih dari 200 pengguna dalam satu waktu, lebih dari 10.000 Penerima per hari, atau lebih dari 30 pesan per menit.</span><span class="sxs-lookup"><span data-stu-id="a2d96-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="a2d96-107">Saat Anda menjalankan alur kerja, pesan email tidak terkirim, dan Anda melihat pesan kesalahan, status internal diatur ke ditangguhkan atau tidak dapat mengirim ke Penerima ditampilkan.</span><span class="sxs-lookup"><span data-stu-id="a2d96-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="a2d96-108">Untuk informasi selengkapnya, lihat [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)berikut ini.</span><span class="sxs-lookup"><span data-stu-id="a2d96-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

