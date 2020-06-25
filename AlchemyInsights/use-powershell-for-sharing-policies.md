---
title: Usare PowerShell per i criteri di condivisione di criteri e relazioni dell'organizzazione
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854005"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Usare PowerShell per i criteri di condivisione di criteri e relazioni dell'organizzazione


Per le relazioni organizzative, consultare la sintassi dettagliata e le informazioni sui parametri per: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) e [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Per creare criteri di condivisione usare [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Per [applicare un criterio di condivisione a una cassetta postale o a un utente](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) è necessario usare una combinazione di [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) e [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) con il criterio appena creato. Per [modificare, disabilitare o rimuovere un criterio di condivisione](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) è necessario usare [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) e [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Per informazioni complete su questo argomento, vedere:**

[Condivisione in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)