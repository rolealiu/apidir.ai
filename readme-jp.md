# APIDir.AI - 無料APIでAIの潜在能力を解き放つ
## AIフレンドリーで、完全なAPIドキュメンテーションでAIの理解と使用が容易な無料APIディレクトリ。

[English](./readme.md) / [中文](./readme-chs.md) / [日本語](./readme-jp.md) 

[APIDir.AI](https://apidir.ai) は、AI開発者やテクノロジー愛好家向けの無料のAPI管理プラットフォームを提供する革新的なウェブサイトです。使いやすいインターフェースを提供し、さまざまなAPIを簡単に検索、利用、管理することで、AIの無限の可能性を引き出すことを目指しています。さらに、各APIには「AIフレンドリー」のラベルを付けているため、理解しやすく、シームレスにプロジェクトに統合できるAPIを簡単に見つけることができます。

🤖 このプロジェクトの95%は、AIによって開発、データ収集、分析されています！

👍 素晴らしい開発者の方々が提供してくださったAPIに感謝します！

## ⭐ 主な特徴

- **無料のAPIディレクトリ**：apidir.aiは幅広い機能をカバーする無料のAPIを幅広く提供し、AIプロジェクトを豊かに多様化します。
- **AIフレンドリー**：各APIは「AIフレンドリー」として丁寧にラベル付けされており、理解しやすく統合しやすいAPIを簡単に見つけることができます。
- **リアルタイムモニタリング**：各APIのパフォーマンスを継続的に監視し、安定性と信頼性を保証し、プロジェクトが中断することなくスムーズに動作するようにしています。

## 👍 apidir.aiの利点

- **時間の節約**：apidir.aiのスマートな検索とAIフレンドリーなラベルを活用して、膨大なAPIからプロジェクトに適したAPIを迅速に見つけることができ、貴重な時間を節約できます。
- **ハードルの低下**：詳細なAPIドキュメントと使用方法を提供することで、学習のハードルを低くし、統合のプロセスを簡素化しています。


## 🚀 早速始めましょう

ウェブサイト：👉 [https://apidir.ai](https://apidir.ai) 👈

APIを探索する：👉 [https://explore.apidir.ai](https://explore.apidir.ai) 

## 📚 APIリスト

🦾 APIDir.AIは、プログラムやAIと簡単に統合できる無料で非認証のAPIを提供し、第三者のAPI認証の必要性をなくします。

| API                      | Request Method | Path                        | Query Parameters                                     | Description                        |
|-------------------------|--------------------|-----------------------------|------------------------------------------------------|---------------------------|
| 検索API                       | GET              | https://get.apidir.ai    | id：API ID、特定のAPIを正確に見つけるためのID </br></br> language：APIデータの言語 </br></br> status：APIの実行状態 </br></br> topics：APIトピック </br></br> price：APIの料金設定 </br></br> ai_friendly：AIフレンドリーかどうか、AIの理解と使用を容易にするため  | APIの詳細情報を取得します。フィルタリング用の複数のパラメータをサポートしています。</br></br> 'id'を渡すと、詳細なドキュメンテーション（利用可能な場合）を持つ単一のAPIが返されます。 |
| APIトピック取得          | GET              | https://topics.apidir.ai  | -language                            | 指定された言語に基づいてAPIトピックを取得します。         |

## ⭐️ Pythonコード例

```python
import requests

# get.apidir.ai APIを使用してAPIの詳細情報を取得する
def get_api_details(api_id):
    url = f'https://get.apidir.ai/?id={api_id}'
    response = requests.get(url)
    data = response.json()
    return data

# コード例 - ID 1のAPIの情報を取得する
api_details = get_api_details('1')
print(api_details)

# topics.apidir.ai APIを使用して特定の言語のAPIトピックを取得する
def get_api_topics(language):
    url = f'https://topics.apidir.ai/?language={language}'
    response = requests.get(url)
    data = response.json()
    return data

# コード例 - 英語言語のAPIトピックを取得する
api_topics = get_api_topics('eng')
print(api_topics)
```

## ⭐️ JavaScriptコード例

```javascript
const fetch = require('node-fetch');

// get.apidir.ai APIを使用してAPIの詳細情報を取得する
async function getApiDetails(apiId) {
  const url = `https://get.apidir.ai/?id=${apiId}`;
  const response = await fetch(url);
  const data = await response.json();
