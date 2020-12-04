---
title: Konsep autentikasi tingkat lanjut yang berlaku untuk Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573522"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="19d12-102">Konsep autentikasi tingkat lanjut yang berlaku untuk Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="19d12-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="19d12-103">Berikut ini adalah konsep autentikasi tingkat lanjut yang berlaku untuk Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="19d12-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="19d12-104">**Autentikasi proaktif**</span><span class="sxs-lookup"><span data-stu-id="19d12-104">**Proactive Authentication**</span></span>

<span data-ttu-id="19d12-105">Saat Anda mengaktifkan kebijakan [Proactiveauthenabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge akan mencoba mengautentikasi pengguna yang masuk secara proaktif melalui layanan Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19d12-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="19d12-106">Secara berkala, akan menggunakan layanan online untuk memeriksa manifest yang berisi konfigurasi yang mengatur autentikasi proaktif.</span><span class="sxs-lookup"><span data-stu-id="19d12-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="19d12-107">Manfaat: autentikasi proaktif memungkinkan autentikasi ke layanan utama, seperti halaman tab baru Office.</span><span class="sxs-lookup"><span data-stu-id="19d12-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="19d12-108">Selain itu, jika Bing digunakan sebagai mesin pencari, autentikasi proaktif meningkatkan kinerja bilah alamat dan membantu menghasilkan hasil pencarian yang dipersonalisasi dengan kebutuhan bisnis Anda.</span><span class="sxs-lookup"><span data-stu-id="19d12-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="19d12-109">**Windows Hello CredUI untuk autentikasi NTLM**</span><span class="sxs-lookup"><span data-stu-id="19d12-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="19d12-110">Jika masuk tunggal (SSO) tidak tersedia ketika sebuah situs web mencoba untuk masuk ke pengguna melalui mekanisme NTLM atau Negotiate, fitur ini akan memungkinkan pengguna untuk berbagi kredensial OS dengan situs web dan untuk memenuhi tantangan autentikasi dengan menggunakan Windows Halo Cred UI.</span><span class="sxs-lookup"><span data-stu-id="19d12-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="19d12-111">Alur masuk ini hanya akan muncul di Windows 10 dan hanya untuk pengguna yang tidak mendapatkan SSO selama tantangan NTLM atau negosiasi.</span><span class="sxs-lookup"><span data-stu-id="19d12-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="19d12-112">**Gunakan kata sandi yang disimpan untuk masuk secara otomatis**</span><span class="sxs-lookup"><span data-stu-id="19d12-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="19d12-113">Pengguna yang menyimpan kata sandi di Microsoft Edge dapat mengaktifkan masuk otomatis ke situs web tempat kredensial disimpan.</span><span class="sxs-lookup"><span data-stu-id="19d12-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="19d12-114">Pengguna bisa mengaktifkan atau menonaktifkan fitur ini di edge://settings/passwords, dan Anda bisa mengonfigurasinya di kebijakan [manajer kata sandi](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="19d12-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
