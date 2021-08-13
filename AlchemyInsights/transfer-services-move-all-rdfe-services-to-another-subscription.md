---
title: Servizi di trasferimento - Spostare tutti i servizi RDFE in un'altra sottoscrizione
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940064"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Servizi di trasferimento - Spostare tutti i servizi RDFE in un'altra sottoscrizione

**Spostare risorse**

Le risorse di Azure possono essere spostate in un'altra sottoscrizione di Azure o in un altro gruppo di risorse nella stessa sottoscrizione usando il portale di Azure, Azure PowerShell, l'interfaccia della riga di comando di Azure o l'API REST per spostare le risorse.

Prima di poter spostare le risorse, vedere:

- [Elenco di controllo prima di spostare le risorse](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Servizi che possono essere spostati](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Come convalidare lo spostamento](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Indicazioni per lo spostamento dei servizi](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Per spostare risorse esistenti in un altro gruppo di risorse o sottoscrizione, è possibile utilizzare:

- [Portale di Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Esercitazione: [Spostare le risorse di Azure in un altro gruppo di risorse o sottoscrizione](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Risolvere gli errori con Gestione risorse di Azure**

Fare riferimento agli articoli seguenti per informazioni su alcuni errori comuni di distribuzione di Azure e ricevere informazioni per risolverli. Se non è possibile trovare il codice di errore per l'errore di distribuzione, vedere [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Risolvere gli errori di distribuzione](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Risolvere i problemi di spostamento delle risorse di Azure in un nuovo gruppo di risorse o sottoscrizione](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Si noti che se si desidera aggiornare la sottoscrizione di Azure, ad esempio il passaggio da gratuito a pagamento, sarà necessario convertire l'abbonamento.

- Per aggiornare una versione di valutazione gratuita, vedere [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Per modificare un account con pagamento in base all'utente, vedere [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Per aggiungere o associare una sottoscrizione di Azure al tenant Azure Active Directory:**

1. Accedi e seleziona la sottoscrizione che vuoi usare dalla pagina [Abbonamenti nel portale di Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Selezionare **Cambia directory.**
3. Esaminare gli avvisi visualizzati e quindi selezionare **Cambia**.
4. La directory viene modificata per la sottoscrizione e verrà visualizzato un messaggio di esito positivo.
5. Utilizzare lo switcher *Directory* per passare alla nuova directory. La corretta visualizzazione di tutti gli elementi potrebbe richiedere fino a 10 minuti.

**Documenti consigliati**

- [Trasferimento della proprietà di una sottoscrizione di Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Spostare risorse in un nuovo gruppo di risorse o sottoscrizione](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gestire le risorse tramite il portale di Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
