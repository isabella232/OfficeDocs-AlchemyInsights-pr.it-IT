---
title: S/MIME in Outlook sul Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772302"
---
# <a name="encrypt-email-messages-in-outlook"></a>Crittografare i messaggi di posta elettronica in Outlook

La crittografia dei messaggi di Microsoft 365 è basata su Microsoft Azure Rights Management (Azure RMS), che fa parte di Azure Information Protection. Se l'abbonamento include Azure Rights Management o Azure Information Protection, **non è necessario eseguire alcuna azione per attivare o disattivare manualmente** il servizio Rights Management.

In base al feedback dei clienti, non è più possibile abilitare le regole del flusso di posta di Exchange per crittografare automaticamente la posta elettronica in uscita contenente alcuni tipi di informazioni riservate nel tenant per impostazione predefinita. Al contrario, vengono fornite istruzioni dettagliate su come è possibile farlo da soli. Per ulteriori informazioni su come creare una regola di trasporto per crittografare le informazioni riservate, vedere [questo articolo](https://aka.ms/OmeEtr).

- Se si utilizza Outlook sul Web (in precedenza **OWA**): quando si compone un messaggio di posta elettronica, è sufficiente fare clic su **Proteggi** in OWA. Verrà applicata l'autorizzazione "non inoltrare". Fare clic su **Cambia autorizzazione** e scegliere **Crittografa** solo per crittografare il messaggio.

- Se si utilizza il **client di Outlook**: per inviare un messaggio crittografato da Outlook 2013 o 2016 o Outlook 2016 per Mac, selezionare **Opzioni**  >  **autorizzazioni**, quindi selezionare l'opzione di protezione necessaria.

- Per **crittografare automaticamente tutti i messaggi di posta elettronica** inviati a determinati destinatari o organizzazioni partner esterne, è necessario creare una regola di trasporto del flusso di posta nell'interfaccia di amministrazione di Exchange. Istruzioni dettagliate sono disponibili in [questo articolo del supporto tecnico](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

