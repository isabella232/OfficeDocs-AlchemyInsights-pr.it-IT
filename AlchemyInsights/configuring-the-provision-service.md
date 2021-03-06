---
title: Configurazione del servizio di provisioning
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480750"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="19168-102">Configurazione del servizio di provisioning</span><span class="sxs-lookup"><span data-stu-id="19168-102">Configuring the Provision service</span></span>

<span data-ttu-id="19168-103">Per il funzionamento del provisioning automatico degli utenti, Azure AD richiede credenziali valide che gli consentono di connettersi all'API dei servizi Web Workday.</span><span class="sxs-lookup"><span data-stu-id="19168-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="19168-104">Inoltre, il pulsante Test Connection nell'app Workday to AD User Provisioning verifica anche se è in grado di connettersi all'agente di provisioning di Azure AD Connect associato al dominio AD.</span><span class="sxs-lookup"><span data-stu-id="19168-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="19168-105">Se il portale di Azure restituisce un errore al salvataggio delle credenziali, seguire i passaggi consigliati di seguito:</span><span class="sxs-lookup"><span data-stu-id="19168-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="19168-106">Verificare di aver configurato l'account utente del sistema di integrazione Workday come indicato nella sezione relativa all'esercitazione Configurare l'utente del sistema di [integrazione in Workday.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="19168-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="19168-107">Verificare che il servizio agente di provisioning di Azure AD Connect sia operativo nel server Windows locale tramite la console di gestione dei servizi.</span><span class="sxs-lookup"><span data-stu-id="19168-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="19168-108">È anche possibile controllare lo stato dell'agente nel portale di Azure facendo clic sul pulsante Visualizza agenti locali.</span><span class="sxs-lookup"><span data-stu-id="19168-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="19168-109">Assicurarsi di immettere il valore del campo "Nome utente workday" utilizzando il formato username@workday-tenant-name.</span><span class="sxs-lookup"><span data-stu-id="19168-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="19168-110">Se il workday-tenant-name non è presente, l'autenticazione di Workday ha esito negativo.</span><span class="sxs-lookup"><span data-stu-id="19168-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="19168-111">Se si sta configurando l'integrazione con il tenant di implementazione di Workday, prendere nota delle ore di inattività pianificate del tenant di Workday.</span><span class="sxs-lookup"><span data-stu-id="19168-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="19168-112">Workday ha pianificato il tempo di inattività per i tenant di implementazione nei fine settimana (in genere dal venerdì sera al sabato mattina) e gli errori di connettività durante questo periodo di inattività sono un problema noto che si risolve automaticamente non appena i tenant di implementazione sono di nuovo online.</span><span class="sxs-lookup"><span data-stu-id="19168-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="19168-113">In rari casi, questo errore può essere visualizzato anche se la password dell'utente del sistema di integrazione è cambiata a causa dell'aggiornamento del tenant o se l'account è in stato bloccato o scaduto.</span><span class="sxs-lookup"><span data-stu-id="19168-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="19168-114">Verificare lo stato dell'utente del sistema di integrazione con l'amministratore di Workday.</span><span class="sxs-lookup"><span data-stu-id="19168-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="19168-115">Per altri dettagli sulla configurazione di Workday per il provisioning automatizzato, consulta [Tutorial: configurare Workday per il provisioning utente automatico](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="19168-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
