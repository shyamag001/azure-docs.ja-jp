---
title: Azure CLI Azure Cache for Redis のサンプル
description: Azure Cache for Redis 用の Azure CLI サンプルキャッシュの作成、キャッシュの削除、キャッシュの詳細、ホスト名、ポート、およびキーの取得、Web アプリの接続。
author: yegu-ms
ms.author: yegu
ms.service: cache
ms.devlang: azurecli
ms.topic: conceptual
ms.date: 04/14/2017
ms.openlocfilehash: c43e23b4bf46258cc91b06a0912d03e85a5c7a14
ms.sourcegitcommit: 849bb1729b89d075eed579aa36395bf4d29f3bd9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2020
ms.locfileid: "75411359"
---
# <a name="azure-cli-samples-for-azure-cache-for-redis"></a>Azure Cache for Redis 用の Azure CLI サンプル

次の表には、Azure CLI を使用して構築された Bash スクリプトへのリンクが含まれています。

| | |
|---|---|
|**キャッシュの作成**||
| [キャッシュを作成する](./scripts/create-cache.md) | リソース グループと Basic レベルの Azure Cache for Redis を作成します。 |
| [クラスタリングを使用した Premium キャッシュの作成](./scripts/create-premium-cache-cluster.md) | リソース グループとクラスタリングが有効になっている Premium レベルのキャッシュを作成します。|
| [キャッシュの詳細を取得する](./scripts/show-cache.md) | プロビジョニングの状態を含む、Azure Cache for Redis インスタンスの詳細を取得します。 |
| [ホスト名、ポート、およびキーを取得する](./scripts/cache-keys-ports.md) | Azure Cache for Redis インスタンスのホスト名、ポート、およびキーを取得します。 |
|**Web アプリとキャッシュ**||
| [Azure Cache for Redis に Web アプリを接続する](./../app-service/scripts/cli-connect-to-redis.md) | Azure Web アプリと Azure Cache for Redis を作成し、Redis の接続の詳細をアプリケーション設定に追加します。 |
|**キャッシュの削除**||
| [キャッシュを削除する](./scripts/delete-cache.md) | Azure Cache for Redis インスタンスを削除する  |
| | |

Azure CLI の詳細については、[Azure CLI のインストール](https://docs.microsoft.com/cli/azure/install-azure-cli)と[Azure CLI の概要](https://docs.microsoft.com/cli/azure/get-started-with-azure-cli)に関するぺージを参照してください。
