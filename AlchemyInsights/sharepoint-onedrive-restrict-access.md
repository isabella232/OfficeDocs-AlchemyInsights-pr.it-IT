---
title: Limitare l'accesso in SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093836"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Limitare l'accesso in SharePoint o OneDrive

Esistono molti modi per limitare l'accesso SharePoint online/OneDrive servizi. Questi diversi metodi di restrizione di accesso sono descritti di seguito. 

**Restrizione delle autorizzazioni**

In SharePoint Online e OneDrive for Business, si limita l'accesso a elementi come siti, file e cartelle concedendo l'accesso solo a quei gruppi/utenti che dovrebbero avere accesso.

- [Personalizzare le autorizzazioni per un SharePoint o una raccolta](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalizzare le autorizzazioni del sito di SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Modificare le autorizzazioni in una sottocartella](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controllare l'accesso da dispositivi non gestiti](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

In quanto SharePoint o amministratore globale, puoi bloccare o limitare l'accesso al contenuto di SharePoint e OneDrive da dispositivi non gestiti (non aggiunti ad Active Directory ibridi o conformi in Intune).

**Restrizione percorso di rete**

Gli amministratori IT possono controllare l'accesso alle risorse SharePoint e OneDrive in base a percorsi di rete definiti attendibili. In questo caso si parla di criteri basati sulla posizione. Per ulteriori informazioni, vedere [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restrizione di blocco del sito** 

In SharePoint Online è possibile bloccare una raccolta siti, in modo che nessuno abbia accesso. Questa impostazione viene impostata tramite PowerShell [e SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) tramite la proprietà [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Impedire agli utenti di creare siti o siti secondari**

In quanto amministratore SharePoint o amministratore globale, puoi consentire agli utenti di creare e amministrare i propri siti SharePoint, determinare il tipo di siti che possono creare e specificare il percorso dei siti. Per ulteriori informazioni, vedere [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

