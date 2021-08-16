---
title: Microsoft Teams - Accesso guest
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: 2c78fec14d43c5cbf6aebbc889d606eb2f6c4c64af85997f523d06872c911a0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012312"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams - Accesso guest

Se è necessaria assistenza per comunicare con utenti esterni all'organizzazione in Teams, è necessario decidere se utilizzare l'accesso guest o l'accesso esterno [(federazione)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)oppure è possibile utilizzare entrambi.

Verificare le [differenze per comprendere](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) le funzionalità disponibili per ognuna di queste.  Ad esempio, l'accesso esterno (federazione) consente comunicazioni 1:1, ad esempio Chat e Presenza.  Gli utenti federati non possono tuttavia Teams collaborazione.  Se si desidera che un utente esterno partecipi Teams conversazioni del canale o condividi file, è necessario attivare l'accesso guest.

**Opzione 1: attivare l'accesso guest** Nell'Teams di amministrazione, accedere a [Org Wide Impostazioni > Accesso guest](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) e attivare "Consenti accesso guest in Teams".  Per un tenant con tutte le altre impostazioni predefinite, questo dovrebbe essere tutto ciò che è necessario fare.  Per personalizzare la configurazione di Accesso guest, eseguire tutti i passaggi descritti nell'Elenco [di controllo per l'accesso guest.](https://docs.microsoft.com/microsoftteams/guest-access-checklist) Al termine, è necessario attendere fino [a 24 ore](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) per l'applicazione delle impostazioni.

Se si è certi di aver completato tutti i passaggi dell'elenco di controllo e sono state più di 24 ore, procedere e provare ad aggiungere un guest al [team.](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)

Per ulteriori informazioni, inclusi i video sulle modalità, vedere [Accesso guest in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Opzione 2: attivare l'accesso esterno (federazione)** Se si desidera attivare anche Accesso esterno (federazione), nell'interfaccia di amministrazione di Teams passare ad Accesso esterno a livello di organizzazione [Impostazioni >](https://admin.teams.microsoft.com/company-wide-settings/external-communications) e attivare "Gli utenti possono comunicare con gli utenti di Skype for Business e Teams" e quindi seguire tutti i passaggi descritti in Consentire agli utenti di Teams di chattare e comunicare con gli utenti di un'altra [organizzazione.](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)
