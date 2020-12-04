---
title: Informazioni su come aggiungere o rimuovere un delegato in Outlook per Windows
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
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571913"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Informazioni su come aggiungere o rimuovere un delegato in Outlook per Windows

Per aggiungere un delegato in Outlook per Windows: 

1. Fare clic sulla scheda **file** seguita dalle **impostazioni dell'account**, quindi selezionare **Delega accesso**.
2. Fare clic su **Aggiungi**. Se **Add** non viene visualizzato, una connessione attiva potrebbe non esistere tra Outlook ed Exchange. La barra di stato di Outlook Visualizza lo stato della connessione.
3. Digitare il nome della persona che si desidera designare come delegato oppure cercare e scegliere il nome nell'elenco dei risultati della ricerca.

    > [!NOTE]
    > Il delegato deve essere una persona nell'elenco indirizzi globale (GAL, Global Address List) dell'organizzazione.
4. Fare clic su **Aggiungi** seguito da **OK**.
5. Nella finestra di dialogo **autorizzazioni delegati** accettare le impostazioni predefinite per le autorizzazioni o selezionare livelli di accesso personalizzati per le cartelle di Exchange.

    - Se un delegato deve disporre dell'autorizzazione necessaria per funzionare solo con le richieste di riunione e le risposte, le impostazioni di autorizzazione predefinite come **delegate ricevono le copie dei messaggi relativi a riunioni inviate a me** sono sufficienti. È possibile lasciare l'impostazione di autorizzazione **posta in arrivo** in **Nessuna**. Le convocazioni di riunione e le risposte andranno direttamente alla posta in arrivo del delegato.

    > [!NOTE]
    > Per impostazione predefinita, al delegato viene concessa l'autorizzazione **Editor (in grado di leggere, creare e modificare elementi)** per la cartella **Calendario** . Quando il delegato risponde a una riunione per conto dell'utente, viene aggiunta automaticamente alla cartella **Calendario** .

5. Per inviare un messaggio per notificare al delegato le autorizzazioni modificate, selezionare la casella di controllo **Invia automaticamente un messaggio per delegare il riepilogo di queste autorizzazioni** .
6. Se lo si desidera, selezionare la casella di controllo il **delegato può visualizzare gli elementi** personali.

    > [!IMPORTANT]
    > Questa impostazione ha effetto su tutte le cartelle di Exchange. Sono inclusi tutti i messaggi, i contatti, il calendario, le attività, le note e le cartelle del journal. Non esiste alcun modo per concedere l'accesso agli elementi privati solo nelle cartelle specificate.

7. Scegliere **OK**.

    > [!NOTE]
    >
    > - I messaggi inviati con le autorizzazioni Invia per conto di sono sia i delegati sia i nomi accanto a **from**. Quando un messaggio viene inviato con l'autorizzazione Invia come, viene visualizzato solo il nome.
    > - Dopo aver aggiunto un utente come delegato, è possibile aggiungere la cassetta postale di Exchange al proprio profilo di Outlook. Per istruzioni, vedere [gestire i messaggi di posta elettronica e gli elementi del calendario di un'altra persona](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Per rimuovere un delegato in Outlook per Windows:

1. Fare clic sulla scheda **file** .
2. Fare clic su **Impostazioni account** seguite da **accesso delegato**.
3. Scegliere il nome del delegato per il quale si desidera modificare le autorizzazioni e quindi fare clic su **Rimuovi** seguito da **OK**.
