---
title: スナップショットから VM を作成する - PowerShell サンプル
description: Azure PowerShell のサンプル スクリプト - スナップショットから VM を作成します
services: virtual-machines-linux
documentationcenter: virtual-machines
author: ramankumarlive
manager: kavithag
editor: ramankum
tags: azure-service-management
ms.assetid: ''
ms.service: virtual-machines-linux
ms.topic: sample
ms.tgt_pltfrm: vm-linux
ms.workload: infrastructure
ms.date: 05/10/2017
ms.author: ramankum
ms.custom: mvc
ms.openlocfilehash: 21e31df7552dfe5e6368235173622695078626b9
ms.sourcegitcommit: 0947111b263015136bca0e6ec5a8c570b3f700ff
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2020
ms.locfileid: "75463663"
---
# <a name="create-a-virtual-machine-from-a-snapshot-with-powershell"></a>PowerShell でスナップショットから仮想マシンを作成する

このスクリプトは、OS ディスクのスナップショットから仮想マシンを作成します。

[!INCLUDE [quickstarts-free-trial-note](../../../includes/quickstarts-free-trial-note.md)]

 

## <a name="sample-script"></a>サンプル スクリプト

[!code-powershell[main](../../../powershell_scripts/virtual-machine/create-vm-from-snapshot/create-vm-from-snapshot.ps1 "Create VM from managed os disk")]

## <a name="clean-up-deployment"></a>デプロイのクリーンアップ

次のコマンドを実行して、リソース グループ、VM、すべての関連リソースを削除します。

```powershell
Remove-AzResourceGroup -Name myResourceGroup
```

## <a name="script-explanation"></a>スクリプトの説明

このスクリプトは、次のコマンドを使用して、スナップショットのプロパティを取得し、スナップショットからマネージド ディスクを作成し、VM を作成します。 表内の各項目は、コマンドごとのドキュメントにリンクされています。

| command | メモ |
|---|---|
| [Get-AzSnapshot](https://docs.microsoft.com/powershell/module/az.compute/get-azsnapshot) | スナップショット名を使用してスナップショットを取得します。 |
| [New-AzDiskConfig](https://docs.microsoft.com/powershell/module/az.compute/new-azdiskconfig) | ディスク構成を作成します。 この構成は、ディスク作成プロセスで使用されます。 |
| [New-AzDisk](https://docs.microsoft.com/powershell/module/az.compute/new-azdisk) | マネージド ディスクを作成します。 |
| [New-AzVMConfig](https://docs.microsoft.com/powershell/module/az.compute/new-azvmconfig) | VM 構成を作成します。 この構成には、VM 名、オペレーティング システム、管理資格情報などの情報が含まれます。 この構成は、VM の作成時に使用されます。 |
| [Set-AzVMOSDisk](https://docs.microsoft.com/powershell/module/az.compute/set-azvmosdisk) | マネージド ディスクを OS ディスクとして仮想マシンに接続します。 |
| [New-AzPublicIpAddress](https://docs.microsoft.com/powershell/module/az.network/new-azpublicipaddress) | パブリック IP アドレスを作成します。 |
| [New-AzNetworkInterface](https://docs.microsoft.com/powershell/module/az.network/new-aznetworkinterface) | ネットワーク インターフェイスを作成します。 |
| [New-AzVM](https://docs.microsoft.com/powershell/module/az.compute/new-azvm) | 仮想マシンを作成します。 |
|[Remove-AzResourceGroup](https://docs.microsoft.com/powershell/module/az.resources/remove-azresourcegroup) | リソース グループと、それに含まれているすべてのリソースを削除します。 |

## <a name="next-steps"></a>次のステップ

Azure PowerShell モジュールの詳細については、[Azure PowerShell のドキュメント](/powershell/azure/overview)を参照してください。

その他の仮想マシン用の PowerShell サンプル スクリプトは、[Azure Linux VM のドキュメント](../linux/powershell-samples.md?toc=%2fazure%2fvirtual-machines%2flinux%2ftoc.json)にあります。