---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821415"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Risolvere i problemi di recapito della posta elettronica per il codice di errore 5.7.23

Verificare il record DNS SPF per il dominio in un controllo record SPF o DNS disponibile pubblicamente sul Web.

Verificare che il messaggio in uscita non sia stato identificato come posta indesiderata da Microsoft e instradato tramite [il pool di recapito ad alto rischio.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) I messaggi nel pool di recapito ad alto rischio non supereranno i controlli SPF e pertanto non verranno accettati dall'organizzazione di posta elettronica di destinazione.

Se il problema persiste, potrebbe essere necessario contattare l'amministratore dell'host di posta a cui si sta tentando di inviare posta elettronica. Prendere nota dell'errore esterno dettagliato disponibile nel messaggio di mancato recapito. Il supporto Tecnico Microsoft potrebbe non essere in grado di fornire ulteriore assistenza.
