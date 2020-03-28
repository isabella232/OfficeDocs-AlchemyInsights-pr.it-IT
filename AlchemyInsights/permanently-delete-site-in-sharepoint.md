---
title: Eliminare definitivamente un sito in SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955166"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Eliminare definitivamente un sito in SharePoint

Per riutilizzare un URL di un sito eliminato (per ricreare un sito) oppure per eliminare definitivamente un sito perché non è più in uso, è possibile usare **Elimina definitivamente** dalla nuova interfaccia di amministrazione di SharePoint. 

1. Passare alla [pagina Siti eliminati della nuova interfaccia di amministrazione di SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) e accedere con un account dotato di autorizzazioni di amministratore per l'organizzazione. 

2. Nella colonna sinistra selezionare un sito. 

3. Fare clic su **Elimina definitivamente**. 

**Nota**: i siti connessi a un gruppo non possono essere eliminati definitivamente dalla nuova interfaccia di amministrazione di SharePoint. È necessario usare il cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).  

Per ulteriori informazioni, vedere [Eliminare definitivamente un sito](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
