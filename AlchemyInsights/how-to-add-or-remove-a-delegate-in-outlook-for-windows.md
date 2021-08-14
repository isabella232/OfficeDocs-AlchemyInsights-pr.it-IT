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
ms.openlocfilehash: ee54e2bcca4f4591b33ee805290192311f6cde09a9e453a813e9db328d19634d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945341"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Come aggiungere o rimuovere un delegato in Outlook per Windows

Per aggiungere un delegato in Outlook per Windows: 

1. Fare clic sulla **scheda File** seguita da **Account Impostazioni** e quindi scegliere Accesso **delegato**.
2. Fare clic su **Aggiungi**. Se **add** non viene visualizzato, è possibile che non esista una connessione attiva tra Outlook e Exchange. Nella Outlook di stato viene visualizzato lo stato della connessione.
3. Digitare il nome della persona che si desidera designare come delegato oppure cercare e scegliere il nome nell'elenco dei risultati della ricerca.

    > [!NOTE]
    > Il delegato deve essere una persona nell'elenco indirizzi globale Exchange globale (GAL) dell'organizzazione.
4. Fare clic **su Aggiungi** seguito da **OK.**
5. Nella finestra **di dialogo Autorizzazioni** delegato accettare le impostazioni di autorizzazione predefinite o selezionare livelli di accesso personalizzati per Exchange cartelle.

    - Se un delegato necessita dell'autorizzazione per funzionare solo con le convocazioni di riunione e le risposte, le impostazioni di autorizzazione predefinite, ad esempio Delegato, ricevono copie dei messaggi relativi alla riunione inviati a **me** sono sufficienti. È possibile lasciare **l'impostazione dell'autorizzazione** Posta in arrivo **su Nessuno.** Le convocazioni di riunione e le risposte verranno inviate direttamente alla posta in arrivo del delegato.

    > [!NOTE]
    > Per impostazione predefinita, al delegato viene concessa l'autorizzazione **Editor (può leggere, creare e** modificare elementi) per la cartella **Calendario.** Quando il delegato risponde a una riunione per conto dell'utente, viene aggiunto automaticamente alla **cartella** Calendario.

5. Per inviare un messaggio per notificare al delegato le autorizzazioni modificate, selezionare la casella di controllo Invia automaticamente un messaggio per delegare **il riepilogo di** queste autorizzazioni.
6. Se si desidera, selezionare la **casella di controllo Delegate can see my private items.**

    > [!IMPORTANT]
    > Questa impostazione influisce su Exchange cartelle. Sono incluse tutte le cartelle Posta, Contatti, Calendario, Attività, Note e Diario. Non è possibile concedere l'accesso agli elementi privati solo nelle cartelle specificate.

7. Scegliere **OK**.

    > [!NOTE]
    >
    > - I messaggi inviati con autorizzazioni Invia per conto di includono sia il delegato che i nomi accanto a **Da**. Quando viene inviato un messaggio con autorizzazioni Invia come, viene visualizzato solo il nome dell'utente.
    > - Dopo aver aggiunto un utente come delegato, può aggiungere la cassetta Exchange cassetta postale al profilo Outlook utente. Per istruzioni, vedere [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Per rimuovere un delegato in Outlook per Windows:

1. Fare clic sulla **scheda File.**
2. Fare clic **su Account Impostazioni** seguito da Accesso **delegato**.
3. Scegliere il nome del delegato per cui si desidera modificare le autorizzazioni, quindi fare clic su **Rimuovi** seguito da **OK.**
