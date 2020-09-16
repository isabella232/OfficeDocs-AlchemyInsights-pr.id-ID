---
title: Perilaku konsistensi GUID/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756286"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="3aa86-102">Perilaku konsistensi GUID/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="3aa86-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="3aa86-103">Azure AD Connect (versi 1.1.524.0 dan setelahnya) kini memfasilitasi penggunaan msDS-Konsistencyguid sebagai atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="3aa86-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="3aa86-104">Saat menggunakan fitur ini, Azure AD Connect mengonfigurasi aturan sinkronisasi secara otomatis untuk:</span><span class="sxs-lookup"><span data-stu-id="3aa86-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="3aa86-105">Gunakan msDS-Konsistencyguid sebagai atribut sourceAnchor untuk objek pengguna.</span><span class="sxs-lookup"><span data-stu-id="3aa86-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="3aa86-106">ObjectGUID digunakan untuk tipe objek lainnya.</span><span class="sxs-lookup"><span data-stu-id="3aa86-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="3aa86-107">Untuk objek pengguna AD lokal yang diberikan yang msDS-Konsistencyguid atribut tidak terisi, Azure AD Connect menulis nilai objectGUID kembali ke atribut msDS-Konsistencyguid dalam direktori aktif di tempat.</span><span class="sxs-lookup"><span data-stu-id="3aa86-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="3aa86-108">Setelah atribut msDS-Konsistencyguid diisi, maka Azure AD Connect lalu mengekspor objek ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3aa86-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="3aa86-109">**Catatan:** Setelah objek AD di tempat diimpor ke Azure AD Connect (yang diimpor ke dalam ruang konektor AD dan diproyeksikan ke dalam metaverse), Anda tidak bisa mengubah nilai penghitungnya lagi.</span><span class="sxs-lookup"><span data-stu-id="3aa86-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="3aa86-110">Untuk menentukan nilai sourceAnchor untuk objek AD di tempat yang diberikan, konfigurasikan atribut msDS-Konsistencyguid sebelum diimpor ke Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3aa86-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="3aa86-111">Untuk informasi selengkapnya tentang SourceAnchor dan Konsistencyguid, lihat yang berikut ini: [AZURE AD Connect: konsep desain](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="3aa86-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

