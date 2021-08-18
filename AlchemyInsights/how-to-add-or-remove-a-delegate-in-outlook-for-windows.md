---
title: Come aggiungere o rimuovere un delegato in Outlook per Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: 8db800d5c23b4cc2057f94abaf357082914143d3
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329029"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Come aggiungere o rimuovere un delegato in Outlook per Windows

Per aggiungere un delegato in Outlook per Windows: 

1. Fare clic sulla **scheda File** seguita da **Account Impostazioni** e quindi scegliere Accesso **delegato**.
2. Fare clic su **Aggiungi**. Se **add** non viene visualizzato, potrebbe non esistere una connessione attiva tra Outlook e Exchange. Nella Outlook di stato viene visualizzato lo stato della connessione.
3. Digitare il nome della persona che si desidera designare come delegato oppure cercare e scegliere il nome nell'elenco dei risultati della ricerca.

    **Nota:** il delegato deve essere una persona nell'elenco indirizzi Exchange globale (GAL) dell'organizzazione.
4. Fare clic **su Aggiungi** seguito da **OK.**
5. Nella finestra **di dialogo Autorizzazioni** delegato accettare le impostazioni di autorizzazione predefinite o selezionare livelli di accesso personalizzati per Exchange cartelle.

    - Se un delegato necessita dell'autorizzazione per funzionare solo con le convocazioni di riunione e le risposte, le impostazioni di autorizzazione predefinite, ad esempio Delegato, ricevono copie dei messaggi relativi alle riunioni inviati a **me** sono sufficienti. È possibile lasciare **l'impostazione dell'autorizzazione** Posta in arrivo **su Nessuno.** Le convocazioni di riunione e le risposte verranno inviate direttamente alla posta in arrivo del delegato.

    **Nota:** per impostazione predefinita, al delegato viene concessa l'autorizzazione **Editor (può leggere, creare e** modificare elementi) per la cartella **Calendario.** Quando il delegato risponde a una riunione per conto dell'utente, viene aggiunto automaticamente alla **cartella** Calendario.

5. Per inviare un messaggio per notificare al delegato le autorizzazioni modificate, selezionare la casella di controllo Invia automaticamente un messaggio per delegare **il riepilogo di** queste autorizzazioni.
6. Se si desidera, selezionare la **casella di controllo Delegate can see my private items.**

    **Importante:** questa impostazione influisce su Exchange cartelle. Sono incluse tutte le cartelle Posta, Contatti, Calendario, Attività, Note e Diario. Non è possibile concedere l'accesso agli elementi privati solo nelle cartelle specificate.

7. Scegliere **OK**.

    **Nota**:
    - I messaggi inviati con autorizzazioni Invia per conto di includono sia il delegato che i nomi accanto a **Da**. Quando viene inviato un messaggio con autorizzazioni Invia come, viene visualizzato solo il nome dell'utente.
    - Dopo aver aggiunto un utente come delegato, può aggiungere la cassetta Exchange cassetta postale al profilo Outlook utente. Per istruzioni, vedere [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Per rimuovere un delegato in Outlook per Windows:

1. Fare clic sulla **scheda File.**
2. Fare clic **su Account Impostazioni** seguito da Accesso **delegato**.
3. Scegliere il nome del delegato per il quale si desidera modificare le autorizzazioni, quindi fare clic su **Rimuovi** seguito da **OK.**
