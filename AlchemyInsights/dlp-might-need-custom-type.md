---
title: DLP mungkin memerlukan jenis khusus
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052904"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="26fcd-102">DLP mungkin memerlukan jenis khusus</span><span class="sxs-lookup"><span data-stu-id="26fcd-102">DLP might need a custom type</span></span>

<span data-ttu-id="26fcd-103">Dengan kebijakan pencegahan kehilangan data (DLP), Anda dapat mengidentifikasi dan melindungi data sensitif di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="26fcd-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="26fcd-104">Dalam beberapa skenario, Anda mungkin perlu membuat jenis informasi sensitif **kustom** sendiri untuk melindungi data organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="26fcd-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="26fcd-105">Misalnya, organisasi Anda mungkin perlu mengidentifikasi dan melindungi id karyawan atau data lain dalam beberapa format khusus untuk organisasi Anda. Jika demikian, lihat artikel berikut untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="26fcd-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="26fcd-106">**Menyesuaikan jenis informasi sensitif internal**</span><span class="sxs-lookup"><span data-stu-id="26fcd-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="26fcd-107">Jika jenis informasi sensitif internal akan memenuhi kebutuhan Anda hanya dengan beberapa tweak, Anda dapat [menyesuaikan jenis informasi sensitif internal](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="26fcd-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="26fcd-108">Misalnya, Anda dapat menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti pendukung seperti tanggal atau alamat.</span><span class="sxs-lookup"><span data-stu-id="26fcd-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="26fcd-109">**Membuat jenis informasi sensitif kustom**</span><span class="sxs-lookup"><span data-stu-id="26fcd-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="26fcd-110">Namun, jika Anda perlu mengidentifikasi dan melindungi berbagai jenis informasi sensitif sama sekali, Anda dapat [membuat jenis informasi sensitif kustom](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) di UI pusat kepatuhan & keamanan.</span><span class="sxs-lookup"><span data-stu-id="26fcd-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="26fcd-111">**Membuat jenis informasi sensitif kustom di keamanan & kepatuhan pusat PowerShell**</span><span class="sxs-lookup"><span data-stu-id="26fcd-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="26fcd-112">Akhirnya, jika UI tidak menyediakan semua pilihan yang Anda butuhkan, Anda dapat [membuat jenis informasi sensitif kustom di keamanan & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="26fcd-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="26fcd-113">Dengan memulai dengan sebuah file XML, Anda dapat menggunakan setiap pilihan yang tersedia.</span><span class="sxs-lookup"><span data-stu-id="26fcd-113">By starting with an XML file, you can use every option available.</span></span>
