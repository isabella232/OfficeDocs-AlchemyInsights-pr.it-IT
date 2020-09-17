---
title: How-to-Import-NK2-files
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
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780063"
---
# <a name="how-to-import-nk2-files"></a>Come importare file con estensione NK2 

Quando si avvia Microsoft Outlook 2013, Outlook 2016, Outlook 2019 o Outlook per Microsoft 365 per la prima volta, la cache dei Nickname (archiviata nel file *ProfileName*. nk2) viene importata in un messaggio nascosto nell'archivio dei messaggi predefinito.

Per importare i file. nk2 in Outlook 2013, Outlook 2016, Outlook 2019 o Outlook per Microsoft 365, verificare che il file. nk2 si trovi nella cartella seguente:%appdata%\Microsoft\Outlook

**Nota**: il file. nk2 deve avere lo stesso nome del profilo di Outlook 2013 o Outlook 2016 corrente. Per impostazione predefinita, il nome del profilo è "Outlook". Per verificare il nome del profilo, attenersi alla seguente procedura: 
1. Fare clic sul pulsante **Start** e quindi scegliere **Pannello di controllo**.
2. Fare doppio clic su **posta**.
3. Nella finestra di dialogo Imposta posta elettronica selezionare **Mostra profili**.
4. Selezionare **Avvia**  >  **esecuzione**.
5. Nella casella **Apri** Digitare *outlook.exe/importnk2*e quindi fare clic su **OK**. 

Dopo aver importato il file. nk2, il contenuto del file viene unito alla cache dei soprannomi esistente memorizzata nella cassetta postale.

**Nota**: il file. nk2 viene rinominato con estensione di file. Old al successivo avvio di Outlook 2013, Outlook 2016, Outlook 2019 o Outlook per Microsoft 365. Se si desidera importare di nuovo il file. nk2, rimuovere prima l'estensione del nome di file. old.

Per ulteriori informazioni, vedere [importare o copiare l'elenco di completamento automatico in un altro computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).