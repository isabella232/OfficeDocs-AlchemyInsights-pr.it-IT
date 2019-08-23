---
title: Ripristinare il file PST prima di importarlo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 3f273d9807a20048f33ce476e091ee2122a773d4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36552427"
---
# <a name="repair-pst-file-before-importing"></a>Ripristinare il file PST prima di importarlo

Prima di importare un file. pst in Outlook, verificare che il file non sia danneggiato ripristinando il file:

1. Uscire da Outlook.

2. Individuare ed eseguire `Scanpst.exe` la cartella del programma di Office (c:\Program Files (x86) \Microsoft\<Office\root\Office\> Version o c:\Programmi\Microsoft Office\root\Office\<Version\>).

3. Nello **strumento di ripristino Posta in arrivo di Microsoft Outlook**fare clic su **Sfoglia** per individuare il file. pst (ad\\ esempio,\>in C:\Users<nomeutente \AppData\Local\Microsoft\Outlook). Selezionare il file con estensione pst e quindi fare clic su **Apri**.

4. Fare clic su **Avvia** per avviare l'analisi.

5. Se si verificano errori nel file, fare clic su **Ripristina**e quindi fare clic su **OK** al termine del ripristino.

6. Provare a importare di nuovo il file. pst in Outlook.

Per ulteriori informazioni, vedere [ripristinare i file di dati di Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) e [correggere i problemi relativi all'importazione di un file PST di Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
