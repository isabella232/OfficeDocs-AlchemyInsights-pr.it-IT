---
title: Termini mancanti dall'SharePoint termini online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106430"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Abilitazione della crittografia Bitlocker con Intune

I criteri Endpoint Protection Intune possono essere usati per configurare le impostazioni di crittografia Boitlocker per i dispositivi Windows, come descritto in : Impostazioni di Windows10 (e versioni successive) per proteggere i dispositivi con Intune

Tenere presente che molti dispositivi più nuovi che eseguono Windows 10 la crittografia bitlocker automatica che viene attivata senza l'applicazione dei criteri MDM. Ciò può influire sull'applicazione dei criteri se sono configurate impostazioni non predefinite. Per ulteriori dettagli, vedere Domande frequenti.


Domande frequenti D: Quali edizioni di Windows supportano la crittografia dei dispositivi usando i Endpoint Protection criteri?
A: Le impostazioni in Intune Endpoint Protection criteri sono implementate usando il CSP Bitlocker.  Non tutte le edizioni né le build di Windows supportano il CSP Bitlocker. In questo momento Windows edizioni: Enterprise; Education, Mobile, Mobile Enterprise e Professional (dalla build 1809 in poi) sono supportati.




D: Se un dispositivo è già crittografato con Bitlocker usando le impostazioni predefinite del sistema operativo per il metodo di crittografia e la forza di crittografia (XTS-AES-128), verrà applicato un criterio con impostazioni diverse che attiva automaticamente la nuova crittografia dell'unità con le nuove impostazioni?

R: no. Per applicare le nuove impostazioni di crittografia, l'unità deve prima essere decrittografata.

Nota Per i dispositivi registrati con Autopilot, la crittografia automatica che si verificherebbe durante la configurazione guidata non viene attivata fino a quando non viene valutato il criterio di Intune che consente di usare le impostazioni basate sui criteri al posto delle impostazioni predefinite del sistema operativo




D Se un dispositivo viene crittografato a seguito dell'applicazione dei criteri di Intune, verrà decrittografato quando tale criterio viene rimosso?

A: La rimozione dei criteri correlati alla crittografia NON comporta la decrittografia delle unità configurate.




D: Perché i criteri di conformità di intune mostrano che il dispositivo non ha "Bitlocker Abilitato", ma lo è?

A: L'impostazione "Bitlocker abilitato" nei criteri di conformità di intune utilizza il client DHA (Device Health Attestation) Windows. Questo client misura solo lo stato del dispositivo al momento dell'avvio. Pertanto, se un dispositivo non è stato riavviato dopo il completamento della crittografia bitlocker, il servizio client DHA non segnala bitlocker come attivo.