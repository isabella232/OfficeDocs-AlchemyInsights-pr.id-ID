---
title: Masalah dengan atribut dan cakupan filter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481893"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="5c692-102">Masalah dengan atribut dan cakupan filter</span><span class="sxs-lookup"><span data-stu-id="5c692-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="5c692-103">**Masalah dengan nilai UPN yang berkonflik**</span><span class="sxs-lookup"><span data-stu-id="5c692-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="5c692-104">Hari kerja untuk penyediaan pengguna untuk Workday untuk provisioning pengguna AD memperlihatkan pesan kesalahan **Hybridsynchronizationactivedirectoryuserprincipalnamenotunique**.</span><span class="sxs-lookup"><span data-stu-id="5c692-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="5c692-105">Operasi gagal karena nilai UPN yang disediakan untuk penambahan/modifikasi bukan merupakan Forest Unique.</span><span class="sxs-lookup"><span data-stu-id="5c692-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="5c692-106">Detail kesalahan: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="5c692-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="5c692-107">Nilai **userPrincipalName** yang akan diatur oleh konektor workday saat membuat akun pengguna AD sudah ada di domain AD target.</span><span class="sxs-lookup"><span data-stu-id="5c692-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="5c692-108">Ini menyiratkan bahwa (1) pengguna sudah ada dan pemeriksaan ID yang cocok gagal untuk pengguna atau (2) aturan pembuatan UPN yang menghasilkan nilai berkonflik.</span><span class="sxs-lookup"><span data-stu-id="5c692-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="5c692-109">Berikut adalah langkah-langkah resolusi yang disarankan:</span><span class="sxs-lookup"><span data-stu-id="5c692-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="5c692-110">Jika pengguna sudah ada dan ID pencocokan yang sesuai gagal untuk menautkan akun Workday ke akun direktori aktif, periksa apakah atribut ID yang cocok (biasanya **idkaryawan**) dalam hari kerja dan iklan memiliki kecocokan yang sama persis.</span><span class="sxs-lookup"><span data-stu-id="5c692-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="5c692-111">Jika mereka tidak memiliki kecocokan, itu adalah masalah data yang perlu diperbaiki.</span><span class="sxs-lookup"><span data-stu-id="5c692-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="5c692-112">Misalnya, jika Idkaryawan dalam hari kerja adalah 001052 dan di 1052 AD, maka mesin provisioning akan gagal untuk menautkan kedua akun dan akan mencoba membuat pengguna yang sudah ada.</span><span class="sxs-lookup"><span data-stu-id="5c692-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="5c692-113">Solusi dalam kasus ini adalah mengubah nilai **idkaryawan** di AD untuk menyertakan angka nol terdepan untuk membuatnya 001052.</span><span class="sxs-lookup"><span data-stu-id="5c692-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="5c692-114">Jika ekspresi yang menghasilkan UPN tidak menghasilkan nilai unik, pertimbangkan menggunakan fungsi de-duplikasi **Selectuniquevalue** untuk menghasilkan nilai unik setiap kali.</span><span class="sxs-lookup"><span data-stu-id="5c692-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="5c692-115">**Hari kerja untuk penyediaan pengguna AD tidak mengatur nilai atribut manajer untuk akun pengguna AD**</span><span class="sxs-lookup"><span data-stu-id="5c692-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="5c692-116">Hari kerja ke pekerjaan penyediaan pengguna AD tidak mengatur nilai atribut **manajer** untuk akun pengguna AD.</span><span class="sxs-lookup"><span data-stu-id="5c692-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="5c692-117">Ada dua kemungkinan skenario saat perilaku ini terlihat:</span><span class="sxs-lookup"><span data-stu-id="5c692-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="5c692-118">Manajer di Workday tidak dapat diselesaikan ke akun pengguna AD terkait karena manajer tidak berada dalam lingkup.</span><span class="sxs-lookup"><span data-stu-id="5c692-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="5c692-119">Dalam skenario **beberapa domain AD** , manajer dalam hari kerja tidak ada di domain yang sama dengan pengguna.</span><span class="sxs-lookup"><span data-stu-id="5c692-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="5c692-120">Cobalah langkah-langkah ini untuk mengatasi masalah tersebut:</span><span class="sxs-lookup"><span data-stu-id="5c692-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="5c692-121">Jika Anda telah menetapkan filter lingkup, pertama-tama Periksa apakah manajer berada dalam lingkup dan itu memenuhi klausul pelingkupan.</span><span class="sxs-lookup"><span data-stu-id="5c692-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="5c692-122">Jika Manajer tidak memenuhi cakupan pelingkupan, Ubah filter sehingga manajer juga berada dalam lingkup operasi penyediaan.</span><span class="sxs-lookup"><span data-stu-id="5c692-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="5c692-123">Jika Anda memiliki beberapa domain, maka konektor memiliki batasan yang diketahui ketidakmampuan untuk mengatasi referensi manajer domain silang.</span><span class="sxs-lookup"><span data-stu-id="5c692-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="5c692-124">Untuk detail selengkapnya tentang mengonfigurasi workday untuk penyediaan otomatis, lihat [Tutorial: mengonfigurasi workday untuk penyediaan pengguna otomatis](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="5c692-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













