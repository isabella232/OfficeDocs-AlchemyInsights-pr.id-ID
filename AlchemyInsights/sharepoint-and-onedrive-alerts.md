---
title: Penundaan dalam menerima pemberitahuan SharePoint dan OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727246"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="40c13-102">Penundaan dalam menerima pemberitahuan SharePoint dan OneDrive</span><span class="sxs-lookup"><span data-stu-id="40c13-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="40c13-103">Pertama, periksa folder sampah atau spam di email Anda.</span><span class="sxs-lookup"><span data-stu-id="40c13-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="40c13-104">Jika **semua pemberitahuan dari beberapa file atau pustaka tertunda**, kunjungi [dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home?ref=/servicehealth) untuk memeriksa setiap saran/kejadian yang mungkin terjadi dengan SharePoint atau Exchange.</span><span class="sxs-lookup"><span data-stu-id="40c13-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="40c13-105">Masalah mungkin dengan kapabilitas pemberitahuan SharePoint atau keterlambatan dalam email melalui Exchange.</span><span class="sxs-lookup"><span data-stu-id="40c13-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="40c13-106">Perhatikan juga Apakah email lain sedang dikirim — jika tidak, masalah ini mungkin terjadi karena penundaan Exchange.</span><span class="sxs-lookup"><span data-stu-id="40c13-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="40c13-107">Jika **pemberitahuan individu dari file atau pustaka tertentu tidak terkirim**, cobalah untuk menghapus dan membuatnya kembali.</span><span class="sxs-lookup"><span data-stu-id="40c13-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="40c13-108">Lihat [mengelola, menampilkan, atau menghapus pemberitahuan SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) untuk membuat ulang pemberitahuan.</span><span class="sxs-lookup"><span data-stu-id="40c13-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="40c13-109">Pemberitahuan tidak bisa dikirim ke grup distribusi.</span><span class="sxs-lookup"><span data-stu-id="40c13-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="40c13-110">Hanya grup keamanan dan O365 yang didukung.</span><span class="sxs-lookup"><span data-stu-id="40c13-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="40c13-111">Anda tidak dapat mengustomisasi Templat email pemberitahuan.</span><span class="sxs-lookup"><span data-stu-id="40c13-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="40c13-112">Anda harus menggunakan alur kerja Microsoft Flow atau SharePoint Designer untuk mencapainya.</span><span class="sxs-lookup"><span data-stu-id="40c13-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
