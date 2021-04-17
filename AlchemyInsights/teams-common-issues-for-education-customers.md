---
title: Problemi comuni di Teams per i clienti del settore dell'istruzione
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
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 6d1fac07673f6f945f382e4e640cf44afb76717d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829452"
---
# <a name="teams-common-issues-for-education-customers"></a>Problemi comuni di Teams per i clienti del settore dell'istruzione

**Per i clienti del settore dell'istruzione**:

Se è necessaria assistenza per la distribuzione di Teams per il supporto dell'apprendimento a distanza, visitare il [FastTrack Center](https://www.microsoft.com/fasttrack) per inviare una richiesta. Leggere i seguenti problemi comuni per i clienti del settore dell'istruzione:

- Gli utenti vedono il messaggio "**Stai perdendo un'occasione!**"? assicurarsi di [Abilitare Microsoft Teams per l'istituto di istruzione](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Nei tenant Education Microsoft Teams non è abilitato per impostazione predefinita. Per prima cosa è necessario attivarlo.

- **Nuovi utenti di Teams?** Consultare [Insegnamento e apprendimento remoto in Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) per le indicazioni più aggiornate su come configurare l'istituto di istruzione, pianificare le lezioni, creare riunioni virtuali e condividere contenuti con gli studenti.

- Dopo l'attivazione, gli utenti possono eseguire Teams installando i client [desktop](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) e [per dispositivi mobili](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) oppure dal browser all'indirizzo https://teams.microsoft.com.

- **Abilitare l'accesso guest a Teams:** esaminare [l'elenco di controllo per l'accesso guest in Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) e verificare che siano stati completati tutti i passaggi.
    - [Informazioni sull'accesso guest in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Configurazione: elenco di controllo per l'accesso guest in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Come un guest partecipa a un team](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Riunioni e chiamate in Teams**: serve aiuto per attivare o configurare Audioconferenza in Microsoft Teams? L'utente è stato creato di recente? In questo caso, sarà necessario attendere 2-24 ore perché le impostazioni abbiano effetto. Per verificare che l'utente disponga della licenza per Audioconferenza e di un numero a pagamento predefinito:
    1. Passare a Utenti attivi e selezionare l'utente in questione.
    2. A seconda della versione dell'interfaccia di amministrazione, scegliere **Licenze e app** o fare clic su **Modifica** in **Licenze dei prodotti**.
    3. Verificare che per l'utente siano selezionate le licenze per Audioconferenza, Microsoft Teams e Skype for Business Online (Piano 2).
    4. In Interfacce di amministrazione fare clic su **Mostra tutto** e poi su **Teams**.
    5. Nell'interfaccia di amministrazione di Microsoft Teams fare clic su **Portale legacy**.
    6. Nell'interfaccia di amministrazione di Skype for Business fare clic su **Audioconferenza** e poi **Utenti**.
    7. Selezionare l'utente in questione e verificare che disponga di un numero a pagamento predefinito.

    Per altre informazioni, vedere [Piani di chiamata Microsoft Teams](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) o chiamare il team Microsoft Commerce Billing per ricevere assistenza con domande relative alla gestione delle licenze.

    Risorse aggiuntive

    - [Riunioni e conferenze in Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Audioconferenza](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Criteri riunione**: i criteri riunione vengono usati per controllare le funzionalità disponibili per i partecipanti alle riunioni programmate dagli utenti nell'organizzazione. Dopo aver creato un criterio e aver apportato le modifiche, è possibile assegnare gli utenti al criterio.

    - **Modificare o creare un criterio riunione**: per modificare o creare un criterio riunione, passare all'**interfaccia di amministrazione di Microsoft Teams > Riunioni > Criteri riunione**. Selezionare un criterio dall'elenco o fare clic su **Aggiungi**. Se si sta creando un nuovo criterio, aggiungere un nome e una descrizione. Il nome non può contenere caratteri speciali o più di 64 caratteri. Scegliere le impostazioni desiderate e poi fare clic su **Salva**. 
    
        Ad esempio, si supponga di avere un gruppo di utenti e di voler limitare la larghezza di banda necessaria per la riunione. È possibile creare un nuovo criterio personalizzato denominato "Larghezza di banda limitata" e disabilitare le impostazioni seguenti:

        In **Audio e video**:
        - Disattivare **Consenti registrazione cloud**.
        - Disattivare **Consenti video IP**.

        In **Condivisione di contenuti**:

        - Disabilitare la modalità di condivisione dello schermo.
        - Disattivare **Consenti la lavagna**.
        - Disattivare **Consenti note condivise**.

        **Assegnare il criterio agli utenti**:

    1. Nel riquadro di spostamento sinistro dell'interfaccia di amministrazione di Microsoft Teams passare a **Utenti**, quindi fare clic sull'utente.
    2. Selezionare l'utente facendo clic a sinistra del nome utente e poi fare clic su **Modifica impostazioni**.
    3. In **Criteri riunione** selezionare il criterio da assegnare e poi fare clic su **Applica**.

    Per assegnare un criterio a più utenti alla volta, vedere [Modificare le impostazioni utente di Teams in blocco](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    In alternativa è possibile eseguire le operazioni seguenti:
    1. Nel riquadro di spostamento sinistro dell'interfaccia di amministrazione di Microsoft Teams passare a **Riunioni > Criteri riunioni**.
    2. Selezionare il criterio facendo clic a sinistra del nome del criterio.
    3. Fare clic su **Gestisci utenti**.
    4. Nel riquadro **Gestisci utenti**, cercare l'utente per nome visualizzato o in base al nome utente, selezionare il nome e poi fare clic su **Aggiungi**. Ripetere questa operazione per ogni utente da aggiungere.
    5. Dopo avere aggiunto gli utenti, fare clic su **Salva**.

- **Risolvere i problemi di assenza della tastiera del telefono**:
    - Verificare che all'utente sia stata assegnata una [licenza di Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Assicurarsi che all'utente sia stato assegnato un [piano di chiamata](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Abilitare gli utenti per [VoIP aziendale](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Risolvere i problemi di accesso a Teams:** prima di tutto, verificare l'[integrità del servizio Microsoft Teams](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Controllare quindi se sono presenti codici di errore comuni e consultare nuovamente [Perché non riesco ad accedere a Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Può anche essere necessario consultare nuovamente [Modelli di identità e autenticazione in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
