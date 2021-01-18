---
title: Masalah penggabungan VM
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
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885208"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="3e6e1-102">Masalah penggabungan VM</span><span class="sxs-lookup"><span data-stu-id="3e6e1-102">Issue joining VMs</span></span>

<span data-ttu-id="3e6e1-103">Untuk mengatasi masalah yang terjadi saat mencoba bergabung dengan VM, lakukan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="3e6e1-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="3e6e1-104">Cobalah untuk masuk menggunakan format **UPN** (misalnya, ' joeuser@contoso.com ') dan bukan nama **SAMAccountName** (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="3e6e1-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="3e6e1-105">Pastikan bahwa Anda telah mengaktifkan sinkronisasi kata sandi sesuai dengan langkah-langkah yang diuraikan dalam panduan *memulai* .</span><span class="sxs-lookup"><span data-stu-id="3e6e1-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="3e6e1-106">Pastikan bahwa akun pengguna yang terpengaruh bukan akun eksternal dalam penyewa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3e6e1-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="3e6e1-107">Pengguna eksternal tidak bisa masuk ke domain terkelola karena layanan domain Azure AD tidak memiliki kredensial untuk akun pengguna tersebut.</span><span class="sxs-lookup"><span data-stu-id="3e6e1-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="3e6e1-108">Jika akun pengguna yang terpengaruh adalah akun pengguna berbasis awan saja, pastikan bahwa pengguna telah mengubah kata sandinya setelah Anda mengaktifkan layanan domain Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3e6e1-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="3e6e1-109">Langkah ini menyebabkan hash kredensial yang diperlukan untuk layanan domain Azure AD yang akan dihasilkan.</span><span class="sxs-lookup"><span data-stu-id="3e6e1-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="3e6e1-110">Jika akun pengguna yang terpengaruh disinkronisasi dari direktori lokal, verifikasi bahwa rilis Azure AD Connect yang direkomendasikan telah dikonfigurasikan untuk melakukan sinkronisasi penuh.</span><span class="sxs-lookup"><span data-stu-id="3e6e1-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="3e6e1-111">Jika masalah tetap ada setelah mengonfirmasi langkah 4, jalankan perintah berikut ini dari mesin sinkronisasi Anda:</span><span class="sxs-lookup"><span data-stu-id="3e6e1-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="3e6e1-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="3e6e1-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>