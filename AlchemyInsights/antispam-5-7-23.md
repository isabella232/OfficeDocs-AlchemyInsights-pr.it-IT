---
title: Protezione da posta indesiderata-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676501"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Risolvere problemi di recapito della posta elettronica per il codice di errore 5.7.23

Verificare il record DNS SPF per il dominio in un controllo del record SPF o DNS disponibile pubblicamente sul Web.

Verificare che il messaggio in uscita non sia stato identificato come posta indesiderata da Microsoft e instradato attraverso il [pool di recapito ad alto rischio](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). I messaggi nel pool di recapito ad alto rischio non superano i controlli SPF e pertanto non verranno accettati dall'organizzazione di posta elettronica di destinazione.

Se il problema persiste, potrebbe essere necessario contattare l'amministratore dell'host di posta elettronica a cui si sta tentando di inviare messaggi di posta elettronica. Prendere nota dell'errore esterno dettagliato disponibile nel messaggio di rimbalzo. Il supporto tecnico Microsoft potrebbe non essere in grado di supportare ulteriormente.
