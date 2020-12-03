---
title: Menghapus penyewa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564618"
---
# <a name="delete-tenant"></a><span data-ttu-id="33a53-102">Menghapus penyewa</span><span class="sxs-lookup"><span data-stu-id="33a53-102">Delete tenant</span></span>

<span data-ttu-id="33a53-103">Untuk menghapus Azure AD, pastikan:</span><span class="sxs-lookup"><span data-stu-id="33a53-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="33a53-104">Anda adalah administrator global di direktori.</span><span class="sxs-lookup"><span data-stu-id="33a53-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="33a53-105">Anda tidak masuk dengan akun yang memiliki direktori default seperti contoso.onmicrosoft.com dalam akun masuk, seperti admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="33a53-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="33a53-106">Hapus semua aplikasi aktif dalam direktori sebelum penghapusan.</span><span class="sxs-lookup"><span data-stu-id="33a53-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="33a53-107">Untuk menghapus aplikasi aktif, navigasikan ke pendaftaran aplikasi dan Hapus aplikasi yang sudah ada.</span><span class="sxs-lookup"><span data-stu-id="33a53-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="33a53-108">Tidak ada langganan aktif untuk layanan online Microsoft apa pun, seperti Microsoft Azure, Office 365 atau Azure AD premium yang terkait pada direktori.</span><span class="sxs-lookup"><span data-stu-id="33a53-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="33a53-109">Mentransfer langganan atau mempercepat pembatalan langganan aktif melalui dukungan dan tagihan Azure.</span><span class="sxs-lookup"><span data-stu-id="33a53-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="33a53-110">Pelajari selengkapnya tentang cara membatalkan langganan Office 365 dan Azure.</span><span class="sxs-lookup"><span data-stu-id="33a53-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="33a53-111">Untuk panduan tentang mengaitkan atau menambahkan langganan yang sudah ada ke penyewa, lihat [mengaitkan atau menambahkan langganan Azure ke penyewa AZURE AD Anda](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="33a53-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="33a53-112">Tidak ada lisensi aktif.</span><span class="sxs-lookup"><span data-stu-id="33a53-112">There are no Active license.</span></span> <span data-ttu-id="33a53-113">Untuk menghapus lisensi, lihat [cara menghapus langganan untuk menghapus lisensi](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="33a53-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="33a53-114">Tidak ada pengguna aktif lainnya dalam direktori selain diri Anda sebagai administrator global saat mencoba menghapus Azure AD.</span><span class="sxs-lookup"><span data-stu-id="33a53-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="33a53-115">Menghapus pengguna aktif lainnya, dan setiap dependensi pada nama domain kustom dalam penyewa juga harus dihapus, seperti pengguna yang dibuat dengan admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="33a53-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="33a53-116">Untuk langkah detail selengkapnya tentang cara:</span><span class="sxs-lookup"><span data-stu-id="33a53-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="33a53-117">Hapus "Azure Active Directory" atau "langganan", lihat [menghapus direktori Azure Active](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="33a53-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="33a53-118">Menghapus aplikasi dalam direktori, lihat [menghapus aplikasi](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="33a53-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
