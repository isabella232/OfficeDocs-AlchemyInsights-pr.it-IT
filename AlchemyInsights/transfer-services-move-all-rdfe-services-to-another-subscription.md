---
title: 'Servizi di trasferimento: spostare tutti i servizi di RDFE in un altro abbonamento'
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681477"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Servizi di trasferimento: spostare tutti i servizi di RDFE in un altro abbonamento

**Spostare risorse**

Le risorse di Azure possono essere spostate in un altro gruppo di risorse o in una sottoscrizione di Azure con la stessa sottoscrizione utilizzando Azure Portal, Azure PowerShell, Azure CLI o l'API REST per spostare le risorse.

Prima di poter spostare le risorse, vedere:

- [Elenco di controllo prima di spostare le risorse](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Servizi che possono essere spostati](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Come convalidare lo spostamento](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Spostare le linee guida per i servizi](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Per spostare le risorse esistenti in un altro gruppo di risorse o sottoscrizione, è possibile utilizzare:

- [Portale di Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [CLI di Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Esercitazione: [spostare le risorse di Azure in un altro gruppo di risorse o sottoscrizione](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Risoluzione degli errori di Azure Resource Manager**

Fare riferimento agli articoli riportati di seguito per informazioni sugli errori di distribuzione di Azure comuni e su come ottenere la risoluzione dei problemi. Se non è possibile trovare il codice di errore per l'errore di distribuzione, vedere [trovare il codice di errore](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Risoluzione dei problemi relativi agli errori di distribuzione](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Risoluzione dei problemi relativi allo spostamento delle risorse di Azure nel nuovo gruppo di risorse o sottoscrizione](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Si noti che, se si desidera aggiornare la sottoscrizione di Azure, ad esempio il passaggio da libero a pay-as-you-go, sarà necessario convertire l'abbonamento.

- Per eseguire l'aggiornamento di una versione di valutazione gratuita, vedere [Upgrade Your Free Trial or Microsoft Imagine Azure Subscription to pay-as-you-go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Per modificare un account Pay-As-You-Go, vedere [Change Your Azure pay-as-you-go Subscription to an different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Per aggiungere o associare una sottoscrizione di Azure al tenant di Azure Active Directory:**

1. Accedere e selezionare l'abbonamento che si desidera utilizzare dalla [pagina abbonamenti nel portale di Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Selezionare **Cambia directory**.
3. Esaminare gli eventuali avvisi visualizzati e quindi selezionare **Cambia**.
4. La directory viene modificata per la sottoscrizione e verrà visualizzato un messaggio di esito positivo.
5. Utilizzare la *directory* Switcher per passare alla nuova directory. Potrebbe essere necessario fino a 10 minuti affinché tutto venga visualizzato correttamente.

**Documenti consigliati**

- [Trasferimento della proprietà di una sottoscrizione di Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Spostare risorse in un nuovo gruppo di risorse o in una sottoscrizione](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gestire le risorse mediante il portale di Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
