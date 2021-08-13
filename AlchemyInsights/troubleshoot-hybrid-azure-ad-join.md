---
title: Risoluzione dei problemi di Aggiunta ad Azure AD ibrido
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939275"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Risoluzione dei problemi di Aggiunta ad Azure AD ibrido

È consigliabile verificare che un dispositivo possa accedere agli endpoint di registrazione dispositivo nell'account di sistema usando lo [script di Test Device Registration Connectivity](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Se si stanno configurando le registrazioni dei dispositivi per la prima volta, è necessario rivedere [Introduzione alla gestione dei dispositivi in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) per informazioni su come impostare i dispositivi sotto il controllo di Azure AD.
1. Se i dispositivi vengono registrati direttamente in Azure AD e si sta eseguendo l’iscrizione di questi in Intune, assicurarsi, prima di tutto, di aver [configurato Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e avere le [licenze](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Assicurarsi di essere autorizzati a eseguire operazioni in Azure AD e Active Directory locale. Solo l’amministratore globale in Azure AD può gestire le impostazioni per la registrazione dei dispositivi. Inoltre, è necessario essere un amministratore di Active Directory e AD FS, se applicabile, se si stanno configurando le registrazioni automatiche in Active Directory locale.

Per altre informazioni sulla risoluzione di potenziali problemi con l’aggiunta ibrida, vedere [Risoluzione dei problemi di aggiunta ibrida](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Per la configurazione di dispositivi aggiunti ad Azure AD ibrido e la gestione dei dispositivi tramite il portale di Azure AD, vedere [Configurare dispositivi aggiunti ad Azure AD ibrido (aggiunto a un dominio locale)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) e [Gestire i dispositivi usando il portale di Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Per risolvere i problemi più comuni di Aggiunta ad Azure Active Directory (AD) ibrido, vedere le [domande frequenti su Aggiunta ad Azure AD ibrido](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
