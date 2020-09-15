---
title: 1554 errore Winsock 10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698866"
---
# <a name="winsock-error-10061"></a>Errore Winsock 10061

Questo codice di errore indica che Microsoft non è stato in grado di stabilire un socket TCP (connessione) con l'host di destinazione. La causa più probabile di questo errore è un problema con la configurazione del firewall. Per risolvere il problema, controllare queste impostazioni:

- Verificare la configurazione del firewall con le informazioni contenute negli [URL e negli intervalli di indirizzi IP di Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Se l'errore è specifico di Exchange Online Protection (EOP), è necessario essere stati precedentemente informati di una modifica apportata agli [indirizzi IP di Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verificare che il provider di servizi Internet (ISP) non blocchi la porta.

- Verificare le impostazioni di smart host e del server di destinazione nei connettori.

Si noti che Microsoft 365 non blocca le connessioni in *ingresso* in questo modo.
