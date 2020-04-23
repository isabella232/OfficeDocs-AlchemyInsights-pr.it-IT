---
title: Record di dispositivo duplicati nel portale
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789866"
---
# <a name="duplicate-device-record-in-the-portal"></a>Record di dispositivo duplicati nel portale

È possibile che nel portale siano presenti 2 record se il dispositivo non segnala correttamente lo stato della co-gestione al sito di Configuration Manager. Per controllare lo stato della co-gestione di un dispositivo, esaminare la colonna **Con co-gestione** per il dispositivo nella console di Configuration Manager. Se la colonna non è visibile, è possibile aggiungerla facendo clic con il pulsante destro del mouse su qualsiasi intestazione di colonna e selezionandola nell'elenco.

Il valore Con co-gestione **Sì**. Se il valore è **No**, aprire l'applet del client di Configuration Manager nel dispositivo client e controllare la proprietà **Co-gestione** nella scheda Generale.

- Se il valore è **Abilitata**, i problemi sono associati alle comunicazioni del client nel punto di gestione. Esaminare il file **CcmMessaging.log** nel dispositivo per individuare i potenziali problemi di connettività.

- Se il valore è **Disabilitata** e il dispositivo è registrato in Intune, assicurarsi che il dispositivo abbia ricevuto i criteri di co-gestione esaminando il file **CoManagementHandler.log** nel dispositivo.
