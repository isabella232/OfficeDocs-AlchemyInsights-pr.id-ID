---
title: Menggunakan AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177544"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="8f708-102">Menggunakan AD FS</span><span class="sxs-lookup"><span data-stu-id="8f708-102">Deploy AD FS</span></span>

<span data-ttu-id="8f708-103">Penyebaran Active Directory Federation Services (AD FS) menggunakan infrastruktur lokal Anda untuk mengotentikasi pengguna untuk layanan Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f708-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="8f708-104">Dengan masuk gabungan, Anda dapat mengaktifkan pengguna untuk masuk ke layanan dan perangkat lunak Office 365 sebagai aplikasi Layanan (SAAS) yang terintegrasi dengan Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8f708-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="8f708-105">Masuk gabungan mengotentikasi pengguna terhadap direktori aktif di tempat melalui AD FS.</span><span class="sxs-lookup"><span data-stu-id="8f708-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="8f708-106">Selain itu, pada jaringan korporat, pengguna tidak akan diminta untuk memasukkan kembali kata sandi mereka.</span><span class="sxs-lookup"><span data-stu-id="8f708-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="8f708-107">[Advisor penyebaran AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) memberi Anda panduan langkah demi langkah untuk menggelar infrastruktur AD FS lokal yang mengautentikasi pengguna untuk layanan Microsoft 365 dan Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f708-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="8f708-108">Dengan panduan ini, organisasi Anda bisa meninjau komponen dan persyaratan AD FS, mendapatkan dan menginstal sertifikat SSL yang diperlukan untuk penggunaan, dan menginstal server proksi aplikasi web yang diperlukan.</span><span class="sxs-lookup"><span data-stu-id="8f708-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
