---
title: Alamat 1065 bantahan EOP outbound IP rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294857"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="88e56-102">Bantahan dari EOP kisaran alamat IP keluar</span><span class="sxs-lookup"><span data-stu-id="88e56-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="88e56-p101">Kami telah mendeteksi potensi masalah dengan organisasi yang (jika tidak diperbaiki oleh 26 Oktober 2018) mungkin istirahat alur e-mail ke lokal atau tujuan eksternal. Sebagaimana diwartakan sebelumnya, untuk menyederhanakan manajemen kisaran alamat IP, kita sedang mengkonsolidasikan rentang alamat IP perlindungan Online pertukaran (EOP) yang digunakan untuk mengirim dan menerima email di luar Office 365. Analisis kami menunjukkan bahwa satu atau lebih email eksternal sumber atau tujuan yang dikonfigurasi di mail aliran konektor tidak menerima koneksi dari IP alamat rentang ditunjukkan [di sini](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="88e56-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="88e56-106">Bertindak sebelum Oktober 26 untuk memastikan sumber dan tujuan ini akan menerima koneksi ke dan dari semua [diterbitkan alamat EOP IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="88e56-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="88e56-107">Untuk informasi lebih lanjut mengenai perubahan ini, lihat pusat pesan posting [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), atau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="88e56-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="88e56-p102">**Catatan**: jika Anda sebelumnya menggunakan IP atau URL penerbitan melalui HTML, XML, dan RSS pembaruan endpoint, Anda juga harus memigrasi ke layanan web baru untuk mengotomatisasi jenis update. Untuk informasi lebih lanjut, lihat [kategori endpoint Office 365 dan kantor 365 alamat IP dan URL web layanan](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="88e56-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  
