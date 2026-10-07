# Liquid d1：テキストと画像による英日QAの探索的評価

Belebeleの短文4択QAを使い、本文をテキスト・通常画像・分割画像・縮小画像で渡したときの正答率、入力トークン、応答時間を比較した技術報告です。

**結論：標準運用はテキストA。** 通常画像B/Cは正解数を維持した一方、入力が増加しました。D40は英語14/14正解・入力7.27%減でこの小集合では有望、日本語11/14正解・入力22.54%減で精度優先では不採用です。実請求総額は未確認です。

- [論文を読む（日本語Markdown）](paper/REPORT_JA.md)
- [論文PDF](paper/REPORT_JA.pdf)
- [実際にモデルへ送信した画像10点](images/main/)

画像は実送信PNGそのもので、説明用の再生成や公開時の再加工はしていません。少数例の探索的結果であり、一般的な性能や速度改善を証明するものではありません。

Belebele由来テキスト・派生画像はFacebook Research / Bandarkar et al.の[Belebele](https://github.com/facebookresearch/belebele)評価データに基づき、[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)で提供します。描画・上下分割・縮小という変更と、元記事の寄稿者への帰属は論文付録に記載しています。

Research report © repository owner

参考：[Liquid AI d1](https://www.liquid.ai/blog/d1-decision-model) · [Belebele論文](https://aclanthology.org/2024.acl-long.44/) · [DeepSeek-OCR](https://arxiv.org/abs/2510.18234) · [Jev](https://arxiv.org/abs/2609.37647)
