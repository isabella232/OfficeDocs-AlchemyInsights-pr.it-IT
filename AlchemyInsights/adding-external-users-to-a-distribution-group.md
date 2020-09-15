---
title: Aggiunta di utenti esterni a un gruppo di distribuzione
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663517"
---
# <a name="add-external-users-to-a-distribution-group"></a>Aggiungere utenti esterni a un gruppo di distribuzione

L'aggiunta di un contatto esterno a un gruppo di distribuzione (DG) è un processo in due fasi:
  
1. Creare un contatto di posta per l'utente esterno:
    
    1. Nell'interfaccia di amministrazione, andare alla pagina **Users**  >  [contatti](https://admin.microsoft.com/adminportal/home#/Contact) utenti. 
    
    2. Selezionare **Aggiungi un contatto**.
    
    3. Digitare le informazioni per il contatto e selezionare **Aggiungi**.
    
2. Aggiungere il contatto di posta elettronica alla DG:
    
    1. Nell'interfaccia di amministrazione, andare alla pagina **gruppi**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Individuare la DG alla quale si desidera aggiungere l'utente esterno e selezionarla per aprire la finestra di dialogo Modifica.
    
    3. Nella scheda **membri** selezionare **Visualizza tutti i membri e Gestisci**. 
    
    4. Selezionare **Aggiungi membri**.
    
    5. Selezionare il contatto di posta creato nel passaggio precedente e quindi fare clic su **Salva**.
    
Se dopo aver seguito questi passaggi gli utenti esterni non possono inviare messaggi di posta elettronica alla DG o non ricevono messaggi di posta elettronica, potrebbe essere che la DG sia contrassegnata solo per consentire l'invio di messaggi di posta elettronica da parte di utenti interni. È possibile controllare questa configurazione e correggerla seguendo le istruzioni riportate [di seguito.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Nota:** Queste istruzioni non si applicano se il tipo del gruppo è "Microsoft 365 Group" invece di "gruppo di distribuzione". In caso contrario, è possibile aggiungere l'utente esterno direttamente al gruppo da Outlook. In [questo articolo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)sono disponibili informazioni dettagliate sui gruppi di Microsoft 365, nonché sulle istruzioni per l'aggiunta di ospiti esterni.
  