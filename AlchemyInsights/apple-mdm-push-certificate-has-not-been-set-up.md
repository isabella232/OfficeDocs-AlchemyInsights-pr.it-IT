---
title: Il certificato Apple MDM push non è stato configurato
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431649"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="991d4-102">Il certificato Apple MDM push non è stato configurato</span><span class="sxs-lookup"><span data-stu-id="991d4-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="991d4-103">Per l'abbonamento non è stato configurato un certificato Apple MDM push, noto anche come certificato del servizio di notifica push Apple (APNS).</span><span class="sxs-lookup"><span data-stu-id="991d4-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="991d4-104">Se non è configurato un certificato Apple MDM push, non è possibile registrare e gestire dispositivi iOS e MacOS.</span><span class="sxs-lookup"><span data-stu-id="991d4-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="991d4-105">Dopo l'aggiunta del certificato in Intune, gli utenti potranno installare l'app Portale aziendale per registrare i propri dispositivi iOS.</span><span class="sxs-lookup"><span data-stu-id="991d4-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="991d4-106">Selezionare **"Accetto".**</span><span class="sxs-lookup"><span data-stu-id="991d4-106">Select **"I agree."**</span></span> <span data-ttu-id="991d4-107">per assegnare a Microsoft l'autorizzazione a inviare dati a Apple.</span><span class="sxs-lookup"><span data-stu-id="991d4-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="991d4-108">Selezionare **Scaricare il CSR** la richiesta di firma del certificato Intune necessaria per creare un certificato Apple MDM push.</span><span class="sxs-lookup"><span data-stu-id="991d4-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="991d4-109">Il file è utilizzato per richiedere un certificato di relazione di trust dal portale dei certificati push di Apple.</span><span class="sxs-lookup"><span data-stu-id="991d4-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="991d4-110">Selezionare **Creare il certificato MDM push** per andare sul portale dei certificati push di Apple.</span><span class="sxs-lookup"><span data-stu-id="991d4-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="991d4-111">Accedere con l'ID Apple aziendale e selezionare **Creare un certificato**.</span><span class="sxs-lookup"><span data-stu-id="991d4-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="991d4-112">Selezionare **Scegliere file**, cercare il file della richiesta di firma del certificato, quindi scegliere **Caricare**.</span><span class="sxs-lookup"><span data-stu-id="991d4-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="991d4-113">Nella pagina di conferma scegliere **Download** per scaricare il file del certificato (con estensione PEM) e salvare il file in locale.</span><span class="sxs-lookup"><span data-stu-id="991d4-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="991d4-114">**Nota**: il certificato è associato all'ID Apple usato per crearlo.</span><span class="sxs-lookup"><span data-stu-id="991d4-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="991d4-115">Come procedura consigliata, usare un ID Apple aziendale per le attività di gestione e verificare che la cassetta postale sia monitorata da più di una persona o usando una lista di distribuzione.</span><span class="sxs-lookup"><span data-stu-id="991d4-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="991d4-116">Non usare mai un ID Apple personale.</span><span class="sxs-lookup"><span data-stu-id="991d4-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="991d4-117">Usare lo stesso ID Apple per rinnovare il certificato push Apple ogni 12 mesi.</span><span class="sxs-lookup"><span data-stu-id="991d4-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="991d4-118">Inserire l'ID Apple usato per creare il certificato MDM push Apple.</span><span class="sxs-lookup"><span data-stu-id="991d4-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="991d4-119">Registrare questo ID come promemoria per quando è necessario rinnovare il certificato.</span><span class="sxs-lookup"><span data-stu-id="991d4-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="991d4-120">Cercare il file del certificato (con estensione PEM), scegliere **Aprire**, quindi scegliere **Caricare**.</span><span class="sxs-lookup"><span data-stu-id="991d4-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="991d4-121">Con il certificato push, Intune può registrare e gestire i dispositivi Apple.</span><span class="sxs-lookup"><span data-stu-id="991d4-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>