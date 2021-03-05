---
title: Hari kerja untuk penyediaan pengguna AD masuk ke status karantina
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481877"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="0ebc6-102">Hari kerja untuk penyediaan pengguna AD masuk ke status karantina</span><span class="sxs-lookup"><span data-stu-id="0ebc6-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="0ebc6-103">**Hari kerja untuk penyediaan pengguna AD masuk ke status karantina dan tidak ada pengguna yang dibuat di AD**</span><span class="sxs-lookup"><span data-stu-id="0ebc6-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="0ebc6-104">Hari kerja untuk penyediaan pengguna AD Ayub telah masuk ke status karantina dan log audit memperlihatkan kejadian kegagalan ekspor dengan kesalahan pesan kesalahan **: OperationsError-SvcErr: terjadi kesalahan operasi. Tidak ada referensi Superior yang telah dikonfigurasikan untuk layanan direktori. Layanan Direktori oleh karena itu tidak dapat menerbitkan referensi ke objek di luar Forest ini**.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="0ebc6-105">Kesalahan ini biasanya muncul jika OU wadah direktori aktif tidak diatur dengan benar atau jika terdapat masalah dengan pemetaan ekspresi yang digunakan untuk **Parenternama**.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="0ebc6-106">Centang OU default untuk parameter **pengguna baru** untuk kesalahan ketik.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="0ebc6-107">Pastikan bahwa OU yang ditentukan sudah ada di iklan Anda.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="0ebc6-108">Jika Anda menggunakan **Parenternama** dalam pemetaan atribut, pastikan bahwa itu selalu mengevaluasi ke wadah yang diketahui dalam domain AD.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="0ebc6-109">Periksa kejadian ekspor dalam log audit untuk melihat nilai yang dihasilkan.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="0ebc6-110">Untuk detail selengkapnya tentang mengonfigurasi workday untuk penyediaan otomatis, lihat [Tutorial: mengonfigurasi workday untuk penyediaan pengguna otomatis](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="0ebc6-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

