---
title: Azure Notification Hubs で Microsoft プッシュ通知サービスを構成する | Microsoft Docs
description: Azure 通知ハブ用に Microsoft プッシュ通知サービスの設定を構成する方法について説明します。
services: notification-hubs
author: sethmanheim
manager: femila
editor: jwargo
ms.service: notification-hubs
ms.workload: mobile
ms.topic: article
ms.date: 03/25/2019
ms.author: sethm
ms.reviewer: jowargo
ms.lastreviewed: 03/25/2019
ms.openlocfilehash: 99f29e7910fe6070c6202f6a936173455f979732
ms.sourcegitcommit: 2ec4b3d0bad7dc0071400c2a2264399e4fe34897
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2020
ms.locfileid: "80127340"
---
# <a name="configure-microsoft-push-notification-service-mpns-settings-in-the-azure-portal"></a>Azure portal で Microsoft プッシュ通知サービス (MPNS) の設定を構成する

この記事では、Azure portal を使用して Azure 通知ハブ用に Microsoft プッシュ通知サービス (MPNS) の設定を構成する方法について説明します。 

## <a name="prerequisites"></a>前提条件
通知ハブを作成していない場合は、ここで作成します。 詳細については、「[Azure portal 内で Azure 通知ハブを作成する](create-notification-hub-portal.md)」を参照してください。 

## <a name="configure-microsoft-push-notification-service-mpns"></a>Microsoft プッシュ通知サービス (MPNS) の構成

次の手順は、通知ハブ用に Microsoft プッシュ通知サービス (MPNS) の設定を構成する手順を示しています。 

1. Azure portal の **[通知ハブ]** ページで、左側のメニューの **[Windows Phone (MPNS)]** を選択します。
1. 非認証プッシュ通知または認証済みプッシュ通知を有効にします。

   a. 非認証プッシュ通知を有効にするには、 **[非認証プッシュを有効にする]**  >  **[保存]** の順に選択します。

      ![非認証プッシュ通知を有効にする方法を示したスクリーンショット](./media/notification-hubs-windows-phone-get-started/azure-portal-unauth.png)

   b. 認証済みプッシュ通知を有効にするには、次の手順に従います。
      * ツール バーの **[証明書のアップロード]** を選択します。
      * ファイル アイコンを選択し、証明書ファイルを選択します。
      * 証明書のパスワードを入力します。
      * **[OK]** を選択します。
      * **[Windows Phone(MPNS)]** ページで、 **[保存]** を選択します。

## <a name="next-steps"></a>次のステップ
Azure Notification Hubs と Microsoft プッシュ通知サービス (MPNS) を使用して、Windows Phone デバイスにプッシュ通知を送信する詳細な手順については、「[Azure Notification Hubs を使用して Windows Phone アプリにプッシュ通知を送信する](notification-hubs-windows-mobile-push-notifications-mpns.md)」を参照してください。

