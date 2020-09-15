---
title: Profili Wi-Fi di Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696265"
---
# <a name="intune-wi-fi-profiles"></a>Profili Wi-Fi di Intune

L'implementazione efficace della connettività Wi-Fi per i client MDM dipende da un profilo distribuito correttamente che riflette i requisiti dell'infrastruttura Wi-Fi aziendale. Per verificare le impostazioni appropriate per le piattaforme client su cui si sta lavorando, si veda: 

[Aggiungere impostazioni Wi-Fi per i dispositivi che utilizzano Android in Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Aggiungere impostazioni Wi-Fi per i dispositivi Android Enterprise dedicati e completamente gestiti in Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Aggiungere impostazioni Wi-Fi per i dispositivi iOS e iPadOS in Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Aggiungere impostazioni Wi-Fi per dispositivi Windows 10 e successivi in Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Aggiungere impostazioni Wi-Fi per dispositivi Windows in Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Problemi comuni**

**Si sta distribuendo un profilo Wi-Fi che dipende da un certificato distribuito specificato nel profilo Wi-Fi. Tuttavia, i profili di configurazione indicano uno stato di errore.**

Controllare che il dispositivo abbia ricevuto il certificato.

1. In Intune, andare su **Tutti i dispositivi** e selezionare il dispositivo > **Configurazione dispositivo**.

2. Controllare che tutti i profili previsti siano elencati e completati.

3. Per un profilo Android, se nella catena di certificati sono presenti certificati intermedi, accertarsi che siano distribuiti ai dispositivi Android.

    Per controllare lo stato del certificato, andare su **Configurazione dispositivo** > **Profili** > **Android CA intermedio** > **Proprietà** > **Certificato attendibile**.

Se si continuano a visualizzare errori, rivedere le sezioni relative alle procedure e alla risoluzione dei problemi. Per maggiori informazioni, si veda [Panoramica per la risoluzione dei problemi relativi ai profili dei certificati SCEP con Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Si è distribuito un profilo Wi-Fi in un dispositivo. Intune indica che l'operazione è riuscita, ma il dispositivo non è connesso alla rete Wi-Fi.**

Lo stato corretto indica che Intune ha distribuito correttamente il profilo come configurato. Tuttavia, queste configurazioni potrebbero non corrispondere ai requisiti di rete e/o di autenticazione. Per maggiori dettagli sul tentativo di connessione, rivedere i registri nel servizio di infrastruttura e autenticazione (sul controller del punto di accesso al Wi-Fi e sul server NPS/Radius). Potrebbe essere necessario collaborare con il team dell'infrastruttura di rete o il terzo fornitore del Wi-Fi per raccogliere e rivedere i registri.