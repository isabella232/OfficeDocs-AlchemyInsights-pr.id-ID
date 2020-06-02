---
title: DLP mungkin memerlukan jenis khusus
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507517"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="1bd5d-102">DLP mungkin memerlukan jenis khusus</span><span class="sxs-lookup"><span data-stu-id="1bd5d-102">DLP might need a custom type</span></span>

<span data-ttu-id="1bd5d-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="1bd5d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1bd5d-104">**DLP mungkin memerlukan jenis informasi kustom**</span><span class="sxs-lookup"><span data-stu-id="1bd5d-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="1bd5d-105">Dengan kebijakan pencegahan kehilangan data (DLP), Anda dapat mengidentifikasi dan melindungi data sensitif di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="1bd5d-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="1bd5d-106">Dalam beberapa skenario, Anda mungkin perlu membuat jenis informasi sensitif **kustom** sendiri untuk melindungi data organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="1bd5d-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="1bd5d-107">Misalnya, organisasi Anda mungkin perlu mengidentifikasi dan melindungi id karyawan atau data lain dalam beberapa format khusus untuk organisasi Anda. Jika demikian, lihat artikel berikut untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="1bd5d-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="1bd5d-108">**Menyesuaikan jenis informasi sensitif internal**</span><span class="sxs-lookup"><span data-stu-id="1bd5d-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="1bd5d-109">Jika jenis informasi sensitif internal akan memenuhi kebutuhan Anda hanya dengan beberapa tweak, Anda dapat [menyesuaikan jenis informasi sensitif internal](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="1bd5d-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="1bd5d-110">Misalnya, Anda dapat menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti pendukung seperti tanggal atau alamat.</span><span class="sxs-lookup"><span data-stu-id="1bd5d-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="1bd5d-111">**Membuat jenis informasi sensitif kustom**</span><span class="sxs-lookup"><span data-stu-id="1bd5d-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="1bd5d-112">Namun, jika Anda perlu mengidentifikasi dan melindungi berbagai jenis informasi sensitif sama sekali, Anda dapat [membuat jenis informasi sensitif kustom](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) di UI pusat kepatuhan & keamanan.</span><span class="sxs-lookup"><span data-stu-id="1bd5d-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="1bd5d-113">**Membuat jenis informasi sensitif kustom di keamanan & kepatuhan pusat PowerShell**</span><span class="sxs-lookup"><span data-stu-id="1bd5d-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="1bd5d-114">Akhirnya, jika UI tidak menyediakan semua pilihan yang Anda butuhkan, Anda dapat [membuat jenis informasi sensitif kustom di keamanan & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="1bd5d-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="1bd5d-115">Dengan memulai dengan sebuah file XML, Anda dapat menggunakan setiap pilihan yang tersedia.</span><span class="sxs-lookup"><span data-stu-id="1bd5d-115">By starting with an XML file, you can use every option available.</span></span>
