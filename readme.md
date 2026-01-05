# 中古本販売店横断検索

## 概要
このページは検索窓に入力した文字列を以下の中古本販売のサイトのURLクエリに埋め込んで別タブでリンクを開くボタンを提供するサイトです。
「検索」と表示されたボタンを押すと、検索窓に打ち込んだ文字列を{query}として、以下のようにURLに埋め込みます。
そしてできた各URLを`target=_blank`で別タブで開きます。

- Bookoffオンライン: `https://shopping.bookoff.co.jp/search/stock/z/genre/12/keyword/{query}?sort=11&per-page=120`
- Amazon: `https://www.amazon.co.jp/s?k={query}&i=stripbooks`
- ネットオフ: `https://www.netoff.co.jp/cmdtyallsearch/?cat=1002&sort=oldest&stock=1&word={query}`
- 駿河屋: `https://www.suruga-ya.jp/search?category=700&adult_s=2&rankBy=release_date(int):ascending&search_word={query}`
- まんだらけ: `https://order.mandarake.co.jp/order/listPage/list?categoryCode=11&keyword={query}`
- メルカリ: `https://jp.mercari.com/search?category_id=72&status=on_sale&keyword={query}`
- Yahoo! オークション: `https://auctions.yahoo.co.jp/search/search?auccat=21600&p={query}`
- ラクマ: `https://fril.jp/s?transaction=selling&query={query}`

このページはWeb検索で表示されないように、noindexとします。