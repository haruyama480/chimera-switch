# chimera-swtich

[浅いキースイッチがなかったので自作することにした](https://qiita.com/haruyama480/items/aa1bcc1d543845d93491) でキメラスイッチを紹介したところ、意外と反響があり、ありがたいことに試してくれる人も出てきました。
しかしキメラスイッチの種類は、既製品のスイッチの種類をNとすると**N^2**の数があります。
それらを個々人が試すのは冗長なので、このレポジトリで結果をまとめ随時更新していこうと思います。

# 目次
- 注意点
- サンプル結果
- 貢献いただける方

# 注意点
キメラスイッチのデメリット
1. ハウジングとステムの相性が悪いと以下が起きます
   - キーが水平方向にぐらつく
   - このぐらつきがチャタリングを起こすことがあります
     - チャタリングはQMKならDebounceを設定するなど、ソフトウェア的に解決できることがあります [参考](https://25keys.com/2022/02/10/debounce/)
   - ずっと電気的に接続されたり、押しても接続されない状態になることがあります
     - これをそれぞれ、fixed-close、fixed-openと呼ぶことにします
2. ステムとハウジングで2つのスイッチが必要なので経済的ではありません

誤差
- サンプル結果は計測手法が統一されていません(計測誤差)
- また、スイッチの個体によっても結果が異なる可能性があります(個体誤差)
- 誤差はあるものと思ってください

# サンプル結果

| ハウジング | ステム | AC\[mm\] | サンプル数 | 発見者 | 備考 |
| :-: | :-: | :-: | :-: | :-: | :- |
| Durock/JWK製のハウジング | [Cherry MX Speed Silver](https://shop.yushakobo.jp/products/cherry-mx) | 0.1-0.4 | >70 | haruyama480 | ハウジングによって打鍵音が異なる。[ultramarine](https://shop.yushakobo.jp/products/4298)のハウジングで、10ヶ月の稼働実績あり |
| [Kailh Midnight Silent V2 Switch](https://shop.yushakobo.jp/products/4270) | [JWK Semi-Silent/Linear](https://shop.yushakobo.jp/products/4665) | 0.3-0.6 | 10 | サリチル酸 | 別名Speed Assassin。[サリチル酸による解説記事](https://salicylic-acid3.hatenablog.com/entry/switches-review-3) |
| [Kailh Midnight Silent V2 Switch](https://shop.yushakobo.jp/products/4270) | [Cherry MX Silent Red (Pink)](https://shop.yushakobo.jp/products/cherry-mx) | 0.4 | 1 | haruyama480 | - |
| [Kailh Speed系](https://shop.yushakobo.jp/products/kailh-speed) | [Cherry MX Speed Silver](https://shop.yushakobo.jp/products/cherry-mx) | 0.7前後 | ? | りゅうせいのたき | (haruyama480)Super Speed系だとfixed-openになってしまいました |


失敗
| ハウジング | ステム | 状態 | 発見者 | 備考 |
| :-: | :-: | :-: | :-: | :-: |
| [Kailh Super Speed系](https://shop.yushakobo.jp/products/4278) | [Cherry MX Speed Silver](https://shop.yushakobo.jp/products/cherry-mx) | fixed-open | haruyama480 | - |



# 貢献いただける方
- PRウェルカムです!
- githubよくわからんって人はissueに結果書いていただけるだけでも!

