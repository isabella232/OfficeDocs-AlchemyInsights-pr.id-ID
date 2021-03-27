---
title: Konsep autentikasi tingkat lanjut berlaku untuk Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398587"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="50e64-102">Konsep autentikasi tingkat lanjut berlaku untuk Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="50e64-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="50e64-103">Berikut adalah konsep autentikasi tingkat lanjut yang berlaku untuk Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="50e64-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="50e64-104">**Autentikasi Proaktif**</span><span class="sxs-lookup"><span data-stu-id="50e64-104">**Proactive Authentication**</span></span>

<span data-ttu-id="50e64-105">Saat Anda mengaktifkan kebijakan [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge akan mencoba mengautentikasi pengguna yang masuk secara proaktif melalui layanan Microsoft.</span><span class="sxs-lookup"><span data-stu-id="50e64-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="50e64-106">Pada interval reguler, layanan online akan menggunakan layanan untuk memeriksa manifes diperbarui yang berisi konfigurasi yang mengatur Autentikasi Proaktif.</span><span class="sxs-lookup"><span data-stu-id="50e64-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="50e64-107">Manfaat: Autentikasi Proaktif memungkinkan autentikasi untuk layanan kunci, seperti Halaman Tab Baru Office.</span><span class="sxs-lookup"><span data-stu-id="50e64-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="50e64-108">Selain itu, jika Bing digunakan sebagai mesin pencarian, Autentikasi Proaktif meningkatkan kinerja bilah alamat dan membantu menghasilkan hasil pencarian yang dipersonalisasi sesuai kebutuhan bisnis Anda.</span><span class="sxs-lookup"><span data-stu-id="50e64-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="50e64-109">**CredUI Windows Hello untuk Autentikasi NTLM**</span><span class="sxs-lookup"><span data-stu-id="50e64-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="50e64-110">Jika masuk tunggal (SSO) tidak tersedia saat situs web mencoba untuk masuk kepada pengguna melalui mekanisme NTLM atau Negotiate, fitur ini akan memungkinkan pengguna untuk berbagi kredensial OS dengan situs web dan untuk memenuhi tantangan autentikasi dengan menggunakan Windows Hello Cred UI.</span><span class="sxs-lookup"><span data-stu-id="50e64-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="50e64-111">Aliran masuk ini hanya akan muncul di Windows 10 dan hanya untuk pengguna yang tidak mendapatkan SSO selama NTLM atau tantangan Negosiasi.</span><span class="sxs-lookup"><span data-stu-id="50e64-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="50e64-112">**Menggunakan kata sandi yang disimpan untuk masuk secara otomatis**</span><span class="sxs-lookup"><span data-stu-id="50e64-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="50e64-113">Pengguna yang menyimpan kata sandi di Microsoft Edge dapat mengaktifkan akses masuk otomatis ke situs web tempat mereka menyimpan kredensial.</span><span class="sxs-lookup"><span data-stu-id="50e64-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="50e64-114">Pengguna dapat mengaktifkan atau menonaktifkan fitur edge://settings/passwords, dan Anda dapat mengonfigurasinya dalam kebijakan [pengelola kata](https://go.microsoft.com/fwlink/?linkid=2134622) sandi.</span><span class="sxs-lookup"><span data-stu-id="50e64-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
