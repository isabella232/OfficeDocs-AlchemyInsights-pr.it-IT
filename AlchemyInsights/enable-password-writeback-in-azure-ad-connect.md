---
title: Abilitare il writeback delle password in Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709731"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Abilitare il writeback delle password in Azure AD Connect

Per abilitare il writeback della reimpostazione della password in modalità self-service, abilitare prima l'opzione writeback in Azure AD Connect. Nel server Azure AD Connect eseguire i passaggi seguenti:

1. Accedere al server Azure AD Connect e avviare la configurazione guidata di **Azure AD Connect**.
2. Nella pagina di **benvenuto** fare clic su **Configura**.
3. Nella pagina **Attività aggiuntive** selezionare **Personalizza le opzioni di sincronizzazione**, quindi fare clic su **Avanti**.
4. Nella pagina **Connessione ad Azure AD**, immettere le credenziali dell'amministratore globale per il tenant Azure e fare clic su Avanti.
5. Nelle pagine **Connessione delle directory** e **Filtro di domini/unità organizzative**, fare clic su **Avanti**.
6. Nella pagina **Funzionalità facoltative** selezionare la casella accanto a **Writeback password** e fare clic su **Avanti**.
7. Nella pagina **Pronto per la configurazione**, fare clic su **Configura** e attendere il completamento del processo.
8. Quando viene visualizzata la fine della configurazione, fare clic su **Esci**.

Dopo l’abilitazione dell’opzione writeback delle password in Azure AD Connect, ora è possibile configurare Azure AD SSPR per il writeback.  Per abilitare il writeback delle password in reimpostazione della password self-service, eseguire la procedura seguente:

1. Accedere al portale di Azure con un account di amministratore globale.
2. Cercare e selezionare **Azure Active Directory**, fare clic su **Reimpostazione della password** e quindi scegliere **Integrazione locale**.
3. Impostare l’opzione per **Vuoi eseguire il writeback delle password nella directory locale?** su **Sì**.
4. Impostare l’opzione per **Vuoi consentire agli utenti di sbloccare gli account senza reimpostare la password?** su ** Sì**.
5. Al termine fare clic su **Salva**.

Per altre informazioni, vedere [Abilitare il writeback della reimpostazione della password in modalità self-service di Azure Active Directory in un ambiente locale](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).
