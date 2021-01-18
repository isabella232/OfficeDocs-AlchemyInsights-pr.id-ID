---
title: Konfigurasi proksi aplikasi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885135"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="a0b10-102">Konfigurasi proksi aplikasi</span><span class="sxs-lookup"><span data-stu-id="a0b10-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="a0b10-103">Untuk memahami cara mengonfigurasi aplikasi proksi aplikasi dalam Azure AD untuk mengekspos aplikasi lokal Anda ke awan, lihat [cara mengonfigurasi aplikasi proksi aplikasi](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="a0b10-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="a0b10-104">Masuk tunggal (SSO) memungkinkan pengguna mengakses aplikasi tanpa mengautentikasi beberapa kali.</span><span class="sxs-lookup"><span data-stu-id="a0b10-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="a0b10-105">Ini memungkinkan autentikasi tunggal terjadi di awan, berlawanan dengan Azure Active Directory, dan memungkinkan layanan atau konektor untuk meniru pengguna untuk menyelesaikan setiap tantangan autentikasi tambahan dari aplikasi.</span><span class="sxs-lookup"><span data-stu-id="a0b10-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="a0b10-106">Untuk mempelajari selengkapnya, lihat [cara mengonfigurasi masuk tunggal ke aplikasi proksi aplikasi](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="a0b10-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="a0b10-107">Gunakan [artikel ini](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) untuk memecahkan masalah umum yang dihadapi orang saat membuat aplikasi proksi aplikasi baru.</span><span class="sxs-lookup"><span data-stu-id="a0b10-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="a0b10-108">Jika Anda mengalami masalah saat menyiapkan autentikasi back-end ke aplikasi Anda, Anda mungkin perlu [memecahkan masalah konfigurasi delegasi Kerberos untuk proksi aplikasi](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) atau mengikuti panduan tentang [mengonfigurasi aplikasi dengan pingaccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) untuk mengatasi masalah Anda.</span><span class="sxs-lookup"><span data-stu-id="a0b10-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
