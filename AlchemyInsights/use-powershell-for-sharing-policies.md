---
title: Usare PowerShell per i criteri di condivisione di criteri e relazioni dell'organizzazione
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 378dedb332ced2c86899401c54726eb6b7e25d08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773419"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Usare PowerShell per i criteri di condivisione di criteri e relazioni dell'organizzazione


Per le relazioni organizzative, consultare la sintassi dettagliata e le informazioni sui parametri per: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) e [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Per creare criteri di condivisione usare [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Per [applicare un criterio di condivisione a una cassetta postale o a un utente](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) è necessario usare una combinazione di [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) e [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) con il criterio appena creato. Per [modificare, disabilitare o rimuovere un criterio di condivisione](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) è necessario usare [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) e [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Per informazioni complete su questo argomento, vedere:**

[Condivisione in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)