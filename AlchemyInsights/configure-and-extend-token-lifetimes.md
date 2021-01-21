---
title: Mengonfigurasi dan memperpanjang masa berlaku token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917003"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="04714-102">Mengonfigurasi dan memperpanjang masa berlaku token</span><span class="sxs-lookup"><span data-stu-id="04714-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="04714-103">Anda dapat menentukan seumur hidup dari token Access, SAML, atau ID yang diterbitkan oleh Microsoft Identity platform.</span><span class="sxs-lookup"><span data-stu-id="04714-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="04714-104">Anda dapat mengatur masa pakai token untuk semua aplikasi di organisasi Anda, untuk aplikasi multi-penyewa (multi-organisasi), atau untuk prinsip layanan tertentu di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="04714-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="04714-105">Untuk informasi selengkapnya, baca [masa hidup token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)yang dapat dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="04714-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="04714-106">Sebagai contoh, baca [contoh cara mengonfigurasi masa hidup token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="04714-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="04714-107">Untuk mempelajari cara mengonfigurasi seumur hidup dan kompatibilitas Token di Azure Active Directory B2C (Azure AD B2C), lihat [mengonfigurasi Token di B2C direktori aktif Azure](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="04714-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="04714-108">Artikel [mengonfigurasi perilaku sesi di Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) menguraikan metode masuk tunggal (SSO) yang digunakan di AZURE AD B2C dan membantu Anda memilih metode SSO yang paling tepat saat mengonfigurasi kebijakan Anda.</span><span class="sxs-lookup"><span data-stu-id="04714-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="04714-109">**Berapa lama token bertahan? Berapa lama waktu yang mereka miliki?**</span><span class="sxs-lookup"><span data-stu-id="04714-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="04714-110">Masa pakai Token adalah 1 jam dan seumur hidup dalam sesi 24 jam.</span><span class="sxs-lookup"><span data-stu-id="04714-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="04714-111">Ini berarti bahwa jika tidak ada permintaan yang dilakukan dalam 24 Jam, Anda perlu masuk lagi sebelum meminta token baru.</span><span class="sxs-lookup"><span data-stu-id="04714-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="04714-112">Setelah 30 Mei 2020, tidak ada penyewa baru yang dapat menggunakan kebijakan seumur hidup untuk mengonfigurasi token sesi dan refresh.</span><span class="sxs-lookup"><span data-stu-id="04714-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="04714-113">Penghentian akan terjadi dalam beberapa bulan setelah itu, yang berarti bahwa kami akan menghentikan menghormati tata sesi dan me-refresh Token yang sudah ada.</span><span class="sxs-lookup"><span data-stu-id="04714-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="04714-114">Anda masih bisa mengonfigurasi masa berlaku token Access setelah penghentian.</span><span class="sxs-lookup"><span data-stu-id="04714-114">You can still configure access token lifetimes after the deprecation.</span></span>






