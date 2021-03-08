---
title: Log kata sandi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527184"
---
# <a name="password-logs"></a><span data-ttu-id="df6e9-102">Log kata sandi</span><span class="sxs-lookup"><span data-stu-id="df6e9-102">Password logs</span></span>

<span data-ttu-id="df6e9-103">**Saya mengalami masalah saat mengakses log audit penyetelan ulang kata sandi**</span><span class="sxs-lookup"><span data-stu-id="df6e9-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="df6e9-104">Untuk memecahkan masalah terkait akses ke log penyetelan ulang kata sandi, lakukan langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="df6e9-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="df6e9-105">Pastikan Anda memiliki wewenang untuk melihat log audit.</span><span class="sxs-lookup"><span data-stu-id="df6e9-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="df6e9-106">Hanya peran berikut yang diizinkan:</span><span class="sxs-lookup"><span data-stu-id="df6e9-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="df6e9-107">Administrator global</span><span class="sxs-lookup"><span data-stu-id="df6e9-107">Global administrator</span></span>
 - <span data-ttu-id="df6e9-108">Administrator keamanan</span><span class="sxs-lookup"><span data-stu-id="df6e9-108">Security administrator</span></span>
 - <span data-ttu-id="df6e9-109">Pembaca keamanan</span><span class="sxs-lookup"><span data-stu-id="df6e9-109">Security reader</span></span>

<span data-ttu-id="df6e9-110">**Saya ingin melihat semua kejadian ulang kata sandi mengaudit dari waktu yang saya gunakan pada awalnya**</span><span class="sxs-lookup"><span data-stu-id="df6e9-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="df6e9-111">Acara pengaturan ulang kata sandi hingga 120.000 disimpan dalam laporan 30 hari terakhir.</span><span class="sxs-lookup"><span data-stu-id="df6e9-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="df6e9-112">Batas maksimal ini berlaku untuk UI saat mengunduh CSV.</span><span class="sxs-lookup"><span data-stu-id="df6e9-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="df6e9-113">1.000.000 acara tersedia melalui PowerShell.</span><span class="sxs-lookup"><span data-stu-id="df6e9-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="df6e9-114">Untuk informasi selengkapnya, lihat link di bawah ini:</span><span class="sxs-lookup"><span data-stu-id="df6e9-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="df6e9-115">Acara reset kata sandi layanan mandiri dari laporan Azure AD dan API kejadian</span><span class="sxs-lookup"><span data-stu-id="df6e9-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="df6e9-116">Cara mengunduh ulang kata sandi acara pendaftaran dengan cepat menggunakan PowerShell</span><span class="sxs-lookup"><span data-stu-id="df6e9-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="df6e9-117">**Saya ingin memahami kapabilitas pelaporan penyetelan ulang kata sandi**</span><span class="sxs-lookup"><span data-stu-id="df6e9-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="df6e9-118">Periksa siapa yang mendaftar atau mereset kata sandi dengan log reset kata sandi Azure AD audit di portal Azure di bawah **pengguna dan grup**.</span><span class="sxs-lookup"><span data-stu-id="df6e9-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="df6e9-119">Untuk informasi selengkapnya, lihat link berikut ini:</span><span class="sxs-lookup"><span data-stu-id="df6e9-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="df6e9-120">Gambaran umum laporan penyetelan ulang kata sandi</span><span class="sxs-lookup"><span data-stu-id="df6e9-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="df6e9-121">Cara menampilkan laporan penyetelan ulang kata sandi di portal Azure</span><span class="sxs-lookup"><span data-stu-id="df6e9-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="df6e9-122">Acara reset kata sandi layanan mandiri dari laporan Azure AD dan API kejadian</span><span class="sxs-lookup"><span data-stu-id="df6e9-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="df6e9-123">Cara mengunduh ulang kata sandi acara pendaftaran dengan cepat menggunakan PowerShell</span><span class="sxs-lookup"><span data-stu-id="df6e9-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


