---
title: Risolvere i problemi di arresto anomalo di OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921011"
---
# <a name="troubleshoot-onedrive-crashes"></a>Risolvere i problemi di arresto anomalo di OneDrive

Se OneDrive si arresta spesso in modo anomalo, provare queste procedure per la risoluzione dei problemi:

**Assicurarsi che non siano impostate chiavi del Registro di sistema:**

1. Usando l'Editor del Registro di sistema, passare a HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Se è presente la chiave DisableFileSyncNGSC con il valore impostato su 1, aprire la chiave e cambiare il valore in 0.
3. Avviare manualmente OneDrive facendo clic su Start ![Premere il tasto WINDOWS](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), digitare OneDrive nella casella di ricerca e quindi fare clic sull'app OneDrive desktop.

**Reimpostare OneDrive:**

Note:

- La reimpostazione di OneDrive disconnette tutte le connessioni di sincronizzazione esistenti (incluso OneDrive personale, se configurato).
- Quando si reimposta OneDrive nel computer, i file e i dati vengono preservati.

**Per reimpostare OneDrive:**

1. Aprire una finestra di dialogo Esegui premendo il tasto WINDOWS e R.
2. Digitare %localappdata%\Microsoft\OneDrive\onedrive.exe /reset e scegliere OK. Potrebbe comparire una finestra di comando per un istante.
3. Avviare manualmente OneDrive facendo clic su Start ![Premere il tasto WINDOWS](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), digitare OneDrive nella casella di ricerca e quindi fare clic sull'app OneDrive desktop.

Note:

- Se prima del ripristino era stata impostata la sincronizzazione solo di alcune cartelle, si dovrà applicare di nuovo questa impostazione al termine della sincronizzazione. Per altre informazioni, vedere [Scegliere le cartelle di OneDrive da sincronizzare con il computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) .
- È necessario completare la procedura per OneDrive personale e OneDrive for Business.