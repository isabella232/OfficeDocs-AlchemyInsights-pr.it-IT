---
title: 2491 messaggi di posta elettronica di avviso provenienti dal criterio ' phishing recapitato a causa di override del tenant o dell'utente
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391356"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="d3d7a-102">Avvisare i messaggi di posta elettronica dal criterio ' phishing recapitato a causa del tenant o dell'utente</span><span class="sxs-lookup"><span data-stu-id="d3d7a-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="d3d7a-103">Un criterio di avviso predefinito denominato "phishing recapitato a causa del tenant o dell'utente" è stato implementato nei tenant con Office 365 ATP P1 e P2 licenses.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="d3d7a-104">Se è stato ricevuto questo avviso, ecco i passaggi da eseguire per esaminare:</span><span class="sxs-lookup"><span data-stu-id="d3d7a-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="d3d7a-105">Dal messaggio di avviso, fare clic su **Visualizza avviso** per passare alla pagina **avvisi** nel centro sicurezza & conformità.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="d3d7a-106">Selezionare l'avviso per visualizzare l'opzione per **visualizzare l'elenco** dei messaggi o visualizzare i messaggio **in Esplora**.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="d3d7a-107">Entrambe queste opzioni consentono di utilizzare i dettagli del messaggio, che include l'ID del messaggio.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="d3d7a-108">Si noti che il collegamento Esplora minacce filtra automaticamente i messaggi che corrispondono ai criteri di avviso.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="d3d7a-109">Potrebbe essere necessario modificare il filtro data in Esplora minacce.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="d3d7a-110">Il messaggio di phishing è stato recapitato a causa di una sostituzione configurata manualmente:</span><span class="sxs-lookup"><span data-stu-id="d3d7a-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="d3d7a-111">Un mittente o un dominio consentito impostato dall'utente.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="d3d7a-112">Un mittente o un dominio consentito impostato dall'amministratore in un criterio di protezione da posta indesiderata.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="d3d7a-113">Un indirizzo IP consentito in un criterio di filtro delle connessioni.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="d3d7a-114">Regola del flusso di posta (nota anche come regola di trasporto) configurata per consentire l'utilizzo dei messaggi.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="d3d7a-115">Se si ritiene che il messaggio sia stato contrassegnato erroneamente come phishing, utilizzare il [componente aggiuntivo dei messaggi del rapporto](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) di Outlook per inviare esempi di messaggi a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d3d7a-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>