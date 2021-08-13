---
title: Sincronizzazione delle password
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960839"
---
# <a name="password-synchronization"></a>Sincronizzazione delle password

**Sincronizzazione hash password non funziona affatto**

Alcuni problemi comuni riscontrati dai clienti quando la sincronizzazione hash delle password non funziona sono:

- All'account di Active Directory utilizzato da Azure AD Connessione per comunicare con Active Directory locale non vengono concesse le autorizzazioni Replica modifiche **directory** e Replica modifiche directory **Tutte** le autorizzazioni, necessarie per la sincronizzazione delle password, è necessario risolvere il problema concedendo queste autorizzazioni all'account di Active Directory.
- La sincronizzazione dell'hash delle password viene disabilitata dopo che un amministratore ha modificato il metodo User Sign-In da **Sincronizzazione** password a un'altra opzione, ad esempio Federazione con **AD FS** nella procedura guidata di Azure AD Connessione- È possibile risolvere il problema ri abilitando di nuovo la funzionalità di sincronizzazione **dell'hash** delle password nella procedura guidata di Azure AD Connessione.
- Problema di connettività con Active Directory locale. Ad esempio, alcuni controller di dominio non sono accessibili [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) da Azure AD Connessione o le porte necessarie sono bloccate da Firewall: è necessario risolvere il problema assicurando che la connettività tra il server di Connessione di Azure AD e Active Directory locale funzioni correttamente.
- Server di azure AD Connessione attualmente in modalità di gestione temporanea, che farà in modo che il server non sia in grado di eseguire gli hash delle password- Per risolvere il problema, seguire i passaggi descritti nella sezione Risolvere i problemi di sincronizzazione delle password con la sincronizzazione di [Azure AD Connessione -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Nessuna password sincronizzata .

**Password Hash Synchronization does not work for some of my users**

1. Se hai notato che l'hash delle password  non è sincronizzato per un utente, usa l'attività di risoluzione dei problemi nel Connessione Azure AD per analizzare e risolvere il problema. Eseguire le attività seguenti:

    a. [Eseguire l'attività di risoluzione dei problemi nella procedura guidata](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Utilizzare il cmdlet per la risoluzione dei problemi per analizzare il problema di sincronizzazione dell'hash delle password per un utilizzo specifico](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. L'oggetto utente di Active Directory locale è abilitato per **l'opzione L'utente deve cambiare password all'accesso** successivo. Quando questa opzione è abilitata, all'utente viene assegnata una password temporanea e verrà richiesto di modificare la password all'accesso successivo. Azure AD Connessione non sincronizza le password temporanee con Azure AD.

Per risolvere il problema precedente, eseguire una delle attività seguenti:

- Chiedere all'utente di accedere all'applicazione locale (ad esempio, Windows Desktop) e modificare la password. La nuova password verrà sincronizzata con Azure AD.
- Richiedere a un amministratore di aggiornare la password dell'utente senza abilitare l'opzione L'utente deve cambiare **password** all'accesso successivo e condividere la nuova password con l'utente.

3. L'oggetto utente di Active Directory locale non è configurato **correttamente** per la sincronizzazione degli oggetti o la sincronizzazione delle password. Per risolvere questo problema, seguire i passaggi descritti in Risolvere i problemi di sincronizzazione [dell'hash](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)delle password con Azure AD Connessione sincronizzazione .







