---
title: Masalah pada tautan dan URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707885"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="dd887-102">Masalah pada tautan dan URL</span><span class="sxs-lookup"><span data-stu-id="dd887-102">Issues with links and URLs</span></span>

<span data-ttu-id="dd887-103">URI pengalihan/URL balasan (kedua ekspresi dapat dipertukarkan) adalah URL yang digunakan oleh platform identitas Microsoft untuk menampilkan token yang diminta aplikasi.</span><span class="sxs-lookup"><span data-stu-id="dd887-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="dd887-104">Untuk informasi tentang URL tersebut, lihat artikel berikut:</span><span class="sxs-lookup"><span data-stu-id="dd887-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="dd887-105">[Aliran autentikasi dan skenario aplikasi](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Informasi mengenai URI pengalihan di halaman **Pendaftaran aplikasi** untuk setiap skenario.</span><span class="sxs-lookup"><span data-stu-id="dd887-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="dd887-106">Pembatasan dan batasan URI pengalihan/URL balasan</span><span class="sxs-lookup"><span data-stu-id="dd887-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="dd887-107">**Saya tidak tahu cara mendaftarkan URI pengalihan/URL balasan yang benar untuk aplikasi saya**</span><span class="sxs-lookup"><span data-stu-id="dd887-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="dd887-108">Saat masuk dengan aplikasi yang Anda kembangkan, jika dialog masuk menampilkan **AADSTS50011: URL balasan yang ditentukan dalam permintaan tidak cocok dengan URL balasan yang dikonfigurasi untuk aplikasi <your app ID>**, Anda perlu menambahkan URI pengalihan yang digunakan kode Anda dalam permintaan token ke platform identitas Microsoft ke pendaftaran aplikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="dd887-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="dd887-109">Untuk menambahkan URL balasan, buka tab **Autentikasi** di halaman **pendaftaran aplikasi** Anda di portal Microsoft Azure, lalu tambahkan entri di bagian **URI Pengalihan**.</span><span class="sxs-lookup"><span data-stu-id="dd887-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="dd887-110">Nilai yang perlu Anda masukkan bergantung pada tipe aplikasi yang Anda buat, seperti yang dijelaskan di bawah ini:</span><span class="sxs-lookup"><span data-stu-id="dd887-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="dd887-111">Untuk aplikasi satu halaman dan aplikasi web, URL balasannya adalah URL di aplikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="dd887-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="dd887-112">Lihat [Pendaftaran aplikasi satu halaman](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) atau [Mendaftarkan aplikasi web menggunakan portal Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="dd887-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="dd887-113">Untuk aplikasi desktop, nilai yang perlu Anda pilih bergantung pada:</span><span class="sxs-lookup"><span data-stu-id="dd887-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="dd887-114">platform (MacOS berbeda dengan Windows atau Linux)</span><span class="sxs-lookup"><span data-stu-id="dd887-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="dd887-115">cara Anda memperoleh token (secara interaktif, dengan alur kode perangkat, dengan Autentikasi Windows Terpadu [IWA] atau dengan nama pengguna/kata sandi).</span><span class="sxs-lookup"><span data-stu-id="dd887-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="dd887-116">Untuk detailnya, lihat [Aplikasi desktop - Pendaftaran aplikasi - URI Pengalihan](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="dd887-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="dd887-117">Untuk aplikasi seluler, URI pengalihan bergantung pada:</span><span class="sxs-lookup"><span data-stu-id="dd887-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="dd887-118">platform (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="dd887-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="dd887-119">informasi yang digunakan untuk membangun aplikasi Anda, seperti ID bundel di iOS, dan nama paket serta hash tanda tangan di Android Pendaftaran aplikasi portal Microsoft Azure akan membantu Anda.</span><span class="sxs-lookup"><span data-stu-id="dd887-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="dd887-120">Untuk detailnya, lihat [Konfigurasi platform dan URI pengalihan](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="dd887-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="dd887-121">Web API dan beberapa cara untuk memperoleh token (IWA dan nama pengguna/kata sandi) secara diam-diam tidak memerlukan URI pengalihan.</span><span class="sxs-lookup"><span data-stu-id="dd887-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="dd887-122">**Saya telah menyebarkan aplikasi web saya dan ketika saya mengujinya, saya mendapatkan pesan ketidakcocokan url balasan**</span><span class="sxs-lookup"><span data-stu-id="dd887-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="dd887-123">Tambahkan URI pengalihan untuk semua lokasi tempat Anda menyebarkan aplikasi web.</span><span class="sxs-lookup"><span data-stu-id="dd887-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="dd887-124">Untuk informasi selengkapnya, lihat [Mendaftarkan aplikasi web menggunakan portal Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="dd887-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="dd887-125">Tambahkan URI pengalihan untuk lokasi segera setelah Anda menyebarkan aplikasi di lokasi itu.</span><span class="sxs-lookup"><span data-stu-id="dd887-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="dd887-126">**Saya tidak bisa mendaftarkan cukup URL balasan**</span><span class="sxs-lookup"><span data-stu-id="dd887-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="dd887-127">Anda merupakan ISV dan memiliki satu atau beberapa URI pengalihan untuk setiap pelanggan Anda.</span><span class="sxs-lookup"><span data-stu-id="dd887-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="dd887-128">Anda ingin melakukan migrasi dari ADAL/Azure AD v1.0 ke MSAL/platform identitas Microsoft dan Anda menekan [jumlah maksimal URI pengalihan](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="dd887-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="dd887-129">Untuk mengatasi ini, [tambahkan URI pengalihan ke layanan utama](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) yang sesuai dengan setiap pelanggan Anda.</span><span class="sxs-lookup"><span data-stu-id="dd887-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
