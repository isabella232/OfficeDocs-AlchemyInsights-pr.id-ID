---
title: Memecahkan masalah dengan Microsoft Defender untuk Office 365 (ATP)
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
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801410"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="a8a97-102">Memecahkan masalah dengan Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="a8a97-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="a8a97-103">**Perhatikan keterlambatan pengiriman pesan email** ?</span><span class="sxs-lookup"><span data-stu-id="a8a97-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="a8a97-104">Coba gunakan opsi pengiriman dinamis untuk kebijakan lampiran aman ATP Anda.</span><span class="sxs-lookup"><span data-stu-id="a8a97-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="a8a97-105">Ini akan menghindari keterlambatan pengiriman pesan email sekaligus melindungi penerima dari file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="a8a97-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="a8a97-106">**Apakah Anda ingin melaporkan kesalahan positif palsu atau negatif palsu** ?</span><span class="sxs-lookup"><span data-stu-id="a8a97-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="a8a97-107">Gunakan link ini untuk mengirim file Anda untuk dianalisis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="a8a97-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="a8a97-108">**Tahukah Anda bahwa Anda bisa mengaktifkan proteksi tautan aman ATP untuk email yang dikirim di antara orang di organisasi Anda** ?</span><span class="sxs-lookup"><span data-stu-id="a8a97-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="a8a97-109">Ikuti langkah-langkah ini:</span><span class="sxs-lookup"><span data-stu-id="a8a97-109">Follow these steps:</span></span>
    1. <span data-ttu-id="a8a97-110">Masuk ke https://protection.office.com , dan masuk.</span><span class="sxs-lookup"><span data-stu-id="a8a97-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="a8a97-111">Masuk ke **Threat management**  >  **Policy**  >  **tautan aman** kebijakan manajemen ancaman.</span><span class="sxs-lookup"><span data-stu-id="a8a97-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="a8a97-112">Di bawah **kebijakan yang berlaku untuk penerima tertentu** , Edit (atau tambahkan) sebuah kebijakan.</span><span class="sxs-lookup"><span data-stu-id="a8a97-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="a8a97-113">Pilih **Terapkan tautan aman ke pesan yang dikirim dalam organisasi** .</span><span class="sxs-lookup"><span data-stu-id="a8a97-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="a8a97-114">Simpan kebijakan Anda, dan Perbolehkan sekitar 30 menit agar perubahan dapat dilakukan melalui Datacenter Anda.</span><span class="sxs-lookup"><span data-stu-id="a8a97-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="a8a97-115">Untuk mendapatkan bantuan lainnya dengan ATP, lihat [Microsoft Defender untuk Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="a8a97-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>