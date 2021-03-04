---
title: Masalah dengan pengguna tunggal
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430210"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="c1f27-102">Masalah dengan pengguna tunggal</span><span class="sxs-lookup"><span data-stu-id="c1f27-102">Problem with single user</span></span>

- <span data-ttu-id="c1f27-103">Pengguna mungkin belum ditetapkan karena layanan tidak memiliki kesempatan untuk mengevaluasi pengguna.</span><span class="sxs-lookup"><span data-stu-id="c1f27-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="c1f27-104">Tinjau panduan cara penyediaan jangka panjang serta bilah kemajuan pada halaman konfigurasi bawaan.</span><span class="sxs-lookup"><span data-stu-id="c1f27-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="c1f27-105">Jika status tetap ditentukan dalam bagian detail tambahan sebelum tanggal pengguna dibuat/diperbarui/dihapus, artinya kami belum mengevaluasi pengguna.</span><span class="sxs-lookup"><span data-stu-id="c1f27-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="c1f27-106">Dalam skenario ini, hal terbaik yang harus dilakukan adalah menunggu Layanan penyediaan untuk menyelesaikan.</span><span class="sxs-lookup"><span data-stu-id="c1f27-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="c1f27-107">Perhatikan bahwa layanan kami hanya mengetahui perubahan pada pengguna di sistem sumber (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="c1f27-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="c1f27-108">Harus ada perubahan yang valid dalam sistem sumber untuk Azure AD untuk mendeteksi perubahan dan alur ke direktori aktif.</span><span class="sxs-lookup"><span data-stu-id="c1f27-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="c1f27-109">Layanan penyediaan dievaluasi pengguna dan ditentukan tidak boleh ditetapkan:</span><span class="sxs-lookup"><span data-stu-id="c1f27-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="c1f27-110">Jika Anda telah mengatur filter pelingkupan atribut berbasis, pastikan bahwa pengguna memenuhi kriteria yang telah Anda tentukan.</span><span class="sxs-lookup"><span data-stu-id="c1f27-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="c1f27-111">Jika pengguna sudah ada di sistem target dan status pengguna dalam kecocokan sumber dan target, kami tidak akan melakukan tindakan lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="c1f27-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="c1f27-112">Layanan penyediaan berusaha untuk menyediakan pengguna dan gagal.</span><span class="sxs-lookup"><span data-stu-id="c1f27-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="c1f27-113">Untuk skenario ini, Tinjau tab pemecahan masalah dan rekomendasi dari log penyediaan:</span><span class="sxs-lookup"><span data-stu-id="c1f27-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="c1f27-114">Atribut yang diperlukan pada pengguna mungkin hilang di direktori aktif di tempat atau Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c1f27-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c1f27-115">Misalnya, aturan pembuatan userPrincipalName atau sAMAccountName tidak menghasilkan nilai yang tepat.</span><span class="sxs-lookup"><span data-stu-id="c1f27-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="c1f27-116">Atribut pencocokan (biasanya Idkaryawan) tidak mengatasi ke pengguna unik dalam direktori aktif di tempat atau Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c1f27-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c1f27-117">Misalnya, ada dua pengguna dengan Idkaryawan yang sama di AD dan layanan mengembalikan kode kesalahan mengindikasikan entri target duplikat untuk entri sumber yang sama.</span><span class="sxs-lookup"><span data-stu-id="c1f27-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="c1f27-118">Untuk meninjau log untuk satu pengguna dan grup, lihat [meninjau log penyediaan masalah dengan pengguna tertentu](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="c1f27-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
