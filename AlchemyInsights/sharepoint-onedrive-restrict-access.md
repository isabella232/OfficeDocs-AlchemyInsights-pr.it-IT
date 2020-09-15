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
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700459"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Limitare l'accesso in SharePoint o OneDrive

Esistono diversi modi per limitare l'accesso ai servizi di SharePoint Online/OneDrive. Di seguito sono descritti i diversi metodi di restrizione di accesso. 

**Limitazione delle autorizzazioni**

In SharePoint Online e OneDrive for business, è possibile limitare l'accesso a elementi come siti, file e cartelle concedendo l'accesso solo ai gruppi/utenti che devono avere accesso.

- [Personalizzare le autorizzazioni per un elenco o una raccolta di SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalizzare le autorizzazioni del sito di SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Modificare le autorizzazioni in una sottocartella](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controllare l'accesso da dispositivi non gestiti](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Come amministratore globale o di SharePoint, è possibile bloccare o limitare l'accesso a SharePoint e il contenuto di OneDrive da dispositivi non gestiti (quelli non ibridi AD Uniti o conformi a Intune).

**Limitazione del percorso di rete**

In qualità di amministratore IT, è possibile controllare l'accesso alle risorse di SharePoint e OneDrive in base a percorsi di rete definiti attendibili. In questo caso si parla di criteri basati sulla posizione. Per ulteriori informazioni, vedere [controllare l'accesso ai dati di SharePoint Online e OneDrive in base al percorso di rete](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Limitazione del blocco del sito** 

In SharePoint Online è possibile bloccare una raccolta siti, in modo che nessuno abbia accesso. Questa impostazione viene impostata tramite PowerShell e [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) tramite la proprietà [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Impedire agli utenti di creare siti o sottositi**

Come amministratore globale o amministratore di SharePoint, è possibile consentire agli utenti di creare e amministrare i propri siti di SharePoint, determinare il tipo di siti che possono creare e specificare il percorso dei siti. Per ulteriori informazioni, vedere [gestire la creazione di siti in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

