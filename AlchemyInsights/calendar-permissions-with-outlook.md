---
title: Autorizzazioni del calendario
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854008"
---
# <a name="calendar-permissions"></a>Autorizzazioni del calendario

Gli utenti possono modificare le proprie autorizzazioni di calendario con Outlook sul Web o in altri client, ma anche come amministratore potrebbe essere necessario indagare.  
Con il cmdlet di PowerShell di Exchange viene visualizzata l'autorizzazione per il calendario di un utente:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Per ulteriori informazioni, vedere quanto segue:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Le autorizzazioni del calendario vengono utilizzate nella condivisione dei calendari, per visualizzare ulteriori informazioni sulla condivisione di un calendario di Outlook, vedere gli articoli seguenti:

- [Condividere un calendario di Outlook con altri utenti](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Condivisione del calendario in Outlook sul Web per le aziende](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Per risolvere i problemi di autorizzazione del calendario, è possibile utilizzare lo strumento [Assistente supporto e ripristino](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .