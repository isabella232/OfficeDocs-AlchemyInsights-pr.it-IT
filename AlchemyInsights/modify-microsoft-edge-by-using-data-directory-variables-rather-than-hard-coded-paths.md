---
title: Modificare Microsoft Edge usando variabili di directory dei dati anziché i percorsi hardcoded
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897893"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Modificare Microsoft Edge usando variabili di directory dei dati anziché i percorsi hardcoded

Ad esempio, in Windows, per archiviare i dati del profilo nei dati dell’applicazione locale di un utente anziché nella posizione predefinita, impostare il criterio *UserDataDir* su **${local_app_data}\Edge\Profile**.

Per ulteriori informazioni, vedere [Creare variabili di directory dei dati utente di Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).