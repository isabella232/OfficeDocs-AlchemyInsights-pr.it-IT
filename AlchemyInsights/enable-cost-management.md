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
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599081"
---
# <a name="enable-cost-management"></a>Abilitare la gestione dei costi

**Che cosa significa ' i costi sono disattivati per l'organizzazione '?**

Le organizzazioni che utilizzano gli account Enterprise Agreement (EA) o Microsoft Customer Agreement (MCA) possono disabilitare l'accesso alle informazioni sui costi e alle informazioni sui prezzi.

Dopo aver eseguito l'accesso al portale di Azure, è possibile utilizzare le API di fatturazione per ottenere fatture a livello di programmazione (una volta che sono stati scelti) e dettagli sull'utilizzo.

**Informazioni su come consentire agli utenti aggiuntivi di accedere alle fatture**

1. Andare a **Blade abbonamenti** nel portale di Azure.
2. Selezionare **fatture** e quindi **accedere alle fatture**.
3. Attivare l'accesso, seguito salvando le modifiche, per consentire agli utenti di ruoli con ambito sottoscrizione di scaricare le fatture.

> [!NOTE]
> L'amministratore dell'account può anche configurare la possibilità di inviare fatture tramite posta elettronica. Per ulteriori informazioni, vedere [ottenere la fattura tramite posta elettronica](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Come aggiungere gli utenti al ruolo del lettore di fatturazione**

1. Andare a **Blade abbonamenti** nel portale di Azure.
2. Selezionare **controllo di accesso (IAM)** e quindi fare clic su **Aggiungi**.
3. Scegliere **Billing Reader** nella pagina **selezionare un ruolo** .
4. Digitare il messaggio di posta elettronica dell'utente che si desidera invitare e quindi fare clic su **OK** per inviare l'invito.
5. Seguire le istruzioni fornite nel messaggio di posta elettronica invita per accedere come lettore di fatturazione. Per ulteriori informazioni, vedere [concedere l'accesso alla fatturazione](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Documenti consigliati**

- [Abilitare le visualizzazioni DA e AO tramite il portale EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Costi inclusi nella gestione dei costi](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Offerte di Microsoft Azure supportate](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Esaminare i costi nell'analisi dei costi](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Fornire l'accesso alle informazioni di fatturazione](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Controllare l'accesso a un contratto per i clienti Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






