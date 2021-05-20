---
title: Memecahkan masalah Pertahanan Microsoft untuk Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545271"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="4d28a-102">Memecahkan masalah Pertahanan Microsoft untuk Office 365</span><span class="sxs-lookup"><span data-stu-id="4d28a-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="4d28a-103">**Apakah Anda menyadari adanya penundaan dalam pengiriman pesan?**</span><span class="sxs-lookup"><span data-stu-id="4d28a-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="4d28a-104">Gunakan [opsi Pengiriman](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) Dinamis di Pertahanan Microsoft Anda untuk Office 365 Brankas Lampiran Dinamis.</span><span class="sxs-lookup"><span data-stu-id="4d28a-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="4d28a-105">Hal ini akan membantu menghindari penundaan pesan saat memproteksi penerima dari file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="4d28a-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="4d28a-106">**Apakah Anda ingin melaporkan positif palsu atau negatif palsu kepada Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="4d28a-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="4d28a-107">Gunakan [Submissions Explorer](https://protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="4d28a-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="4d28a-108">-\*\* Apakah Anda tahu bahwa Anda dapat mengaktifkan Brankas Tautan untuk email internal yang dikirim antar penerima di organisasi Anda?\*\* Ikuti langkah-langkah ini:</span><span class="sxs-lookup"><span data-stu-id="4d28a-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="4d28a-109">Buka [https://protection.office.com](https://protection.office.com) dan masuk dengan akun administrator global atau administrator keamanan.</span><span class="sxs-lookup"><span data-stu-id="4d28a-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="4d28a-110">Di panel navigasi kiri di bawah **Manajemen ancaman**, pilih **Opsi** \> **Brankas Tautan**.</span><span class="sxs-lookup"><span data-stu-id="4d28a-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="4d28a-111">Di bagian **Kebijakan yang berlaku untuk seluruh organisasi,** pilih kebijakan dan klik **Edit**.</span><span class="sxs-lookup"><span data-stu-id="4d28a-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="4d28a-112">Di **Pengaturan** bawah , aktifkan **Terapkan link aman ke pesan yang dikirim dalam organisasi**.</span><span class="sxs-lookup"><span data-stu-id="4d28a-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
