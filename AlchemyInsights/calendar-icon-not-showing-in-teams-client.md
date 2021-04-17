---
title: Ikon Kalender tidak muncul di klien Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819956"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="cc932-102">Ikon Kalender tidak muncul di klien Teams</span><span class="sxs-lookup"><span data-stu-id="cc932-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="cc932-103">Tab Kalender di Teams memerlukan akses ke kotak surat Exchange melalui Layanan Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc932-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="cc932-104">Kotak surat Exchange bisa Online atau Lokal.</span><span class="sxs-lookup"><span data-stu-id="cc932-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="cc932-105">Untuk pengguna Online yang tidak melihat Tab Kalender, pastikan mereka [dilisensikan untuk kotak surat Exchange Online dan kotak surat diaktifkan](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="cc932-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="cc932-106">Jika pengguna memiliki kotak surat yang valid di Exchange Online, tetapi tetap tidak bisa melihat tab Kalender, Anda mungkin mengalami masalah jaringan.</span><span class="sxs-lookup"><span data-stu-id="cc932-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="cc932-107">Gunakan [Penganalisis Konektivitas Jarak Jauh Microsoft](https://testconnectivity.microsoft.com/) dan jalankan **Tes Konektivitas Layanan Web Microsoft Exchange** untuk pengguna yang terdampak.</span><span class="sxs-lookup"><span data-stu-id="cc932-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="cc932-108">Terakhir, perisa [Aplikasi Teams – Kebijakan penyiapan aplikasi](https://admin.teams.microsoft.com/policies/app-setup) untuk memastikan aplikasi Kalender tidak dihapus dari kebijakan yang diterapkan pada pengguna (kemungkinan besar kebijakan **Global (default skala Organisasi)**.</span><span class="sxs-lookup"><span data-stu-id="cc932-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="cc932-109">Jika pengguna Anda di rumah menggunakan Lokal, Anda perlu mengonfirmasi bahwa konfigurasi Hibrid Anda sehat.</span><span class="sxs-lookup"><span data-stu-id="cc932-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="cc932-110">Gunakan [Panduan Konfigurasi Hibrid](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) untuk memecahkan masalah.</span><span class="sxs-lookup"><span data-stu-id="cc932-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="cc932-111">Perhatikan bahwa [Teams membutuhkan Exchange 2016 CU3 atau lebih tinggi](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="cc932-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
