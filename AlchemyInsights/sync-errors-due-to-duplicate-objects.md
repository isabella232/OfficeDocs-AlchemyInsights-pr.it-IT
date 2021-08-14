---
title: 902 (Errori di sincronizzazione dovuti a oggetti duplicati)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998798"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Errori di sincronizzazione dovuti a oggetti duplicati

È possibile che venga visualizzato uno dei seguenti messaggi di errore al termine della sincronizzazione della directory Microsoft 365:

- Impossibile aggiornare questo oggetto in Microsoft Online Services perché gli attributi seguenti associati all'oggetto hanno valori che potrebbero essere già associati a un altro oggetto nella directory locale.

- Un oggetto sincronizzato con lo stesso indirizzo proxy esiste già nella directory Microsoft Online Services directory.

- Impossibile aggiornare questo oggetto perché gli attributi seguenti associati all'oggetto hanno valori che potrebbero essere già associati a un altro oggetto nei servizi directory locali: UserPrincipalName.

Per identificare e risolvere il problema, scaricare ed eseguire lo [strumento idFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).

Per ulteriori informazioni, vedere [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
