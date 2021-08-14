---
title: Usare TeamViewer per gestire da remoto i dispositivi Intune
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
- "1284"
- "6700008"
ms.openlocfilehash: 35c82f8b91a4a0a75f8aa376771a20e6684620c55e8a06abe59db22cab945139
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53990531"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Usare TeamViewer per gestire da remoto i dispositivi Intune

I dispositivi gestiti da Intune possono essere amministrati da remoto con [TeamViewer](https://www.teamviewer.com/).

Per gestire Intune con TeamViewer, eseguire le operazioni seguenti: 

Per iniziare, occorre ottenere le credenziali da TeamViewer per configurare TeamViewer Connector in Intune. Questo consente all'amministratore di immettere le credenziali nell'interfaccia utente di TeamViewer Connector sotto Dispositivi, un'operazione una tantum per stabilire il collegamento tra Intune e il servizio TeamViewer.

**Parte 1: avviare una sessione con un dispositivo remoto**

1. In **Tutti i dispositivi** selezionare il dispositivo con cui si vuole iniziare una sessione remota.
2. Da **... Altro**, selezionare **Nuova sessione di assistenza remota**.
3. Selezionare **Sì** per confermare che si vuole stabilire una sessione remota.
    Dopo la conferma della richiesta di "Avvio di una nuova sessione remota" da parte del servizio TeamViewer, viene visualizzata un'opzione che consente di **Avviare assistenza remota** sotto i dettagli del riquadro Panoramica o Informazioni di base per il dispositivo. Selezionare **Vedere altro** per espandere il riquadro e visualizzare lo stato dell'assistenza remota.
4. Selezionare **Avvia sessione remota** per avviare la sessione a favore dell’amministratore.
5. Scegliere di scaricare il file binario di TeamViewer (Windows) e selezionare **Eseguire**.<br/>
    **Nota** È possibile ignorare qualsiasi pagina del Web browser aperta sul sito Web di TeamViewer.

6. Confermare la richiesta dell'app TeamViewer di apportare modifiche al dispositivo (solo per Windows).
7. L'app TeamViewer è avviata e include il codice di sessione per autenticare la connessione con il dispositivo remoto.

**Parte 2: nel dispositivo di destinazione di una sessione remota**

1. Aprire il portale aziendale Intune.
2. Cercare un contrassegno di notifica: "L’amministratore IT richiede un controllo del dispositivo per una sessione di assistenza remota" e selezionare la notifica.
3. Scegliere di scaricare l'applicazione TeamViewer o confermare il download dell'app TeamViewer dall'App Store e selezionare **Eseguire**.
    **Nota** È possibile ignorare qualsiasi pagina del Web browser aperta sul sito Web di TeamViewer.

4. Confermare la richiesta dell'app TeamViewer di apportare modifiche al dispositivo (solo per Windows).
5. L'app TeamViewer è avviata e include il codice di sessione per autenticare la connessione con il dispositivo remoto.
6. Un popup richiede se si vuole consentire l'avvio della sessione.

**Nota** I codici di sessione generati dal servizio TeamViewer sono utilizzabili una sola volta. Se si perde la connessione, è necessario:

1. Chiudere l'istanza dell'app TeamViewer nel dispositivo remoto e nella postazione di lavoro dell’amministratore.
2. Chiudere il portale aziendale nel dispositivo remoto.
3. Avviare una "Nuova sessione di assistenza remota" nel portale di amministrazione.
4. Riaprire il portale aziendale nel dispositivo remoto per ricevere la nuova notifica.
5. Scaricare e aprire l'app TeamViewer sia nel dispositivo remoto sia nella postazione di lavoro dell’amministratore, come in precedenza.