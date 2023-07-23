---
title: "Note Block Studioで10 ticks以上にできない場合の対処法"
date: 2023-07-24T04:07:32+09:00
draft: false
categories: [Minecraft]
---

地味に最初の記事ですね。今回は、Minecraft Note Block Studioで曲のtickを10 ticks以上にできない場合の対処法を紹介します。備忘録です。

## 環境

まず環境を合わせてください。バージョンは3.10.0です。

{{< figure src="/img/note_block_studio_version.png" alt="バージョン表示" >}}

## どんな内容？

{{< figure src="/img/note_block_studio_10_ticks.png" alt="10 ticks" >}}

テンポが速い曲だと最大値である10 ticks per secondでは速度が足りないことがあります。そういう場合は、音を全部選択して圧縮することで一音の長さを半分にすることができます。

やり方を以下に示します。まず最初に、全ての音符ブロックをCtrl+Aを使用して選択してください。

{{< figure src="/img/note_block_studio_all_selected.png" alt="全てを選択" >}}

その次に、Editタブを開いてCompress selectionをクリックしてください。これにより音符すべてが圧縮されます。

{{< figure src="/img/note_block_studio_compress_selections.png" alt="Edit" >}}

10 ticksの曲を一回圧縮した場合、速さが二倍になるので実質20 ticksと同じ聞え方になります。ただ、速さ的に無理がある場合はこの方法を使うと音符ブロックがいくつか消えたりすることがありますのでご注意ください。

また、もう一回圧縮するとさらに早くすることもできます。ただ圧縮をしすぎるといくつかの音ブロックが消えるかもしれません。

## まとめ

この備忘録は速い曲を音ブロック化するときはほぼ必須になると思います。

一応言っておきますが、音ブロックをschematicとして出力する場合はマイクラの仕様上この操作をしないと元のスピードを再現できません。しかし、データパックとして出力する場合はこの限りではありません。データパックとして利用できる場合は元のticksのままデータパックとして出力して利用することをお勧めします。