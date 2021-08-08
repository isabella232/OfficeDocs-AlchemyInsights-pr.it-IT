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
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934837"
---
# <a name="add-external-users-to-a-distribution-group"></a>Aggiungere utenti esterni a un gruppo di distribuzione

L'aggiunta di un contatto esterno a un gruppo di distribuzione è un processo in due passaggi:
  
1. Creare un contatto di posta per l'utente esterno:
    
    1. Nell'interfaccia di amministrazione passare alla **pagina Contatti**  >  [](https://admin.microsoft.com/adminportal/home#/Contact) utenti. 
    
    2. Selezionare **Aggiungi un contatto**.
    
    3. Digitare le informazioni per il contatto e selezionare **Aggiungi**.
    
2. Aggiungere il contatto di posta al DG:
    
    1. Nell'interfaccia di amministrazione passare alla **pagina**  >  [Gruppi di](https://admin.microsoft.com/adminportal/home#/groups) gruppi. 
    
    2. Individuare il DG a cui si desidera aggiungere l'utente esterno e selezionarlo per aprire la finestra di dialogo di modifica.
    
    3. Nella scheda **Membri** selezionare Visualizza **tutti e gestisci membri**. 
    
    4. Selezionare **Aggiungi membri**.
    
    5. Selezionare il contatto di posta creato nel passaggio precedente e quindi selezionare **Salva**.
    
Se dopo aver seguito questi passaggi gli utenti esterni non possono inviare messaggi di posta elettronica alla DG o non riceverlo, è possibile che la DG sia contrassegnata per consentire solo i messaggi di posta elettronica provenienti da utenti interni. Puoi controllare questa configurazione e correggerla seguendo le istruzioni [qui](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Nota:** Queste istruzioni non si applicano se il tipo del gruppo è "Microsoft 365 gruppo" anziché "Gruppo di distribuzione". In questo caso, è possibile aggiungere l'utente esterno direttamente al gruppo da Outlook. In questo articolo sono disponibili informazioni dettagliate Microsoft 365 utenti guest e istruzioni per l'aggiunta di guest [esterni.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  