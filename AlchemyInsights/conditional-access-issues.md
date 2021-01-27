---
title: Masalah akses bersyarat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014884"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="8b600-102">Masalah akses bersyarat</span><span class="sxs-lookup"><span data-stu-id="8b600-102">Conditional access issues</span></span>

<span data-ttu-id="8b600-103">**Mengatasi masalah dengan diagnostik masuk**</span><span class="sxs-lookup"><span data-stu-id="8b600-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="8b600-104">Anda dapat dengan cepat menemukan apa yang terjadi atau mendiagnosis masalah terkait masuk pengguna dengan menggunakan [diagnostik masuk](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="8b600-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="8b600-105">Luncurkan diagnostik masuk.</span><span class="sxs-lookup"><span data-stu-id="8b600-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="8b600-106">Temukan acara untuk dianalisis dengan memasukkan detail yang Anda miliki tentang pengguna, aplikasi, waktu masuk, id permintaan, atau id korelasi.</span><span class="sxs-lookup"><span data-stu-id="8b600-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="8b600-107">Tinjau hasil diagnostik yang memperlihatkan detail tentang apa yang terjadi dan tindakan apa yang bisa Anda lakukan untuk membuat perubahan (jika ada perubahan yang diperlukan).</span><span class="sxs-lookup"><span data-stu-id="8b600-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="8b600-108">**Langkah-langkah untuk memecahkan masalah masuk**</span><span class="sxs-lookup"><span data-stu-id="8b600-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="8b600-109">Navigasikan ke halaman masuk Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8b600-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="8b600-110">Memfilter masuk menurut pengguna, rentang waktu, aplikasi, status, aplikasi klien, dan seterusnya.</span><span class="sxs-lookup"><span data-stu-id="8b600-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="8b600-111">Pilih acara masuk dan Tampilkan Tab akses bersyarat untuk melihat kebijakan mana yang dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="8b600-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="8b600-112">Klik pada baris kebijakan untuk menampilkan detail kebijakan dan memahami alasannya.</span><span class="sxs-lookup"><span data-stu-id="8b600-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="8b600-113">**Alat untuk memecahkan masalah kebijakan akses bersyarat**</span><span class="sxs-lookup"><span data-stu-id="8b600-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="8b600-114">Mode hanya-laporan memungkinkan Anda mengevaluasi kebijakan tanpa memengaruhi pengguna.</span><span class="sxs-lookup"><span data-stu-id="8b600-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="8b600-115">Alat apa-jika memungkinkan Anda mensimulasikan acara masuk dan melihat kebijakan mana yang berlaku.</span><span class="sxs-lookup"><span data-stu-id="8b600-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="8b600-116">Insight dan buku kerja pelaporan menampilkan dampak waktu nyata dari setiap kebijakan.</span><span class="sxs-lookup"><span data-stu-id="8b600-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="8b600-117">**Kebijakan perlindungan garis dasar**</span><span class="sxs-lookup"><span data-stu-id="8b600-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="8b600-118">Kebijakan perlindungan garis dasar telah usang.</span><span class="sxs-lookup"><span data-stu-id="8b600-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="8b600-119">Mereka tidak lagi diberlakukan dan akan segera dihapus dari Azure portal.</span><span class="sxs-lookup"><span data-stu-id="8b600-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="8b600-120">Kami menyarankan untuk mengaktifkan [keamanan default](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="8b600-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="8b600-121">Untuk informasi selengkapnya tentang akses bersyarat Lihat:</span><span class="sxs-lookup"><span data-stu-id="8b600-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="8b600-122">[Praktik terbaik untuk akses bersyarat di direktori](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 aktif Azure [Kondisi dalam akses bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrol dalam akses bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Lokasi dalam akses bersyarat](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="8b600-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
