---
title: 1554 Errore Winsock 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083234"
---
# <a name="winsock-error-10061"></a>Errore Winsock 10061

Questo codice di errore indica che Microsoft non è riuscito a stabilire un socket TCP (connessione) con l'host di destinazione. La causa più probabile di questo errore è un problema con la configurazione del firewall. Per risolvere il problema, controllare queste impostazioni:

- Verificare la configurazione del firewall con le informazioni negli [URL Microsoft 365 indirizzi IP e negli intervalli di indirizzi IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Se l'errore è specifico di Exchange Online Protection (EOP), in precedenza dovrebbe essere stata notificata una modifica agli [Exchange Online Protection IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verificare che il provider di servizi Internet (ISP) non blocchi la porta.

- Verificare le impostazioni dello smart host e del server di destinazione nei connettori.

Tenere presente Microsoft 365 non blocca le *connessioni* in ingresso in questo modo.
