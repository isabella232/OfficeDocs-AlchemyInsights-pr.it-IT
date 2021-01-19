---
title: 'Controller di dominio '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886848"
---
# <a name="domain-controller"></a>Controller di dominio

**Impossibile abilitare AAD-DS o errore restituito nell'ambito della distribuzione**

Per poter abilitare o distribuire Azure Active Directory Domain Services, seguire questi passaggi:

1. Se si sta usando una rete virtuale già esistente, controllare il gruppo di sicurezza di rete per rilevare eventuali regole che bloccano le porte necessarie per la sincronizzazione in AAD-DS nel portale https://aka.ms/aadds-networking.
2. Controllare se è presente la risposta al messaggio di errore nella guida disponibile in  https://aka.ms/aadds-troubleshoot-enable.
3. Provare a distribuire Azure Active Directory Domain Services in una nuova rete virtuale.
4. Seguire la Guida introduttiva su come distribuire AAD-DS, disponibile qui [Tutorial per creare Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. In caso di problemi con la distribuzione di Azure Active Directory Domain Services, vedere [Risolvere i problemi di Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) per risolvere gli errori comuni e ripristinare il servizio. 

**Impossibile disabilitare AAD-DS**

AAD-DS non può essere messo in pausa. Per interrompere l'utilizzo del dominio gestito è necessario eliminarlo.

Se si incorre in errori, per risolvere messaggi di errori comuni e i relativi passaggi per la risoluzione dei problemi e ripristinare il servizio, vedere [Risolvere i problemi di Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
