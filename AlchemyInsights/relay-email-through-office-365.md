---
title: Inoltrare la posta elettronica con Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: e971593b7a67e1bb40243fc762bace6b87a35741
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745401"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="4ece3-102">Configurare un dispositivo multifunzione o un'applicazione per l'invio di posta elettronica tramite Office 365</span><span class="sxs-lookup"><span data-stu-id="4ece3-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="4ece3-103">Per informazioni sulle opzioni e le procedure, vedere [Come configurare un dispositivo multifunzione o un'applicazione per l'invio di posta elettronica con Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="4ece3-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="4ece3-104">**Nota:** se si dispone di un dispositivo o di un'applicazione che di recente ha smesso di funzionare, tenere presente che da qualche tempo è stata avviata la [disattivazione della crittografia 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) come previsto.</span><span class="sxs-lookup"><span data-stu-id="4ece3-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="4ece3-105">Per vedere i dispositivi interessati, andare al [Report sui client di autenticazione SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="4ece3-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="4ece3-106">Gli errori più comuni riguardano autenticazione, TLS, algoritmo di crittografia, algoritmo non corrispondente o connessione interrotta.</span><span class="sxs-lookup"><span data-stu-id="4ece3-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="4ece3-107">Per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="4ece3-107">To resolve this issue:</span></span>
 - <span data-ttu-id="4ece3-108">**Windows Server 2003 IIS SMTP smetteranno di funzionare ed è necessaria una versione più recente di Windows.**</span><span class="sxs-lookup"><span data-stu-id="4ece3-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="4ece3-109">Contattare il fornitore dell'applicazione o del dispositivo per verificare se è supportata una crittografia moderna o se è disponibile un aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="4ece3-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
