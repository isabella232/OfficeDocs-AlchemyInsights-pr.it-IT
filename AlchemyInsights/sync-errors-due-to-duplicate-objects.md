---
title: 902 (Errori di sincronizzazione a causa di oggetti duplicati)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708066"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Errori di sincronizzazione dovuti a oggetti duplicati

Al termine della sincronizzazione della directory in Microsoft 365, potrebbe essere visualizzato uno dei seguenti messaggi di errore:

- Impossibile aggiornare questo oggetto in Microsoft Online Services perché gli attributi seguenti associati a questo oggetto hanno valori che potrebbero essere già associati a un altro oggetto nella directory locale.

- Un oggetto sincronizzato con lo stesso indirizzo proxy esiste già nella directory Microsoft Online Services locale.

- Impossibile aggiornare questo oggetto perché gli attributi seguenti associati a questo oggetto hanno valori che potrebbero essere già associati a un altro oggetto nei servizi directory locali: UserPrincipalName.

Per identificare e risolvere il problema, scaricare ed eseguire lo strumento di correzione degli errori [di DirSync idFix.](https://github.com/Microsoft/idfix)

Per ulteriori informazioni, vedere [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
