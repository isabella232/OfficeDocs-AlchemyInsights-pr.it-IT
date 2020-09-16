---
title: 902 (errori di sincronizzazione a causa di oggetti duplicati)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737345"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Errori di sincronizzazione a causa di oggetti duplicati

È possibile che venga visualizzato uno dei seguenti messaggi di errore quando la sincronizzazione della directory termina in Microsoft 365:

- Impossibile aggiornare l'oggetto nei servizi Microsoft online perché i seguenti attributi associati a questo oggetto dispongono di valori che potrebbero essere già associati a un altro oggetto nella directory locale.

- Un oggetto sincronizzato con lo stesso indirizzo proxy esiste già nella directory dei Microsoft Online Services.

- Non è possibile aggiornare l'oggetto perché i seguenti attributi associati a questo oggetto dispongono di valori che potrebbero essere già associati a un altro oggetto nei servizi directory locali: UserPrincipalName.

Per identificare e risolvere il problema, scaricare ed eseguire lo strumento di correzione degli [errori di IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Per ulteriori informazioni, vedere [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
