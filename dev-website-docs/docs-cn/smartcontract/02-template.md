

* Native 合约 API： 有关本体网络中使用的 Native 合约 API，请参考 [Native Contract API](https://github.com/ontio/ontology/blob/master/docs/specifications/native_contract/paramapi.md)。

* Python 合约 API： 有关本体网络中使用的 Python 合约 API 和示例，请参考 [API doc](https://apidoc.ont.io/smartcontract/)。


为了方便开发者快速开始智能合约编写，我们提供了众多实用的合约模板。

我们推出了1.0和2.0 两个版本的编译器，今后将以2.0作为主流，请各位优先参考适配2.0版本的模板

### 2.0 模板

| # | 智能合约                         |        语言      |   描述   |
| -----| ---------------------------------------- | ---------------- | ---------------- |
| 1| [Oep4](https://github.com/ONT-Avocados/python-template/blob/master/OEP4Sample/OEP4Sample_compiler2.0.py) |    Python     |    Oep4  |
| 2| [Oep5](https://github.com/ONT-Avocados/python-template/blob/master/OEP5Sample/OEP5Sample_compiler2.0.py) |  Python   |  Oep5   |
| 3| [Oep8](https://github.com/ONT-Avocados/python-template/blob/master/OEP8Sample/OEP8Sample_compiler2.0.py) |  Python   |  Oep8   |
| 4| [Invoke Oep4](https://github.com/ONT-Avocados/python-template/blob/master/Static_Call_Oep4/static_call_Oep4_compiler2.0.py) |  Python  | 在智能合约中调用 Oep4 方法 |
| 5| [Storage example](https://github.com/ONT-Avocados/python-template/blob/master/Storage_Example/storage_example_compiler2.0.py) |   Python  |   Storage 示例  |
| 6| [Struct example](https://github.com/ONT-Avocados/python-template/blob/master/Struct_Example/struct_example_compiler2.0.py) |   Python  | Struct 示例  |
| 7| [Invoke native in sc](https://github.com/ONT-Avocados/python-template/blob/master/NativeAssetInvoke/native_asset_invoke_compiler2.0.py) | Python | 在智能合约中调用 native |
| 8| [Migrate Contract](https://github.com/ONT-Avocados/python-template/blob/master/MigrateDestruct/migrate_destroyWithinContract_compiler2.0.py) | Python | 迁移合约 |
| 9| [Event test](https://github.com/ONT-Avocados/python-template/blob/master/EventTest/event_test_compiler2.0.py) | Python|   Event 测试  |
|10| [Smart contract libs](https://github.com/ONT-Avocados/python-template/tree/master/libs) | Python|  合约 libs    |

> 2.0编译版本中，`from boa.builtins import concat,ToScriptHash` 由于方法重复已经被取消，请使用`from ontology.interop.Ontology.Runtime import Base58ToAddress`

### 1.0 模板

| # | 智能合约                         |        语言      |   描述   |
| -----| ---------------------------------------- | ---------------- | ---------------- |
| 1| [Oep4](https://github.com/ONT-Avocados/python-template/blob/master/OEP4Sample/OEP4Sample.py) |    Python     |    Oep4  |
| 2| [Oep5](https://github.com/ONT-Avocados/python-template/blob/master/OEP5Sample/OEP5Sample.py) |  Python   |  Oep5   |
| 3| [Oep8](https://github.com/ONT-Avocados/python-template/blob/master/OEP8Sample/OEP8Sample.py) |  Python   |  Oep8   |
| 4| [Invoke Oep4](https://github.com/ONT-Avocados/python-template/blob/master/Static_Call_Oep4/static_call_Oep4.py) |  Python  | 在智能合约中调用 Oep4 方法 |
| 5| [Storage example](https://github.com/ONT-Avocados/python-template/blob/master/Storage_Example/storage_example.py) |   Python  |   Storage 示例  |
| 6| [Struct example](https://github.com/ONT-Avocados/python-template/blob/master/Struct_Example/struct_example.py) |   Python  | Struct 示例  |
| 7| [Invoke native in sc](https://github.com/ONT-Avocados/python-template/blob/master/NativeAssetInvoke/native_asset_invoke.py) | Python | 在智能合约中调用 native |
| 8| [Migrate Contract](https://github.com/ONT-Avocados/python-template/blob/master/MigrateDestruct/migrate_destroyWithinContract.py) | Python | 迁移合约 |
| 9| [Event test](https://github.com/ONT-Avocados/python-template/blob/master/EventTest/event_test.py) | Python|   Event 测试  |
|10| [Smart contract libs](https://github.com/ONT-Avocados/python-template/tree/master/libs) | Python|  合约 libs    |

> 在主网发行合约后如果需要在浏览器中显示，请提交 [申请表](https://docs.google.com/forms/d/e/1FAIpQLSdszQp1BbviS83psIZUZYMKoNkn0e4zcYxrVqM6v5Qbmzby3g/viewform?vc=0&c=0&w=1)
>
> 在测试网发行合约后如果需要在浏览器中显示，请发邮件到 sulingxiao@onchain.com

### 项目

| # | 智能合约                             |        语言      |   描述   |
| -----| ---------------------------------------- | ---------------- | ---------------- |
| 1| [Spokkz](https://github.com/Spuul/spokkz-ontology-smart-contracts/blob/master/contracts/contracts/SpokkzCoin.py) |    Python     |      |
| 2| [Muzika](https://github.com/MuzikaFoundation/ontology-smart-contract/blob/master/contracts/contracts/MuzikaCoin.py) |    Python     |      |
| 3| [Pumpkin](https://github.com/skyinglyh1/CollectPumpkin/blob/master/collectPumpkin.py) |    Python     |      |
