---
title: Perilaku konsistensi Encyguid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705736"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="19b0d-102">Perilaku konsistensi Encyguid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="19b0d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="19b0d-103">Azure AD menyambung (versi 1.1.524.0 dan setelah) sekarang memfasilitasi penggunaan msDS-konsistensi Encyguid sebagai sourceAnchor atribut.</span><span class="sxs-lookup"><span data-stu-id="19b0d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="19b0d-104">Saat menggunakan fitur ini, Azure AD menyambung secara otomatis mengkonfigurasi aturan sinkronisasi untuk:</span><span class="sxs-lookup"><span data-stu-id="19b0d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="19b0d-105">Gunakan msDS-konsistensi Encyguid sebagai sourceAnchor atribut untuk objek pengguna.</span><span class="sxs-lookup"><span data-stu-id="19b0d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="19b0d-106">ObjectGUID digunakan untuk jenis objek lainnya.</span><span class="sxs-lookup"><span data-stu-id="19b0d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="19b0d-107">Untuk setiap objek pengguna AD lokal yang atribut msDS-Konsistencyguid tidak diisi, Azure AD menyambung menulis objectGUID nilai kembali ke atribut msDS-Konsistencyguid di direktori aktif di tempat.</span><span class="sxs-lookup"><span data-stu-id="19b0d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="19b0d-108">Setelah atribut msDS-Konsistencyguid diisi, Azure AD menyambung kemudian ekspor objek ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="19b0d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="19b0d-109">**Catatan:** Setelah objek AD lokal diimpor ke Azure AD menyambung (yaitu, diimpor ke Ruang konektor AD dan diproyeksikan ke metaverse), Anda tidak dapat mengubah nilai sourceAnchor lagi.</span><span class="sxs-lookup"><span data-stu-id="19b0d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="19b0d-110">Untuk menentukan nilai sourceAnchor untuk objek AD lokal tertentu, konfigurasikan atribut msDS-konsistensi Encyguid sebelum diimpor ke Azure AD menyambung.</span><span class="sxs-lookup"><span data-stu-id="19b0d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="19b0d-111">Untuk informasi lebih lanjut tentang SourceAnchor dan konsistensi Encyguid, lihat berikut ini: [AZURE AD menyambung: konsep desain](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="19b0d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

