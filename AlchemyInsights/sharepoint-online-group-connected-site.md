---
title: Aggiungere un gruppo a un sito di SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719486"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Creare un sito connesso a un gruppo in SharePoint Online

<p><strong>Durante la creazione o la ricreazione di un sito collegato a un gruppo sono stati riscontrati un paio di problemi comuni.&nbsp;</strong></p>  <p>1.Se è stato eliminato un gruppo e il relativo sito connesso e si desidera creare un altro sito con lo stesso URL, è necessario rimuovere definitivamente il sito precedente.</p>  <ul>  <li>Scaricare <a title="SPO Management Shell" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - per altre informazioni su Guida introduttiva a PowerShell, <a title="vedere Guida introduttiva a SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Guida introduttiva a SharePoint Online Management</a>Shell. <br /><br /></li>  <li>Rimuovere il sito dai siti eliminati utilizzando il <a title="SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Cmdlet Remove-</a> SPODeletedSite di PowerShell.</li>  </ul>  <p>Se si sta creando un sito collegato a un gruppo e viene visualizzato un messaggio di avviso <strong>"è già presente un altro gruppo con lo stesso alias"</strong>, controllare i gruppi esistenti dall'interfaccia di amministrazione di <a title="Office 365" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 dall'interfaccia di amministrazione</a>. Per risolvere il problema, eliminare il gruppo esistente se non è più necessario o creare il sito con un altro alias assegnato.&nbsp;</p>  <p><strong>Esistono diversi modi per creare e utilizzare i gruppi moderni con SharePoint.&nbsp;</strong></p>  <ol>  <li>È possibile connettere i siti esistenti a un gruppo di Office 365. Per altre informazioni, vedere <a title="connettere un gruppo di Office 365 utilizzando l'utente di ineterface di SharePoint" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Connettere un gruppo di Office 365 utilizzando l'utente di</a>SharePoint ineterface.</li>  <li>Per creare un sito collegato a un gruppo di Office 365, è necessario creare un sito del team. Per altre informazioni, vedere <a title="creare un sito del team in SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Creare un sito del team in SharePoint.</a></li>  </ol>

