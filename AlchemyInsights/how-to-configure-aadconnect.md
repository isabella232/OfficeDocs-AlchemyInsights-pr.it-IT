---
title: 646 Come configurare AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963647"
---
# <a name="configure-sync-features"></a>Configurare le funzionalità di sincronizzazione

Azure AD Connessione include diverse funzionalità abilitate per impostazione predefinita o che è possibile abilitare in un secondo momento. Alcune funzionalità richiedono una configurazione aggiuntiva in ambienti specifici.

- [I](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limiti di filtro vengono sincronizzati con Azure AD. Per impostazione predefinita, tutti gli utenti, i contatti, i gruppi e Windows 10 account computer vengono sincronizzati. È possibile includere o escludere oggetti in base a domini, unità organizzative o altri attributi.

- [La sincronizzazione dell'hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) delle password sincronizza l'hash delle password da Active Directory locale ad Azure AD. Ciò consente la gestione delle password in un'unica posizione, ma l'uso della stessa password sia in ambienti locali che in ambienti cloud. Poiché Active Directory è l'origine autorevole, è possibile utilizzare criteri password personalizzati.

- [La reimpostazione della password self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) consente agli utenti di reimpostare le proprie password nel cloud applicando comunque i criteri password locali.

- [Il writeback dei dispositivi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) consente ai dispositivi registrati in Azure AD di essere scritti in Active Directory locale in modo che possano essere usati per l'accesso condizionale.

- [Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). È possibile modificare questa impostazione per soddisfare le esigenze dell'organizzazione.

- [L'aggiornamento](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) automatico è abilitato per impostazione predefinita per le installazioni rapide e garantisce che la versione di Azure AD Connessione sia sempre aggiornata.
