---
title: 1065 bantasi alamat IP keluar EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704600"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="11772-102">Bantasi rentang alamat IP keluar EOP</span><span class="sxs-lookup"><span data-stu-id="11772-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="11772-103">Kami telah mendeteksi potensi masalah dengan organisasi Anda yang (jika tidak dikoreksi pada tanggal 26 Oktober, 2018) dapat merusak alur e-mail ke tujuan lokal atau eksternal.</span><span class="sxs-lookup"><span data-stu-id="11772-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="11772-104">Seperti yang telah dikomunikasikan sebelumnya, untuk menyederhanakan manajemen kisaran alamat IP, kami mengkonsolidasikan rentang alamat IP Exchange Online Protection (EOP) yang digunakan untuk mengirim dan menerima email di luar Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="11772-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="11772-105">Analisis kami menunjukkan bahwa satu atau lebih dari sumber email eksternal atau tujuan yang telah dikonfigurasi di konektor aliran surat tidak menerima sambungan dari kisaran alamat IP yang ditunjukkan [di sini](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="11772-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="11772-106">Bertindaklah sebelum Oktober 26 untuk memastikan sumber dan tujuan ini akan menerima koneksi ke dan dari semua [Alamat EOP IP yang diterbitkan](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="11772-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="11772-107">Untuk informasi lebih lanjut tentang perubahan ini, silakan lihat pesan pusat posting [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), atau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="11772-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="11772-108">**Catatan**: jika sebelumnya Anda menggunakan IP atau URL penerbitan melalui HTML, XML, dan RSS untuk pembaruan titik akhir, Anda juga harus bermigrasi ke layanan web baru untuk mengotomatisasi jenis pembaruan ini.</span><span class="sxs-lookup"><span data-stu-id="11772-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="11772-109">Untuk informasi selengkapnya, lihat [microsoft 365 Endpoint kategori dan microsoft 365 alamat IP dan URL layanan web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="11772-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
