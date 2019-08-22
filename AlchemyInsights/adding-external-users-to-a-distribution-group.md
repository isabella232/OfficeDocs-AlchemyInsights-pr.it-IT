---
title: Aggiunta di utenti esterni a un gruppo di distribuzione
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494531"
---
# <a name="add-external-users-to-a-distribution-group"></a>Aggiungere utenti esterni a un gruppo di distribuzione?

L'aggiunta di un contatto esterno a un gruppo di distribuzione (DG) è un processo in due passaggi:
  
1. Creare un contatto di posta per l'utente esterno:
    
    1. Nell'interfaccia di amministrazione, andare alla pagina **** > [contatti](https://admin.microsoft.com/adminportal/home#/Contact) utenti. 
    
    2. Selezionare **Aggiungi un contatto**.
    
    3. Digitare le informazioni per il contatto e selezionare **Aggiungi**.
    
2. Aggiungere il contatto di posta elettronica alla DG:
    
    1. Nell'interfaccia di amministrazione, andare alla **** > [](https://admin.microsoft.com/adminportal/home#/groups) pagina gruppi. 
    
    2. Individuare la DG alla quale si desidera aggiungere l'utente esterno e selezionarla per aprire la finestra di dialogo Modifica.
    
    3. Nella scheda **membri** selezionare **Visualizza tutti i membri e Gestisci**. 
    
    4. Selezionare **Aggiungi membri**.
    
    5. Selezionare il contatto di posta creato nel passaggio precedente e quindi fare clic su **Salva**.
    
Se dopo aver seguito questi passaggi gli utenti esterni non possono inviare messaggi di posta elettronica alla DG o non ricevono messaggi di posta elettronica, potrebbe essere che la DG sia contrassegnata solo per consentire l'invio di messaggi di posta elettronica da parte di utenti interni. È possibile controllare questa configurazione e correggerla seguendo le istruzioni [](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)riportate di seguito.
  
 **Nota:** Queste istruzioni non si applicano se il tipo del gruppo è "Office 365 Group" invece di "gruppo di distribuzione". In caso contrario, è possibile aggiungere l'utente esterno direttamente al gruppo da Outlook. Informazioni dettagliate sui gruppi di Office 365 i clienti e le istruzioni per l'aggiunta di ospiti esterni sono disponibili in [questo articolo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  