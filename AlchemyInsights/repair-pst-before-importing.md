---
title: Ripristinare il file PST prima di importarlo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 518543f664873c99d5f296284199cd417c620e00
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720141"
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
