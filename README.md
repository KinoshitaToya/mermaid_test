# 課題
Mermaidを触ってみよう

マークダウンファイルを編集して、Mermaidで図を描いてみよう

# 取り組み方
* 本プロジェクトをforkしてください。
* README.mdを編集して、Mermaidを使いこなしてください
* できたらプルリクエストを出します

# 課題項目
## 流れ図
### 条件
- 開始と終了ノードをつける
- 条件分岐を組み込む
- 5ノード以上
- カッコいいほど高得点

## 解答
```mermaid
flowchart LR;
  開始 --> 分岐 --> True
  分岐 --> False
  True --> 終了
  False --> 終了
  
```

## シーケンス図
### 条件
- 3人以上
- メッセージをやり取りしない人がいないように
- 自己呼び出しを含むこと
- カッコいいほど高得点

## 解答
```mermaid
sequenceDiagram
    actor 統也
    actor 太郎
    actor 花子
    太郎->>花子: この問題解けた？
    activate 花子
    花子-->>太郎: ごめん。まだなんだ。
    deactivate 花子
    統也->>太郎: その問題なら解けたよ！
    activate 太郎
    太郎-->>統也: 教えて！
    deactivate 太郎
    activate 統也
    統也-->>太郎: いいよ！
    deactivate 統也
    花子->>統也: 私にも教えて！
    activate 統也
    統也-->>花子: もちろん！
    deactivate 統也
```

## クラス図

### 条件
- 3つ以上
- 汎化と集約を含むこと
- カッコいいほど高得点

## 解答
```mermaid
classDiagram
    キャラクター o-- アイテム
```
