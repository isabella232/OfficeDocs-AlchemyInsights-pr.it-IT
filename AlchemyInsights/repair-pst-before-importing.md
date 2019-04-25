---
title: Ripristinare il file PST prima di importarlo
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1226
ms.assetid: ''
ms.openlocfilehash: 66b045c04ccbeb133e1bae3b9c29e01b4820d33f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383768"
---
# <a name="repair-pst-file-before-importing"></a>Ripristinare il file PST prima di importarlo

Prima di importare un file. pst in Outlook, verificare che il file non sia danneggiato ripristinando il file:

1. Uscire da Outlook.

2. Individuare ed eseguire `Scanpst.exe` la cartella del programma di Office (c:\Program Files (x86) \Microsoft\<Office\root\Office\> Version o c:\Programmi\Microsoft Office\root\Office\<Version\>).

3. Nello **strumento di ripristino Posta in arrivo di Microsoft Outlook**fare clic su **Sfoglia** per individuare il file. pst (ad\\esempio\>, in C:\Users <username \AppData\Local\Microsoft\Outlook). Selezionare il file con estensione pst e quindi fare clic su **Apri**.

4. Fare clic su **Avvia** per avviare l'analisi.

5. Se si verificano errori nel file, fare clic su **Ripristina**e quindi fare clic su **OK** al termine del ripristino.

6. Provare a importare di nuovo il file. pst in Outlook.

Per ulteriori informazioni, vedere [ripristinare i file di dati di Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) e [correggere i problemi relativi all'importazione di un file PST di Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
