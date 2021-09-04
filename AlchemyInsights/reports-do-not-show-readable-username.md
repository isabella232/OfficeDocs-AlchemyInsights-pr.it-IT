---
title: Il nome utente non è leggibile nei report nell'interfaccia di amministrazione di Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2021
ms.locfileid: "58896348"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Il nome utente non è leggibile nei report nell'interfaccia di amministrazione di Microsoft 365

I report nell'interfaccia di amministrazione di Microsoft 365 non mostrano i nomi utente, ma valori alfanumerici come B2BC6C15BB9FCDEA71E5CD302D228CC8.

Questo comportamento è previsto ed è stato comunicato nel Centro messaggi (MC275344, pubblicato il 3 agosto 2021). 

Gli amministratori globali possono ripristinare questa modifica per il tenant e mostrare informazioni personali dell'utente, se le procedure di privacy dell'organizzazione lo consentono. Per ripristinare la modifica per il tenant:

1. Nell'interfaccia di amministrazione, passare a **Impostazioni** > **Impostazioni organizzazione** > [**Servizi**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services) e selezionare **Report**. 
1. In **Scegliere come mostrare le informazioni utente**, selezionare **Mostra informazioni personali dell'utente nei report** ed eseguire di nuovo il report.