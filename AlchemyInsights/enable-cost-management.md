---
title: Abilitare la gestione dei costi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 62f3cfb161c4f8da735bd288a2d6e22971b4aada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325467"
---
# <a name="enable-cost-management"></a>Abilitare la gestione dei costi

**Cosa significa "i costi sono disabilitati per l'organizzazione"?**

Le organizzazioni che utilizzano Enterprise Agreement (EA) o microsoft customer agreement (MCA) possono disabilitare l'accesso alle informazioni sui costi e ai prezzi.

Dopo l'accesso al portale di Azure, possono usare le API di fatturazione per ottenere a livello di programmazione le fatture (una volta acconsentito esplicitamente) e i dettagli sull'utilizzo.

**Come consentire ad altri utenti di accedere alle fatture**

1. Passare al **pannello Sottoscrizioni** nel portale di Azure.
2. Selezionare **Fatture** e quindi **Accesso alle fatture**.
3. Attivare l'accesso, seguito dal salvataggio delle modifiche, per consentire agli utenti con ruoli con ambito di sottoscrizione di scaricare le fatture.

**Nota:** l'amministratore dell'account può anche configurare l'invio delle fatture tramite posta elettronica. Per ulteriori informazioni, vedere [Ottenere la fattura tramite posta elettronica.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**Come aggiungere utenti al ruolo Lettore fatturazione**

1. Passare al **pannello Sottoscrizioni** nel portale di Azure.
2. Selezionare **Controllo di accesso (IAM)** e quindi fare clic su **Aggiungi.**
3. Scegliere **Lettore fatturazione** nella **pagina Seleziona un** ruolo.
4. Digitare il messaggio di posta elettronica dell'utente che si desidera invitare e quindi fare clic su **OK** per inviare l'invito.
5. Segui le istruzioni fornite nell'e-mail di invito per accedere come lettore di fatturazione. Per ulteriori informazioni, vedere [Concedere l'accesso alla fatturazione](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Documenti consigliati**

- [Abilitare le visualizzazioni DA e AO tramite il portale di EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Costi inclusi nella gestione dei costi](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Offerte Microsoft Azure supportate](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Esaminare i costi nell'analisi dei costi](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Fornire l'accesso alle informazioni di fatturazione](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Controllare l'accesso al Contratto del cliente Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






