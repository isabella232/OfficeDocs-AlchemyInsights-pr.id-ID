---
title: Mengonfigurasi titik koneksi Layanan (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036144"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="e6391-102">Mengonfigurasi titik koneksi Layanan (SCP)</span><span class="sxs-lookup"><span data-stu-id="e6391-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="e6391-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="e6391-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="e6391-104">**Alasan**: tidak dapat membaca objek SCP dan mendapatkan informasi penyewa Azure AD</span><span class="sxs-lookup"><span data-stu-id="e6391-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="e6391-105">**Resolusi**: rujuk ke bagian [mengonfigurasi titik koneksi Layanan](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="e6391-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="e6391-106">**Rencana tindakan**</span><span class="sxs-lookup"><span data-stu-id="e6391-106">**Action plan**</span></span>

- <span data-ttu-id="e6391-107">Periksa apakah perangkat telah menerima GPO untuk validasi terkendali.</span><span class="sxs-lookup"><span data-stu-id="e6391-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="e6391-108">Pastikan bahwa GPO telah membuat kunci registri.</span><span class="sxs-lookup"><span data-stu-id="e6391-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="e6391-109">Pastikan Anda memiliki 2 tombol yang dibuat dengan ID direktori Anda dan domain onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="e6391-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="e6391-110">**Mengonfigurasi pengaturan registri sisi klien untuk SCP**</span><span class="sxs-lookup"><span data-stu-id="e6391-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="e6391-111">Gunakan contoh berikut untuk membuat objek kebijakan grup (GPO) untuk menggunakan pengaturan registri yang mengonfigurasi entri SCP dalam registri perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="e6391-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="e6391-112">Buka konsol manajemen kebijakan grup dan buat GPO baru di domain Anda.</span><span class="sxs-lookup"><span data-stu-id="e6391-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="e6391-113">Berikan nama GPO yang baru Anda buat (misalnya, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="e6391-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="e6391-114">Edit GPO dan temukan jalur berikut: **pengaturan > konfigurasi komputer > pengaturan Windows > Registry**.</span><span class="sxs-lookup"><span data-stu-id="e6391-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="e6391-115">Klik kanan **Registry** dan pilih **item baru > Registry**.</span><span class="sxs-lookup"><span data-stu-id="e6391-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="e6391-116">Pada tab **umum** , konfigurasikan yang berikut ini:</span><span class="sxs-lookup"><span data-stu-id="e6391-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="e6391-117">**Tindakan**: Perbarui</span><span class="sxs-lookup"><span data-stu-id="e6391-117">**Action**: Update</span></span>
    
- <span data-ttu-id="e6391-118">**Sarang**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="e6391-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="e6391-119">**Jalur kunci**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="e6391-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="e6391-120">**Nama nilai**: tenantid</span><span class="sxs-lookup"><span data-stu-id="e6391-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="e6391-121">**Tipe nilai**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="e6391-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="e6391-122">**Data nilai**: id direktori atau GUID dari contoh Azure AD Anda (nilai ini bisa ditemukan di **portal Azure > direktori aktif azure > properti > id direktori**)</span><span class="sxs-lookup"><span data-stu-id="e6391-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="e6391-123">Klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="e6391-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="e6391-124">Klik kanan **Registry** dan pilih **item baru > Registry**.</span><span class="sxs-lookup"><span data-stu-id="e6391-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="e6391-125">Pada tab **umum** , konfigurasikan yang berikut ini:</span><span class="sxs-lookup"><span data-stu-id="e6391-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="e6391-126">**Tindakan**: Perbarui</span><span class="sxs-lookup"><span data-stu-id="e6391-126">**Action**: Update</span></span>
    
- <span data-ttu-id="e6391-127">**Sarang**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="e6391-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="e6391-128">**Jalur kunci**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="e6391-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="e6391-129">**Nama nilai**: tenantname</span><span class="sxs-lookup"><span data-stu-id="e6391-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="e6391-130">**Tipe nilai**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="e6391-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="e6391-131">**Data nilai**: nama domain Anda yang diverifikasi jika Anda menggunakan lingkungan gabungan seperti AD FS.</span><span class="sxs-lookup"><span data-stu-id="e6391-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="e6391-132">Nama domain Anda yang diverifikasi atau nama domain onmicrosoft.com Anda (misalnya, contoso. onmicrosoft). com jika Anda menggunakan lingkungan terkelola</span><span class="sxs-lookup"><span data-stu-id="e6391-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="e6391-133">Klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="e6391-133">Click **OK**.</span></span>

7. <span data-ttu-id="e6391-134">Tutup editor untuk GPO yang baru dibuat.</span><span class="sxs-lookup"><span data-stu-id="e6391-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="e6391-135">Tautkan GPO yang baru dibuat ke ou yang diinginkan yang berisi komputer gabungan domain yang menjadi bagian dari populasi peluncuran yang terkontrol.</span><span class="sxs-lookup"><span data-stu-id="e6391-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="e6391-136">Untuk informasi selengkapnya, lihat [validasi terkontrol hibrid AZURE AD Join-AZURE AD | Dokumen Microsoft](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) dan  [pemecahan masalah hibrid perangkat gabungan Azure Active Directory | Dokumen Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="e6391-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









