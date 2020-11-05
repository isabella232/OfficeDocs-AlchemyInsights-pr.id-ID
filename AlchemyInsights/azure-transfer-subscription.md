---
title: Mentransfer kepemilikan tagihan Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922078"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="43491-102">Mentransfer kepemilikan tagihan Azure</span><span class="sxs-lookup"><span data-stu-id="43491-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="43491-103">Masuk ke [Azure portal](https://portal.azure.com/) sebagai administrator akun tagihan yang memiliki langganan yang ingin Anda transfer.</span><span class="sxs-lookup"><span data-stu-id="43491-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="43491-104">Jika tidak yakin apakah Anda dan administrator, atau jika Anda perlu menentukan siapa, lihat [menentukan administrator tagihan akun](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="43491-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="43491-105">Cari **biaya manajemen + tagihan**.</span><span class="sxs-lookup"><span data-stu-id="43491-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="43491-106">Pilih **langganan** dari panel kiri.</span><span class="sxs-lookup"><span data-stu-id="43491-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="43491-107">Bergantung pada akses, Anda mungkin perlu memilih lingkup tagihan lalu **langganan** atau **langganan Azure**.</span><span class="sxs-lookup"><span data-stu-id="43491-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="43491-108">Pilih **transfer kepemilikan tagihan** untuk langganan yang ingin Anda transfer</span><span class="sxs-lookup"><span data-stu-id="43491-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="43491-109">Masukkan alamat email pengguna yang merupakan administrator tagihan akun yang akan menjadi pemilik baru untuk langganan lalu pilih **Kirim permintaan transfer**</span><span class="sxs-lookup"><span data-stu-id="43491-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="43491-110">Pengguna mendapatkan email dengan instruksi untuk meninjau permintaan transfer Anda.</span><span class="sxs-lookup"><span data-stu-id="43491-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="43491-111">Untuk menyetujui permintaan transfer, pengguna akan memilih link dalam email dan mengikuti instruksi.</span><span class="sxs-lookup"><span data-stu-id="43491-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="43491-112">**Catatan** : jika Anda mentransfer kepemilikan tagihan langganan Anda ke akun pengguna di penyewa Azure AD lainnya, semua penetapan [Access Control (RBAC) berbasis peran](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)untuk mengelola sumber daya dalam langganan dihapus secara permanen.</span><span class="sxs-lookup"><span data-stu-id="43491-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="43491-113">Hanya pemilik baru yang akan memiliki akses untuk mengelola sumber daya dalam metode berlangganan.</span><span class="sxs-lookup"><span data-stu-id="43491-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="43491-114">Untuk informasi selengkapnya, lihat [mentransfer langganan ke pengguna di penyewa AZURE AD lainnya](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="43491-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="43491-115">**Dokumen yang direkomendasikan**</span><span class="sxs-lookup"><span data-stu-id="43491-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="43491-116">Mentransfer kepemilikan tagihan Azure langganan ke akun lain</span><span class="sxs-lookup"><span data-stu-id="43491-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="43491-117">Tentang mentransfer kepemilikan tagihan untuk langganan Azure</span><span class="sxs-lookup"><span data-stu-id="43491-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="43491-118">Mentransfer Visual Studio, Jaringan mitra Microsoft (MPN) dan membayar saat Anda menggunakan langganan dev/uji</span><span class="sxs-lookup"><span data-stu-id="43491-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="43491-119">Tanya Jawab Umum kepemilikan transfer</span><span class="sxs-lookup"><span data-stu-id="43491-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="43491-120">Memecahkan masalah pengalihan kepemilikan</span><span class="sxs-lookup"><span data-stu-id="43491-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
