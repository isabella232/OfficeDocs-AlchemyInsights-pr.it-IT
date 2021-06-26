---
title: Inoltrare la posta elettronica con Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117987"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="5d300-102">Configurare un dispositivo multifunzione o un'applicazione per l'invio di posta elettronica</span><span class="sxs-lookup"><span data-stu-id="5d300-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="5d300-103">Per informazioni sulle opzioni e le procedure, vedere [Come configurare un dispositivo multifunzione o un'applicazione per l'invio di posta elettronica con Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="5d300-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="5d300-104">Se di recente un dispositivo o un'applicazione ha smesso di funzionare, i motivi più comuni sono:</span><span class="sxs-lookup"><span data-stu-id="5d300-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="5d300-105">**Errori correlati all'autenticazione durante l'utilizzo dell'invio del client di autenticazione SMTP**: di recente sono state apportate alcune modifiche relative al funzionamento dell'autenticazione SMTP.</span><span class="sxs-lookup"><span data-stu-id="5d300-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="5d300-106">Per altre informazioni su come risolvere i problemi, vedere la sezione relativa alle autenticazioni non riuscite di [Risolvere i problemi relativi a stampanti, scanner e applicazioni line-of-business che inviano messaggi di posta elettronica tramite Microsoft 365 o Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span><span class="sxs-lookup"><span data-stu-id="5d300-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="5d300-107">**Microsoft accetta solo la versione TLS 1.2 durante la connessione sicura a Office 365**: se si usa la connessione protetta (TLS), verificare che il dispositivo dell'applicazione supporti TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="5d300-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="5d300-108">Per altre informazioni, vedere [Preparazione per TLS 1.2 in Office 365 e Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="5d300-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="5d300-109">Per altri problemi e soluzioni, vedere [Risolvere i problemi relativi a stampanti, scanner e applicazioni line-of-business che inviano posta elettronica usando Microsoft 365 o Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span><span class="sxs-lookup"><span data-stu-id="5d300-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="5d300-110">Per vedere i dispositivi interessati, passare al [Report sui client di autenticazione SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="5d300-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="5d300-p103">**Nota**: Exchange Online non supporta gli scenari di invio di posta elettronica in blocco. Per inviare messaggi di posta elettronica commerciali in blocco, ad esempio newsletter per i clienti, è necessario usare provider di terze parti specializzati per questi servizi.</span><span class="sxs-lookup"><span data-stu-id="5d300-p103">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios. To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
