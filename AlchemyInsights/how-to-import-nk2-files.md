---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043210"
---
# <a name="how-to-import-nk2-files"></a>Come importare file nk2 

Quando si avvia Microsoft Outlook 2013, Outlook 2016, Outlook 2019 o Outlook per Microsoft 365 per la prima volta, la cache dei nomi alternativi (archiviata nel file nomeprogetto .nk2) viene importata in un messaggio nascosto nell'archivio messaggi predefinito.

Per importare file nk2 in Outlook 2013, Outlook 2016, Outlook 2019 o Outlook per Microsoft 365, verificare che il file nk2 si trova nella cartella seguente: %appdata%\Microsoft\Outlook

**Nota:** il file nk2 deve avere lo stesso nome del profilo Outlook 2013 o Outlook 2016 2013. Per impostazione predefinita, il nome del profilo è "Outlook". Per controllare il nome del profilo, attenersi alla seguente procedura: 
1. Fare clic sul pulsante **Start** e quindi scegliere **Pannello di controllo**.
2. Fare doppio clic su **Posta**.
3. Nella finestra di dialogo Configurazione posta selezionare **Mostra profili**.
4. Selezionare **Start** > **Esegui**.
5. Nella casella **Apri** digitareoutlook.exe */importnk2* e quindi selezionare **OK.** 

Dopo aver importato il file nk2, il contenuto del file viene unito nella cache dei nomi alternativi esistente archiviata nella cassetta postale.

**Nota:** il file nk2 viene rinominato con estensione old al successivo avvio di Outlook 2013, Outlook 2016, Outlook 2019 o Outlook per Microsoft 365. Se si desidera importare di nuovo il file nk2, rimuovere prima l'estensione .old.

Per ulteriori informazioni, vedere [Importare o copiare l'elenco di completamento automatico in un altro computer.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)