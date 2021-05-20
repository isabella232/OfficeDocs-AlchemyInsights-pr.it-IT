---
title: 2491 Avvisa i messaggi di posta elettronica dal criterio "Phish Delivered due to tenant or user override"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544582"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="416d0-102">Messaggi di posta elettronica di avviso dal criterio "Phish Delivered due to tenant or user override"</span><span class="sxs-lookup"><span data-stu-id="416d0-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="416d0-103">Un criterio di avviso predefinito denominato "Phish Delivered due to tenant or user override" è stato implementare ai tenant con Microsoft Defender per le licenze P1 e P2 Office 365.</span><span class="sxs-lookup"><span data-stu-id="416d0-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="416d0-104">Se hai ricevuto questo avviso, ecco i passaggi da analizzare:</span><span class="sxs-lookup"><span data-stu-id="416d0-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="416d0-105">Nel messaggio di avviso fare clic **su** Visualizza avviso per passare alla **pagina Avvisi** nel Centro sicurezza & conformità.</span><span class="sxs-lookup"><span data-stu-id="416d0-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="416d0-106">Seleziona l'avviso per visualizzare l'opzione **Visualizza elenco messaggi** o Visualizza messaggi in Esplora **risorse.**</span><span class="sxs-lookup"><span data-stu-id="416d0-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="416d0-107">Entrambe queste opzioni visualizzano i dettagli del messaggio, che include l'ID messaggio.</span><span class="sxs-lookup"><span data-stu-id="416d0-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="416d0-108">Tieni presente che il collegamento Esplora minacce filtra automaticamente i messaggi che soddisfano i criteri di avviso.</span><span class="sxs-lookup"><span data-stu-id="416d0-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="416d0-109">Potrebbe essere necessario modificare il filtro data in Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="416d0-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="416d0-110">Il messaggio di phishing è stato recapitato a causa di una sostituzione configurata manualmente:</span><span class="sxs-lookup"><span data-stu-id="416d0-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="416d0-111">Mittente o dominio consentito impostato dall'utente.</span><span class="sxs-lookup"><span data-stu-id="416d0-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="416d0-112">Un mittente o un dominio consentito impostato dall'amministratore in un criterio di protezione da posta indesiderata.</span><span class="sxs-lookup"><span data-stu-id="416d0-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="416d0-113">Un indirizzo IP consentito in un criterio filtro connessioni.</span><span class="sxs-lookup"><span data-stu-id="416d0-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="416d0-114">Una regola del flusso di posta (nota anche come regola di trasporto) configurata per consentire l'ingresso dei messaggi.</span><span class="sxs-lookup"><span data-stu-id="416d0-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="416d0-115">Se si ritiene che il messaggio sia stato erroneamente contrassegnato come phish, utilizzare il Outlook componente aggiuntivo [Segnala](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) messaggio per inviare esempi di messaggi a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="416d0-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
