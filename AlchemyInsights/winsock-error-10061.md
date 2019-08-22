---
title: 1554 errore Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f54c7fc81c274871fbc22908ce0fb21500975d9e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530800"
---
# <a name="winsock-error-10061"></a>Errore Winsock 10061

Questo codice di errore indica che Office 365 non è stato in grado di stabilire un socket TCP (connessione) con l'host di destinazione. La causa più probabile di questo errore è un problema con la configurazione del firewall. Per risolvere il problema, controllare queste impostazioni:

- Verificare la configurazione del firewall con le informazioni negli [intervalli di indirizzi IP e URL di Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Se l'errore è specifico di Exchange Online Protection (EOP), è necessario essere stati precedentemente informati di una modifica apportata agli [indirizzi IP di Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verificare che il provider di servizi Internet (ISP) non blocchi la porta.

- Verificare le impostazioni di smart host e del server di destinazione nei connettori.

Si noti che Office 365 non blocca le connessioni in *ingresso* in questo modo.
