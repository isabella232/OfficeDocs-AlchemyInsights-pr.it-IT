---
title: Spostare i messaggi di posta elettronica nella cassetta postale di archiviazione
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799784"
---
# <a name="move-email-to-the-archive-mailbox"></a>Spostare la posta elettronica nella cassetta postale di archiviazione

Se si desidera che vengano eseguiti controlli automatici per le impostazioni indicate di seguito, selezionare il pulsante indietro <--nella parte superiore di questa pagina e quindi immettere l'indirizzo di posta elettronica dell'utente che ha problemi a spostare la posta elettronica nella cassetta postale di archiviazione.

1. Verificare che sia stata abilitata una **cassetta postale di archiviazione** . In caso contrario, utilizzare la procedura descritta in [questo articolo](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) per abilitare la cassetta postale di archiviazione.

2. Per archiviare automaticamente i messaggi nella cassetta postale di archiviazione, è necessario impostare un tag di conservazione con l'azione **Sposta nell'archivio** su **applicato automaticamente all'intero tag della cassetta postale (impostazione predefinita)**. Utilizzare la procedura seguente per creare il tag: [archivio predefinito](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)tag.

3. Successivamente, aggiungere il tag di **archiviazione** al criterio di conservazione. Nell'interfaccia di amministrazione di Exchange, scegliere **criteri di conservazione** > aggiungere il **tag Move to Archive** al criterio > **Save**.

4. A questo punto, [assegnare il criterio di conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) alla cassetta postale dell'utente specifico. Lo stesso criterio verrà applicato sia alla cassetta postale **principale** che a quella di **archiviazione** .

Potrebbe essere necessario forzare l'esecuzione dell'Assistente cartelle gestite e applicare le nuove impostazioni alla cassetta postale dell'utente. Eseguire il seguente comando quando [si è connessi a Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) per avviare l'Assistente cartelle gestite per una cassetta postale specifica:
  
Start-ManagedFolderAssistant-Identity <name of the mailbox>

Per ulteriori informazioni sulla configurazione di un criterio di archiviazione, vedere [set up an Archive and Deletion Policy for Mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  