---
title: DLP mungkin perlu jenis kustom
ms.author: stephow
author: stephow-MSFT
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
ms.openlocfilehash: 8b49afcf50e5eb53f517bbdbd002fb80dddb6f9b
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389688"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="abea2-102">DLP mungkin perlu jenis kustom</span><span class="sxs-lookup"><span data-stu-id="abea2-102">DLP might need a custom type</span></span>

<span data-ttu-id="abea2-103">Dengan kebijakan pencegahan (DLP) kehilangan data, Anda dapat mengidentifikasi dan melindungi data yang sensitif di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="abea2-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="abea2-104">Dalam beberapa skenario, Anda mungkin perlu membuat jenis informasi sensitif **kustom** Anda sendiri untuk melindungi data organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="abea2-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="abea2-105">Misalnya, organisasi Anda mungkin perlu untuk mengidentifikasi dan melindungi karyawan id atau data lain dalam beberapa format yang khusus untuk organisasi Anda Jika demikian, lihat artikel berikut untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="abea2-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="abea2-106">**Menyesuaikan informasi sensitif built-in tipe**</span><span class="sxs-lookup"><span data-stu-id="abea2-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="abea2-107">Jika jenis built-in informasi sensitif yang akan memenuhi kebutuhan Anda dengan hanya beberapa tweak, Anda dapat [menyesuaikan informasi sensitif built-in tipe](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="abea2-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="abea2-108">Misalnya, Anda dapat menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti yang mendukung seperti tanggal atau alamat.</span><span class="sxs-lookup"><span data-stu-id="abea2-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="abea2-109">**Membuat jenis informasi sensitif kustom**</span><span class="sxs-lookup"><span data-stu-id="abea2-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="abea2-110">Tetapi jika Anda perlu untuk mengidentifikasi dan melindungi jenis informasi sensitif yang berbeda sama sekali, Anda dapat [membuat jenis kustom informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) di UI dari & keamanan Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="abea2-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="abea2-111">**Membuat jenis informasi sensitif kustom dalam keamanan & kepatuhan pusat PowerShell**</span><span class="sxs-lookup"><span data-stu-id="abea2-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="abea2-112">Akhirnya, jika UI tidak menyediakan semua opsi yang Anda butuhkan, Anda dapat [membuat jenis informasi sensitif kustom dalam keamanan & kepatuhan pusat PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="abea2-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="abea2-113">Dengan memulai dengan sebuah file XML, Anda dapat menggunakan semua pilihan yang tersedia.</span><span class="sxs-lookup"><span data-stu-id="abea2-113">By starting with an XML file, you can use every option available.</span></span>
