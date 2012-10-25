#binary websocketをはじめよう

websocketでメッセージを送るときJavaScriptのオブジェクトをそのまま送ることはできません。
シリアライズしないといけないわけですけど、一番手軽なのはJSONにすることです(`JSON.stringify` 使うだけですから)。
ただ、JSONはファイルサイズや処理コストが大きくなるという問題もあります
。ここでは、websocketでのお絵かきアプリ(最初につくるアプリの定番ですよね？)で

* JSON
* msgpack
* cの構造体的なもの

のそれぞれで実装してみて、どう違うかについて説明してみたいと思います。