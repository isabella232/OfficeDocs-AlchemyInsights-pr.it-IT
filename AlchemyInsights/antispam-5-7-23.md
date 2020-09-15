---
title: Protezione da posta indesiderata-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717329"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Risolvere problemi di recapito della posta elettronica per il codice di errore 5.7.23

Verificare il record DNS SPF per il dominio in un controllo del record SPF o DNS disponibile pubblicamente sul Web.

Verificare che il messaggio in uscita non sia stato identificato come posta indesiderata da Microsoft e instradato attraverso il [pool di recapito ad alto rischio](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). I messaggi nel pool di recapito ad alto rischio non superano i controlli SPF e pertanto non verranno accettati dall'organizzazione di posta elettronica di destinazione.

Se il problema persiste, potrebbe essere necessario contattare l'amministratore dell'host di posta elettronica a cui si sta tentando di inviare messaggi di posta elettronica. Prendere nota dell'errore esterno dettagliato disponibile nel messaggio di rimbalzo. Il supporto tecnico Microsoft potrebbe non essere in grado di supportare ulteriormente.
