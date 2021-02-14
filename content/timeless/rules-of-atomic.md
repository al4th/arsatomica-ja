+++
title = "アトミックのルール"
date = 2017-08-19T11:14:36+02:00
description = "An explanation of the rules of atomic chess for the beginner."

slug = "atomic-rules"
categories = ["reference"]
tags = ["rules", "beginner"]
type = "timeless"
series = []
+++

アトミックの世界へようこそ！　アトミックのルールは[リチェスのサイト](https://lichess.org/variant/atomic)でも説明されているが、このページについて知っているプレイヤーは少ないようだ。それに初心者のうちは、チェックに関するルールを明確に理解するのは難しいように見える。ここでは全ルールについて、それが何を意味しているのかを実例を交えながら説明している。<!--Welcome to atomic chess! The variant rules are also explained at [their own page on lichess](https://lichess.org/variant/atomic), but not many people know about that page, and the rules about checks may seem unclear at first. Presented here are all the rules with examples to show you what it all means.-->

以下で示した手順を[リチェス上で直接](https://lichess.org/study/Y9Aj5y3j/)見て、実際に駒を動かしてみよう！

## アトミックの目的 ##
アトミックチェスでは、相手のキングをチェックメイトにするか、爆破して盤上から消せば勝ちになる。ただし爆破の場合、自分のキングが盤上に残っていなければならない。<!--In atomic chess, you win by checkmating or exploding the enemy king, with your king remaining on the board.-->

## テイク ##

アトミックが普通のチェスと大きく異なる点は、テイクの破壊力である。テイクが起きると:<!--The most striking feature of atomic chess is the destructive power of captures. When a capture is played:-->

1. 取られたピースだけでなく、取った側のピースも亡くなる (そして盤上からなくなる)。
2. そして、取られた駒を中心とした3マス×3マスの正方形をイメージしてほしい。この正方形の中にあるポーン以外のピースは全て亡くなる。

ここに示した例では、白の5手目に応じて、黒番が3つの異なるパターンのテイクを行っている。それぞれのパターンでどの駒が亡くなるのかを説明している。<!--This example shows 3 different captures by black depending on white's 5th move, and explains which pieces die in each capture.-->

{{< lichess-embed src="https://lichess.org/study/Y9Aj5y3j/gIvsi0CZ#4" >}}


ほとんどの対局は、相手からの脅威をかわしながらテイクで駒得することを中心にして進んでいく。相手キングを消滅させて勝利することもある！　実際のところ、__相手キングを爆破する__\*やり方で対局が終わるというのはかなりよくあることだ。<!--Much of the game revolves around winning material (or the enemy king!) with captures while dodging your opponent's threats. In fact, __exploding the enemy king__\* is a fairly common way for the game to end.-->

このことは、お互いのキングはどの駒もテイクできないということも意味している。テイクしたときに自殺となってしまうからである。自分のキングで相手のキングを取ることすらもできない。<!--This also means that kings cannot capture anything, as they would die in the process. They can't even capture each other!-->

\*補足: もっと正確に言うなら、"相手キングを爆破する"というよりは"相手キングに隣接した駒の一つをテイクし、爆発に巻き込む"である。しかし"キングを爆破する"の方がはるかに言いやすいので、このような言い方をしている。<!--\*Pedantic note: Phrased more accurately, it would be "capturing a piece next to the enemy king, catching it in the explosion", but "exploding the king" is much easier to say.-->

### 例外：アンパッサンテイク ###
アンパッサンの場合、テイクで起きることの2ステップ目における爆心地は、テイクされたポーンのいた位置ではなく、テイクされたポーンが通過した位置（テイクしたポーンが動いた先）になる。<!--In the case of en passant, the 3x3 square in step 2 is not centred on the captured pawn, but on the square it bypassed (the square the capturing pawn moved to).-->

{{< lichess-embed src="https://lichess.org/study/Y9Aj5y3j/VEOjghJD#5" >}}


## 禁止手 ##

アトミックの目的は、自分のキングを生かしたまま、相手のキングをチェックメイトにしたり爆破することである。したがって自分のキングの隣にある駒をテイクするといった、自分のキングが爆発に巻き込まれる着手は禁止されている。自分のキングがチェックされた状態のまま相手の手番になるような着手も禁止されている（訳注：チェックの放置や、相手の駒をテイクすることでチェックとなってしまう場合が該当する）。ただし相手キングを爆破する着手の場合は、このルールが適用されない。
2つ目がトリッキーであり、慣れるまでに少し時間がかかる。私は"キングの爆破 \> チェック"として覚えるようにしている。<!--The goal in atomic chess is to checkmate or explode the enemy king while keeping your king alive. It is therefore illegal to play a move that explodes your own king, such as capturing a piece next to your king. It is also illegal to play a move that leaves your own king in check, unless you immediately explode the opponent's king.This second part is tricky, and takes a while to get used to. I remember it as "King explosion \> check".-->

下に例を示す。黒番は9...Qxc7とすると、キングがチェックされた状態のまま白番を迎えるため、このような手は指せない。<!--In this example, black cannot leave the king in check with 9...Qxc7.-->

{{< lichess-embed src="https://lichess.org/study/Y9Aj5y3j/AVDvSCCW#16" >}}

一方下に示した例では、黒番は自分のキングにかけられたチェックを無視して4...Bxd2#と指すことができ、白のキングを爆破して勝利することができる。<!--Whereas in this example, black can ignore the check on his king and win by exploding the enemy king with 4...Bxd2#.-->

{{< lichess-embed src="https://lichess.org/study/Y9Aj5y3j/DluXatzP#7" >}}


## キングの隣接 ##
キングがどの駒もテイクできないので、キングで相手のキングをテイクすることもできない。だからアトミックでは、キング同士が隣同士になるのは全くおかしなことではない。さらに言えば、キング同士が隣り合っている限りはどちらのキングもチェックを免除される。というのも、どちらかのキングがテイクされる手は必ずテイクした側のキングを爆破する手になってしまうため、手出しできない状態となっている。このような性質のために、相手のキングに隣接しているが自分のキングに隣接していないピースを爆破することで勝てる、非常に興味深いエンドゲームがいくつか存在する。<!--Because kings cannot capture anything, they also cannot capture each other. So It is perfectly normal in atomic chess for the kings to be next to each other. Furthermore, while they are adjacent, the kings are immune to checks (since each one can't be captured without exploding the other king, they are not under attack in that sense.) This can make for some very interesting endgames, where the winning method is to explode a piece next to your opponent's king but not next to yours.-->

{{< lichess-embed src="https://lichess.org/study/Y9Aj5y3j/8gu21f1H#0" >}}


## キャッスリング ##
キャッスリングは普通のチェスと同じように機能する。チェックされている限りはキャッスリングできないし、キングの移動中のマスや移動先のマスが攻撃を受けているとキャッスリングはできない。しかし、相手キングに隣接しているマスであれば、自分のキングは攻撃を受けることなく安全に通過したり到達したりすることができる。つまり互いのキングが隣接している間はチェックが無効化されるのである。<!--Castling works the same as in normal chess. You cannot castle while in check, through check, or into check. The king can however safely pass through or reach any square adjacent to the enemy king; adjacent kings nullify checks.-->

{{< lichess-embed src="https://lichess.org/study/Y9Aj5y3j/tV1rwQvI#0" >}}

---------

駒を動かしながらルールを確認するために、下にアトミックの短い対局例を示した。<!--To see the rules in action, here's a short example game of atomic.-->

{{< lichess-embed src="https://lichess.org/study/Y9Aj5y3j/bGNv3Ppy#0" >}}

ここまでがアトミックのルールである。これでもう相手がチェックを無視したりとか、キングを自分のキングに隣接させてきたりしても驚くことはない。対局の準備は整った！<!--Those are the rules of atomic chess. Now you won't be surprised anymore by your opponent ignoring check or having adjacent kings, and you're ready to go out and play!-->