---
title: Autenticazione a più fattori imprevista
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: a664bd709062ec1335ebcf1f9adddc8aef917ac1
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766605"
---
# <a name="unexpected-multi-factor-authentication"></a>Autenticazione a più fattori imprevista

Se il tenant è stato creato dopo il 21 ottobre 2019 e si riceve una richiesta di conferma per l'autenticazione a più fattori, è probabile che siano state abilitate le [impostazioni predefinite per la sicurezza](https://aka.ms/securitydefaults) nel tenant. 

Per gestire le impostazioni predefinite per la sicurezza:

1. Accedere all'[interfaccia di amministrazione](https://go.microsoft.com/fwlink/p/?linkid=834822) con le credenziali di amministratore globale.

2. Passare alle [Proprietà di Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).

3. Nella parte inferiore della pagina fare clic su **Gestire le impostazioni predefinite per la sicurezza**.

4. Fare clic su **Sì** per abilitare le impostazioni predefinite di sicurezza e su **No** per disabilitare le impostazioni predefinite per la sicurezza.
