---
title: Autorizzazioni calendario
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819912"
---
# <a name="calendar-permissions"></a>Autorizzazioni calendario

Gli utenti possono modificare le proprie autorizzazioni di calendario con Outlook sul Web o altri client, ma come amministratore potrebbe essere necessario analizzare anche.  
Con il cmdlet PowerShell di Exchange verrà mostrata l'autorizzazione per il calendario di un utente:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Per ulteriori informazioni, vedere:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Le autorizzazioni del calendario vengono utilizzate nella condivisione dei calendari per visualizzare ulteriori informazioni sulla condivisione di un calendario di Outlook, vedere questi articoli:

- [Condividere un calendario di Outlook con altri utenti](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Condividere il calendario in Outlook sul Web per le aziende](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Per risolvere i problemi relativi all'autorizzazione calendario, è possibile utilizzare [lo strumento Assistente supporto e](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) ripristino.