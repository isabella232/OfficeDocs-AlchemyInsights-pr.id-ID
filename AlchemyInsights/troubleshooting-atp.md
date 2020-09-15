---
title: Pemecahan masalah proteksi ancaman tingkat lanjut Office 365
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658917"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="5a757-102">Pemecahan masalah proteksi ancaman tingkat lanjut Office 365</span><span class="sxs-lookup"><span data-stu-id="5a757-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="5a757-103">Apakah Anda melihat keterlambatan dalam pengiriman pesan?</span><span class="sxs-lookup"><span data-stu-id="5a757-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="5a757-104">Gunakan opsi [pengiriman dinamis](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) dalam kebijakan lampiran aman ATP Anda.</span><span class="sxs-lookup"><span data-stu-id="5a757-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="5a757-105">Ini akan membantu menghindari keterlambatan pesan sekaligus melindungi penerima dari file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="5a757-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="5a757-106">Apakah Anda ingin melaporkan positif palsu atau negatif palsu ke Microsoft?</span><span class="sxs-lookup"><span data-stu-id="5a757-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="5a757-107">Gunakan [link](https://www.microsoft.com/wdsi/filesubmission/) ini untuk mengirim file untuk dianalisis.</span><span class="sxs-lookup"><span data-stu-id="5a757-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="5a757-108">Apakah Anda tahu bahwa Anda bisa mengaktifkan proteksi link aman untuk email internal yang dikirim antar penerima di dalam organisasi Anda?</span><span class="sxs-lookup"><span data-stu-id="5a757-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="5a757-109">Ikuti langkah-langkah ini:</span><span class="sxs-lookup"><span data-stu-id="5a757-109">Follow these steps:</span></span>

  1. <span data-ttu-id="5a757-110">Masuk ke [https://protection.office.com](https://protection.office.com) dan masuk dengan akun administrator global atau administrator keamanan.</span><span class="sxs-lookup"><span data-stu-id="5a757-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="5a757-111">Di panel navigasi kiri di bawah **manajemen ancaman**, pilih **Policy** \> **link aman**kebijakan.</span><span class="sxs-lookup"><span data-stu-id="5a757-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="5a757-112">Di **kebijakan yang berlaku untuk seluruh bagian organisasi** , pilih kebijakan dan klik **Edit**.</span><span class="sxs-lookup"><span data-stu-id="5a757-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="5a757-113">Di bawah **pengaturan**, Aktifkan **Terapkan tautan aman ke pesan yang dikirim dalam organisasi**.</span><span class="sxs-lookup"><span data-stu-id="5a757-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
