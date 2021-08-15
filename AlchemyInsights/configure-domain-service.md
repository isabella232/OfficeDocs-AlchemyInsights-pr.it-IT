---
title: Configurare il servizio di dominio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: cf8ea7d73adf36f71ae92abad48ef9b664eb0c96094a38750c86cf42958b5323
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994761"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Impossibile abilitare AAD-DS o errore restituito nell'ambito della distribuzione

Per poter abilitare o distribuire Azure Active Directory Domain Services, seguire questi passaggi:

1. Se si sta usando una rete virtuale già esistente, controllare il gruppo di sicurezza di rete per rilevare eventuali regole che bloccano le porte necessarie per la sincronizzazione in AAD-DS nel portale https://aka.ms/aadds-networking.
2. Controllare se è presente la risposta al messaggio di errore nella guida disponibile in  https://aka.ms/aadds-troubleshoot-enable.
3. Provare a distribuire Azure Active Directory Domain Services in una nuova rete virtuale.
4. Seguire la Guida introduttiva su come distribuire AAD-DS: [Creare e configurare Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. In caso di problemi con la distribuzione di Azure Active Directory Domain Services, vedere [Risolvere i problemi di Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) per risolvere gli errori comuni e ripristinare il servizio. 

**Impossibile disabilitare AAD-DS**

AAD-DS non può essere messo in pausa. Per interrompere l'utilizzo del dominio gestito è necessario eliminarlo.
Per eliminare il dominio gestito, vedere [Eliminare Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



