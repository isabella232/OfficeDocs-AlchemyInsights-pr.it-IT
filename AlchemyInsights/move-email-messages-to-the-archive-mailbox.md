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
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974961"
---
# <a name="move-email-to-the-archive-mailbox"></a>Spostare la posta elettronica nella cassetta postale di archiviazione

Se si desidera che eserciti controlli automatizzati per le impostazioni indicate di seguito, selezionare il pulsante Indietro <-- nella parte superiore di questa pagina, quindi immettere l'indirizzo di posta elettronica dell'utente che ha problemi a spostare la posta elettronica nella cassetta postale di archiviazione.

1. Verificare che sia **stata abilitata una** cassetta postale di archiviazione. In caso contrario, eseguire la procedura descritta in [questo articolo](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) per abilitare la cassetta postale di archiviazione.

2. Per archiviare automaticamente i messaggi nella  cassetta postale di archiviazione, è necessario impostare un tag di conservazione con l'azione Sposta nell'archivio su applicato automaticamente all'intera **cassetta postale (impostazione predefinita).** Seguire la procedura qui descritta per creare il tag: [Archivia tag predefinito.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Aggiungi quindi il tag **Archive** ai criteri di conservazione. Nell'Exchange di amministrazione scegliere Criteri di **conservazione** > aggiungere il **tag** Sposta nell'archivio al criterio > **Salva**.

4. Assegnare [ora i criteri di conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) alla cassetta postale dell'utente specifico. Lo stesso criterio verrà applicato sia alla cassetta **postale principale** che alla cassetta **postale di** archiviazione.

Potrebbe essere necessario forzare l'esecuzione dell'Assistente cartelle gestite (MFA) e applicare le nuove impostazioni alla cassetta postale dell'utente. Eseguire il comando seguente mentre si è connessi a [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) per avviare l'Assistente cartelle gestite per una cassetta postale specifica:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Per ulteriori informazioni sulla configurazione di un criterio di archiviazione, vedere [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  