---
title: Menetapkan grup ke peran Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885069"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="1773f-102">Menetapkan grup ke peran Azure AD</span><span class="sxs-lookup"><span data-stu-id="1773f-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="1773f-103">Untuk menetapkan grup Azure AD dengan sumber kewenangan di Azure AD ke peran Azure AD, lakukan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="1773f-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="1773f-104">Membuat grup baru-untuk membuat grup baru:</span><span class="sxs-lookup"><span data-stu-id="1773f-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="1773f-105">untuk.</span><span class="sxs-lookup"><span data-stu-id="1773f-105">a.</span></span> <span data-ttu-id="1773f-106">Masuk ke Pusat admin Azure AD dengan **administrator peran istimewa** atau izin **administrator global** .</span><span class="sxs-lookup"><span data-stu-id="1773f-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="1773f-107">b.</span><span class="sxs-lookup"><span data-stu-id="1773f-107">b.</span></span> <span data-ttu-id="1773f-108">Pilih **grup > direktori aktif Azure > semua grup > grup baru**.</span><span class="sxs-lookup"><span data-stu-id="1773f-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="1773f-109">'s.</span><span class="sxs-lookup"><span data-stu-id="1773f-109">c.</span></span> <span data-ttu-id="1773f-110">Buat grup.</span><span class="sxs-lookup"><span data-stu-id="1773f-110">Create the group.</span></span>

2. <span data-ttu-id="1773f-111">Tetapkan peran ke grup selama pembuatan grup atau setelah grup dibuat.</span><span class="sxs-lookup"><span data-stu-id="1773f-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="1773f-112">untuk.</span><span class="sxs-lookup"><span data-stu-id="1773f-112">a.</span></span> <span data-ttu-id="1773f-113">Untuk menetapkan peran ke grup pada saat pembuatan grup, Aktifkan tombol Alihkan **AZURE AD bisa ditetapkan ke grup** dan Buat grup.</span><span class="sxs-lookup"><span data-stu-id="1773f-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="1773f-114">b.</span><span class="sxs-lookup"><span data-stu-id="1773f-114">b.</span></span> <span data-ttu-id="1773f-115">Untuk menetapkan peran ke grup setelah dibuat, navigasikan ke tab **peran yang ditetapkan** untuk grup yang baru dibuat, dan tetapkan peran ke grup.</span><span class="sxs-lookup"><span data-stu-id="1773f-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="1773f-116">**Mengelola keanggotaan grup yang ditetapkan untuk peran Azure AD**</span><span class="sxs-lookup"><span data-stu-id="1773f-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="1773f-117">Untuk mencegah elevasi hak istimewa, secara default, hanya administrator peran istimewa dan administrator global yang bisa mengubah keanggotaan grup yang ditetapkan pada peran.</span><span class="sxs-lookup"><span data-stu-id="1773f-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="1773f-118">Namun, mereka dapat memilih untuk menetapkan pemilik untuk grup tersebut dan mendelegasikan tugas ini.</span><span class="sxs-lookup"><span data-stu-id="1773f-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="1773f-119">Untuk detail selengkapnya tentang penetapan grup awan ke Azure AD, lihat [menetapkan peran iklan ke grup awan](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="1773f-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="1773f-120">Untuk detail selengkapnya tentang pemecahan masalah yang ditetapkan untuk grup awan, lihat [memecahkan masalah yang ditetapkan untuk grup awan](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="1773f-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





