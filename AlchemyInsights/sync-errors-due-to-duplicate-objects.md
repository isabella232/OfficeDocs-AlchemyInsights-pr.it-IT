---
title: 902 (errori di sincronizzazione a causa di oggetti duplicati)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757999"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Errori di sincronizzazione a causa di oggetti duplicati

Quando la sincronizzazione della directory viene completata, potrebbe essere visualizzato uno dei seguenti messaggi di errore:

- Impossibile aggiornare l'oggetto nei servizi Microsoft online perché i seguenti attributi associati a questo oggetto dispongono di valori che potrebbero essere già associati a un altro oggetto nella directory locale.

- Un oggetto sincronizzato con lo stesso indirizzo proxy esiste già nella directory dei Microsoft Online Services.

- Non è possibile aggiornare l'oggetto perché i seguenti attributi associati a questo oggetto dispongono di valori che potrebbero essere già associati a un altro oggetto nei servizi directory locali: UserPrincipalName.

Per identificare e risolvere il problema, scaricare ed eseguire lo strumento di correzione degli [errori di IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Per ulteriori informazioni, vedere [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
