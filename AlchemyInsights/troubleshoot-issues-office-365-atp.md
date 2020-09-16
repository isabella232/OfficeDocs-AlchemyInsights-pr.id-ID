---
title: Memecahkan masalah dengan Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758068"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="cee95-102">Memecahkan masalah dengan Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="cee95-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="cee95-103">**Perhatikan keterlambatan pengiriman pesan email**?</span><span class="sxs-lookup"><span data-stu-id="cee95-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="cee95-104">Coba gunakan opsi pengiriman dinamis untuk kebijakan lampiran aman ATP Anda.</span><span class="sxs-lookup"><span data-stu-id="cee95-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="cee95-105">Ini akan menghindari keterlambatan pengiriman pesan email sekaligus melindungi penerima dari file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="cee95-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="cee95-106">**Apakah Anda ingin melaporkan kesalahan positif palsu atau negatif palsu**?</span><span class="sxs-lookup"><span data-stu-id="cee95-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="cee95-107">Gunakan link ini untuk mengirim file Anda untuk dianalisis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="cee95-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="cee95-108">**Tahukah Anda bahwa Anda bisa mengaktifkan proteksi tautan aman ATP untuk email yang dikirim di antara orang di organisasi Anda**?</span><span class="sxs-lookup"><span data-stu-id="cee95-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="cee95-109">Ikuti langkah-langkah ini:</span><span class="sxs-lookup"><span data-stu-id="cee95-109">Follow these steps:</span></span>
    1. <span data-ttu-id="cee95-110">Masuk ke https://protection.office.com , dan masuk.</span><span class="sxs-lookup"><span data-stu-id="cee95-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="cee95-111">Masuk ke **Threat management**  >  **Policy**  >  **tautan aman**kebijakan manajemen ancaman.</span><span class="sxs-lookup"><span data-stu-id="cee95-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="cee95-112">Di bawah **kebijakan yang berlaku untuk penerima tertentu**, Edit (atau tambahkan) sebuah kebijakan.</span><span class="sxs-lookup"><span data-stu-id="cee95-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="cee95-113">Pilih **Terapkan tautan aman ke pesan yang dikirim dalam organisasi**.</span><span class="sxs-lookup"><span data-stu-id="cee95-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="cee95-114">Simpan kebijakan Anda, dan Perbolehkan sekitar 30 menit agar perubahan dapat dilakukan melalui Datacenter Anda.</span><span class="sxs-lookup"><span data-stu-id="cee95-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="cee95-115">Untuk mendapatkan bantuan lainnya dengan ATP, lihat [proteksi ancaman tingkat lanjut Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="cee95-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>