---
title: Criteri di conservazione in Exchange'interfaccia di amministrazione non funziona
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074936"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Criteri di conservazione nell'Exchange di amministrazione

Se si desidera eseguire controlli automatizzati per le impostazioni indicate di seguito, selezionare il pulsante Indietro <, nella parte superiore di questa pagina, quindi immettere l'indirizzo di posta elettronica dell'utente che ha problemi con i criteri di conservazione.

Se si verificano problemi con i criteri di conservazione nell'interfaccia di amministrazione di Exchange che non si applicano alle cassette postali o agli elementi che non si spostano nella cassetta postale di archiviazione, controllare quanto segue:

**Cause radice:**

- **L'Assistente cartelle** gestite non ha elaborato la cassetta postale dell'utente. L'Assistente cartelle gestite tenta di elaborare ogni cassetta postale nell'organizzazione basata su cloud una volta ogni sette giorni.

  **Soluzione:** Eseguire l'Assistente cartelle gestite.

- **RetentionHold** è stato **abilitato** nella cassetta postale. Se la cassetta postale è stata impostata su RetentionHold, il criterio di conservazione sulla cassetta postale non verrà elaborato durante tale periodo.

  **Soluzione:** Controllare lo stato dell'impostazione del blocco di conservazione e aggiornare in base alle esigenze. Per informazioni dettagliate, vedere [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Nota:** Se una cassetta postale è inferiore a 10 MB, l'Assistente cartelle gestite non eelaborare automaticamente la cassetta postale.
 
Per altre info sui criteri di conservazione nell'Exchange di amministrazione, vedi:

- [Tag di conservazione e criteri di conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Applicare un criterio di conservazione alle cassette postali](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) o Aggiungere o rimuovere tag di [conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Come identificare il tipo di blocco applicato a una cassetta postale](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
