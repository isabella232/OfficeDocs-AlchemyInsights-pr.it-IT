---
title: Migrazione da AIP a MIP/Etichettatura unificata nel Centro conformità
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825375"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrazione da AIP a MIP/Etichettatura unificata nel Centro conformità

Per passare dalle etichette AIP all'etichettatura unificata nel Centro sicurezza e conformità, procedere come segue:

**Attivare la protezione nel portale Azure**

1. Se non si è già fatto, aprire una nuova finestra del browser e [accedere al portale Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Passare al pannello **Azure Information Protection**. Ad esempio, nel menu Hub, fare clic su **Tutti i servizi** e iniziare a digitare **Informazioni** nella casella Filtro. Selezionare **Azure Information Protection**. Se non è mai stato effettuato l'accesso al pannello Azure Information Protection prima, consultare i [passaggi aggiuntivi](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) una tantum per aggiungere il pannello al portale. Per aprire il pannello Azure Information Protection, bisogna avere un [piano Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) o un piano Office 365 che includa Rights Management. Se si dispone di uno di questi abbonamenti, ma si visualizza un messaggio che dice che non è possibile trovare un abbonamento valido, [contattare il Supporto tecnico Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) o usare i canali di supporto standard.

2. Localizzare le opzioni del menu **Gestisci** e selezionare **Attivazione della protezione**. Fare clic su **Attiva**, quindi confermare l'operazione. Quando l'attivazione è completata, la Barra informazioni mostrerà **L'attivazione è stata completata**.

**Migrare le etichette di Azure Information Protection al Centro sicurezza e conformità di Office 365**

1. Assicurarsi di aver effettuato l'accesso come utente con autorizzazione da amministratore globale.

2. Passare al pannello **Azure Information Protection**.

3. Nell'opzione del menu **Gestisci** selezionare **Etichettatura unificata**.

4. Nel pannello **Azure Information Protection - Etichettatura unificata** fare clic su **Attiva** e seguire le istruzioni online.

**Nota**: verificare di disporre delle autorizzazioni appropriate prima di attivare la migrazione al Centro sicurezza e conformità. Per altre informazioni, vedere questi articoli:

1. [È necessario essere un amministratore globale per configurare Azure Information Protection o è possibile delegare l'operazione ad altri amministratori?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Informazioni importanti sui ruoli amministrativi dopo la migrazione al Centro sicurezza e conformità.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Per altre informazioni sulla migrazione da AIP all'Etichettatura unificata nel Centro sicurezza e conformità, consultare [Migrare le etichette](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
