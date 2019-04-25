---
title: ConsistencyGuid / sourceAnchor perilaku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408111"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="0081d-102">ConsistencyGuid / sourceAnchor perilaku</span><span class="sxs-lookup"><span data-stu-id="0081d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="0081d-103">Azure iklan Connect (versi 1.1.524.0 dan setelah) sekarang memfasilitasi penggunaan msDS-ConsistencyGuid sebagai atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="0081d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="0081d-104">Bila menggunakan fitur ini, Azure iklan terhubung secara otomatis mengkonfigurasi aturan sinkronisasi untuk:</span><span class="sxs-lookup"><span data-stu-id="0081d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="0081d-105">Menggunakan msDS-ConsistencyGuid sebagai atribut sourceAnchor untuk objek pengguna.</span><span class="sxs-lookup"><span data-stu-id="0081d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="0081d-106">ObjectGUID digunakan untuk jenis objek lain.</span><span class="sxs-lookup"><span data-stu-id="0081d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="0081d-107">Untuk setiap lokal pengguna AD objek yang msDS-ConsistencyGuid atribut tidak dihuni, Azure iklan menghubungkan menulis nilainya objectGUID kembali ke atribut msDS-ConsistencyGuid di Active Directory lokal.</span><span class="sxs-lookup"><span data-stu-id="0081d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="0081d-108">Setelah atribut msDS-ConsistencyGuid diisi, kemudian Azure iklan menghubungkan ekspor objek Azure iklan.</span><span class="sxs-lookup"><span data-stu-id="0081d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="0081d-109">**Catatan:** Sekali lokal iklan objek diimpor ke Azure iklan terhubung (yang diimpor ke Ruang konektor iklan dan diproyeksikan ke Metaverse), Anda tidak dapat mengubah nilai sourceAnchor lagi.</span><span class="sxs-lookup"><span data-stu-id="0081d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="0081d-110">Untuk menentukan nilai sourceAnchor untuk diberikan lokal iklan objek, mengkonfigurasi atribut msDS-ConsistencyGuid yang sebelum itu diimpor ke Azure iklan terhubung.</span><span class="sxs-lookup"><span data-stu-id="0081d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="0081d-111">Untuk informasi lebih lanjut di SourceAnchor dan ConsistencyGuid, lihat berikut: [Azure iklan terhubung: Desain konsep](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="0081d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

