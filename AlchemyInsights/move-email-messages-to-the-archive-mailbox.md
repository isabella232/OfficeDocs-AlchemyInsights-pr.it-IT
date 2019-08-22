---
title: Spostare i messaggi di posta elettronica nella cassetta postale di archiviazione
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36549007"
---
# <a name="move-email-to-the-archive-mailbox"></a>Spostare la posta elettronica nella cassetta postale di archiviazione

1. Verificare che sia stata abilitata una **cassetta postale di archiviazione** . In caso contrario, utilizzare la procedura descritta in [questo articolo](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) per abilitare la cassetta postale di archiviazione.

2. Per archiviare automaticamente i messaggi nella cassetta postale di archiviazione, è necessario impostare un tag di conservazione con l'azione **Sposta nell'archivio** su **applicato automaticamente all'intero tag della cassetta postale (impostazione predefinita)**. Utilizzare la procedura seguente per creare il tag: [archivio predefinito](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)tag.

3. Successivamente, aggiungere il tag di **archiviazione** al criterio di conservazione. Nell'interfaccia di amministrazione di Exchange, scegliere **criteri di conservazione** > aggiungere il **tag Move to Archive** al criterio > **Save**.

4. A questo punto, [assegnare il criterio di conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) alla cassetta postale dell'utente specifico. Lo stesso criterio verrà applicato sia alla cassetta postale **principale** che a quella di **archiviazione** .

Potrebbe essere necessario forzare l'esecuzione dell'Assistente cartelle gestite e applicare le nuove impostazioni alla cassetta postale dell'utente. Eseguire il seguente comando quando [si è connessi a Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) per avviare l'Assistente cartelle gestite per una cassetta postale specifica:
  
Start-ManagedFolderAssistant-Identity<name of the mailbox>

Per ulteriori informazioni sulla configurazione di un criterio di archiviazione, vedere [set up an Archive and Deletion Policy for Mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  