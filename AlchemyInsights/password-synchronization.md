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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449141"
---
# <a name="password-synchronization"></a>Sincronizzazione delle password

**La sincronizzazione dell'hash delle password non funziona affatto**

Alcuni problemi comuni riscontrati dai clienti quando la sincronizzazione hash delle password non funziona sono:

- All'account di Active Directory usato da Azure AD Connect per  comunicare con Active Directory locale non vengono concesse le autorizzazioni Replica modifiche directory e Replica modifiche **directory tutte,** necessarie per la sincronizzazione delle password. È necessario risolvere il problema concedendo queste autorizzazioni all'account di Active Directory.
- La sincronizzazione dell'hash delle password viene disabilitata dopo che un amministratore ha modificato il metodo user Sign-In da **Sincronizzazione** password a un'altra opzione, ad esempio Federazione con **AD FS** nella procedura guidata di Azure AD Connect. È possibile risolvere il problema ri abilitando la funzionalità di sincronizzazione **dell'hash** delle password nella procedura guidata di Azure AD Connect.
- Problema di connettività con Active Directory locale. Ad esempio, alcuni controller di dominio non sono [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) accessibili da Azure AD Connect o le porte richieste sono bloccate da Firewall. È necessario risolvere il problema assicurando che la connettività tra il server Azure AD Connect e Active Directory locale funzioni correttamente.
- Il server Azure AD Connect è attualmente in modalità di gestione temporanea, il che fa in modo che il server non sia in grado di eseguire gli hash delle password. Per risolvere il problema, seguire la procedura descritta nella sezione Risolvere i problemi di sincronizzazione delle password con la sincronizzazione di [Azure AD Connect -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Nessuna password sincronizzata.

**La sincronizzazione dell'hash delle password non funziona per alcuni utenti**

1. Se hai notato che l'hash delle password  non è sincronizzato per un utente, usa l'attività di risoluzione dei problemi in Azure AD Connect per analizzare e risolvere il problema. Eseguire le attività seguenti:

    a. [Eseguire l'attività di risoluzione dei problemi nella procedura guidata](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Utilizzare il cmdlet per la risoluzione dei problemi per analizzare il problema di sincronizzazione dell'hash delle password per un utilizzo specifico](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. L'oggetto utente di Active Directory locale è abilitato per l'opzione Cambiamento password **all'accesso** successivo. Quando questa opzione è abilitata, all'utente viene assegnata una password temporanea e verrà richiesto di modificarla al successivo accesso. Azure AD Connect non sincronizza le password temporanee con Azure AD.

Per risolvere il problema precedente, eseguire una delle attività seguenti:

- Chiedere all'utente di accedere all'applicazione locale (ad esempio, Windows Desktop) e modificare la password. La nuova password verrà sincronizzata con Azure AD.
- Richiedere a un amministratore di aggiornare la password dell'utente senza abilitare l'opzione Modifica **password** all'accesso successivo e condivisione della nuova password con l'utente.

3. L'oggetto utente di Active Directory locale non è configurato **correttamente** per la sincronizzazione degli oggetti o la sincronizzazione delle password. Per risolvere questo problema, seguire i passaggi descritti in Risoluzione dei problemi di sincronizzazione hash delle password con la sincronizzazione [di Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







