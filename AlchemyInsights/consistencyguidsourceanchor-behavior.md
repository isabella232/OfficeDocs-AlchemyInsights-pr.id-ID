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
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927656"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="0a1cd-102">ConsistencyGuid / sourceAnchor perilaku</span><span class="sxs-lookup"><span data-stu-id="0a1cd-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="0a1cd-p101">Azure iklan Connect (versi 1.1.524.0 dan setelah) sekarang memfasilitasi penggunaan msDS-ConsistencyGuid sebagai atribut sourceAnchor. Bila menggunakan fitur ini, Azure iklan terhubung secara otomatis mengkonfigurasi aturan sinkronisasi untuk:</span><span class="sxs-lookup"><span data-stu-id="0a1cd-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="0a1cd-p102">Menggunakan msDS-ConsistencyGuid sebagai atribut sourceAnchor untuk objek pengguna. ObjectGUID digunakan untuk jenis objek lain.</span><span class="sxs-lookup"><span data-stu-id="0a1cd-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="0a1cd-p103">Untuk setiap lokal pengguna AD objek yang msDS-ConsistencyGuid atribut tidak dihuni, Azure iklan menghubungkan menulis nilainya objectGUID kembali ke atribut msDS-ConsistencyGuid di Active Directory lokal. Setelah atribut msDS-ConsistencyGuid diisi, kemudian Azure iklan menghubungkan ekspor objek Azure iklan.</span><span class="sxs-lookup"><span data-stu-id="0a1cd-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="0a1cd-p104">**Catatan:** Sekali lokal iklan objek diimpor ke Azure iklan terhubung (yang diimpor ke Ruang konektor iklan dan diproyeksikan ke Metaverse), Anda tidak dapat mengubah nilai sourceAnchor lagi. Untuk menentukan nilai sourceAnchor untuk diberikan lokal iklan objek, mengkonfigurasi atribut msDS-ConsistencyGuid yang sebelum itu diimpor ke Azure iklan terhubung.</span><span class="sxs-lookup"><span data-stu-id="0a1cd-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="0a1cd-111">Untuk informasi lebih lanjut di SourceAnchor dan ConsistencyGuid, lihat berikut: [Azure iklan terhubung: Desain konsep](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="0a1cd-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

