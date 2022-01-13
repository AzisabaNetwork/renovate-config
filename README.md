# AzisabaNetwork/renovate-config
[AzisabaNetwork](https://github.com/AzisabaNetwork)で使われている、[renovate](https://github.com/renovatebot/renovate)用のConfigです

## 適用する前に
[default.json](default.json)を変更する際はAzisabaNetwork内のリポジトリのみを考慮するため、外部のいくつかのプロジェクトに適用していた場合、告知なく破壊的な変更が行われる可能性があります。使用する際は十分に理解した上でのご使用をお願いします
## 適用
```json:renovate.json
{
  "extends": [
    "github>AzisabaNetwork/renovate-config"
  ]
}
```

## 機能
* DependencyDashboardを有効化
* Open状態のPRの最大個数を10個に指定
* PRの1時間あたりのRateLimitを解除
* 脆弱性通知のPRに`vulnerabilities`タグを指定
* パッケージ更新のPRに`dependencies`タグを指定
* タイムゾーンを`Asia/Tokyo`に指定
* PRが作成される時間帯を9:00-23:00のみに制限
* [MavenCompilerPlugin](https://maven.apache.org/plugins/maven-compiler-plugin/)を自動マージ

## ライセンス / License
[Apache License 2.0](LICENSE)
