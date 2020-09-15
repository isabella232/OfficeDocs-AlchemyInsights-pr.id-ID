---
title: DLP mungkin memerlukan tipe kustom
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712187"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="9f1f8-102">DLP mungkin memerlukan tipe kustom</span><span class="sxs-lookup"><span data-stu-id="9f1f8-102">DLP might need a custom type</span></span>

<span data-ttu-id="9f1f8-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="9f1f8-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9f1f8-104">**DLP mungkin memerlukan tipe informasi kustom**</span><span class="sxs-lookup"><span data-stu-id="9f1f8-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="9f1f8-105">Dengan kebijakan pencegahan kehilangan data (DLP), Anda bisa mengidentifikasi dan melindungi data sensitif di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="9f1f8-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="9f1f8-106">Dalam beberapa skenario, Anda mungkin perlu membuat tipe informasi sensitif **kustom** Anda sendiri untuk melindungi data organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="9f1f8-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="9f1f8-107">Misalnya, organisasi Anda mungkin perlu mengidentifikasi dan melindungi id karyawan atau data lain dalam beberapa format tertentu untuk organisasi Anda. Jika demikian, lihat artikel berikut ini untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="9f1f8-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="9f1f8-108">**Mengkustomisasi tipe informasi sensitif bawaan**</span><span class="sxs-lookup"><span data-stu-id="9f1f8-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="9f1f8-109">Jika tipe informasi sensitif bawaan akan memenuhi kebutuhan Anda hanya dengan beberapa tweak, Anda dapat [mengustomisasi tipe informasi sensitif bawaan](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="9f1f8-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="9f1f8-110">Misalnya, Anda bisa menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti yang mendukung seperti tanggal atau alamat.</span><span class="sxs-lookup"><span data-stu-id="9f1f8-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="9f1f8-111">**Membuat tipe informasi sensitif kustom**</span><span class="sxs-lookup"><span data-stu-id="9f1f8-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="9f1f8-112">Tapi jika Anda perlu mengidentifikasi dan melindungi tipe informasi sensitif yang berbeda secara bersamaan, Anda bisa [membuat tipe informasi sensitif kustom](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) di UI pusat kepatuhan & keamanan.</span><span class="sxs-lookup"><span data-stu-id="9f1f8-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="9f1f8-113">**Membuat tipe informasi sensitif kustom di keamanan & pusat kepatuhan PowerShell**</span><span class="sxs-lookup"><span data-stu-id="9f1f8-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="9f1f8-114">Akhirnya, jika UI tidak menyediakan semua opsi yang Anda perlukan, Anda bisa [membuat tipe informasi sensitif kustom di pusat kepatuhan & keamanan PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9f1f8-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="9f1f8-115">Dengan memulai dengan file XML, Anda bisa menggunakan setiap opsi yang tersedia.</span><span class="sxs-lookup"><span data-stu-id="9f1f8-115">By starting with an XML file, you can use every option available.</span></span>
