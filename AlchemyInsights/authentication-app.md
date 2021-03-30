---
title: Aplikasi autentikasi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405064"
---
# <a name="authentication-app"></a><span data-ttu-id="0d7e1-102">Aplikasi autentikasi</span><span class="sxs-lookup"><span data-stu-id="0d7e1-102">Authentication app</span></span>

<span data-ttu-id="0d7e1-103">Jika Anda adalah Admin Global, Anda bisa dengan cepat mencari tahu apa yang terjadi atau mendiagnosis masalah yang terkait dengan masuknya pengguna dengan menggunakan Diagnostik [Masuk.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="0d7e1-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="0d7e1-104">Mulai diagnostik dengan mengklik tombol "[Luncurkan Diagnostik](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)".</span><span class="sxs-lookup"><span data-stu-id="0d7e1-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="0d7e1-105">Temukan kegiatan yang akan dianalisis dengan memasukkan detail yang Anda miliki tentang pengguna, aplikasi, waktu masuk, ID permintaan, atau ID korelasi.</span><span class="sxs-lookup"><span data-stu-id="0d7e1-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="0d7e1-106">Tinjau hasil diagnostik yang memperlihatkan detail tentang apa yang terjadi dan tindakan apa yang dapat Anda lakukan untuk membuat perubahan, jika diperlukan perubahan.</span><span class="sxs-lookup"><span data-stu-id="0d7e1-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="0d7e1-107">**Periksa skenario yang berlaku:**</span><span class="sxs-lookup"><span data-stu-id="0d7e1-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="0d7e1-108">Jika pengguna tidak mendapatkan pemberitahuan push di aplikasi Microsoft Authenticator, verifikasi bahwa mereka tidak ditampilkan di bawah pengguna yang diblokir MFA seperti yang dijelaskan di Memblokir dan membuka blokir [pengguna.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="0d7e1-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="0d7e1-109">Jika pengguna tidak diblokir untuk MFA tetapi tidak menerima pemberitahuan push, mereka dapat membuka aplikasi Microsoft Authenticator yang akan menarik permintaan persetujuan yang tertunda.</span><span class="sxs-lookup"><span data-stu-id="0d7e1-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="0d7e1-110">Sebagai metode masuk alternatif, pengguna juga bisa mengklik Masuk dengan cara lain dan memilih menggunakan kode verifikasi dari aplikasi seluler saya.</span><span class="sxs-lookup"><span data-stu-id="0d7e1-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="0d7e1-111">Aplikasi Microsoft Authenticator adalah satu-satunya metode yang tersedia untuk banyak pengguna.</span><span class="sxs-lookup"><span data-stu-id="0d7e1-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="0d7e1-112">[Pelajari selengkapnya tentang default keamanan,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)periksa [FAQ Aplikasi Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) untuk pertanyaan yang sering diajukan dan cara mengatasinya.</span><span class="sxs-lookup"><span data-stu-id="0d7e1-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="0d7e1-113">**Video yang Disarankan**</span><span class="sxs-lookup"><span data-stu-id="0d7e1-113">**Recommended Videos**</span></span>

<span data-ttu-id="0d7e1-114">[Cara menyiapkan Aplikasi Authenticator di telepon baru (2 menit).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="0d7e1-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
