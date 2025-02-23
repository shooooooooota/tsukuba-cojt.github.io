---
layout: root
tags: results
title: サークル検索サービス
year: 2022
term: spring
icon: "/image/results/2022/circle/icon.png"
cover: "/image/results/2022/circle/cover_new.png"
description: サークルを簡単に検索できるサービス
repositories: ["https://github.com/shunsuke0424/circle-kun"]
students: [202011453, 202213594]
---

{% include "results_header.njk" %}

## 参加学生

{% student_by_id students_data, students %}

## 作品紹介

# サークルクル君

## 1.想定利用者と利用目的(Who)

### ①想定利用者：新1年生

#### 利用状況や利用目的

- 筑波大学のサークルに関して、何も知らない
- 運動系のサークルに入りたい
- きつくなく、ゆるいサークルを知りたい
- 「筑波大学 サークル一覧」と検索したところ、このサイトが検索順位 1 位だったのでクリックした

### ②想定利用者：3編生

#### 利用状況や利用目的

- 3年次編入生
- 3年生なので、サークルに入るか悩んでいる
- 編入下ばかりで、知り合いも少ないので、交友関係を広めたいと思っている
- twitterのTLで筑波大学新歓 Web のツイートが流れてきて、そこからこのサイトに飛んだ

<br>

## 2.既存システムの問題点と改善策

現在、筑波大学サークル一覧検索システムとして、[筑波大学 新歓 Web](https://www.stb.tsukuba.ac.jp/~shinkan-web/ "筑波大学 新歓 Web")が挙げられる。以下に筑波大学新歓Webの画面例を示す。

<img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/%E7%AD%91%E6%B3%A2%E5%A4%A7%E5%AD%A6%E6%96%B0%E6%AD%93web_1.png" width="525" height="300">

<img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/%E7%AD%91%E6%B3%A2%E5%A4%A7%E5%AD%A6%E6%96%B0%E6%AD%93web_2.png" width="525" height="300">

<img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/%E7%AD%91%E6%B3%A2%E5%A4%A7%E5%AD%A6%E6%96%B0%E6%AD%93web_3.png" width="525" height="300">

### 2.1既存システムの問題点

1. ある程度の目星がついていれば、キーワード検索が可能だが、そうでなければ団体一覧からしか探すしかない
2. 複数条件の検索ができない
3. カテゴリー分けされている訳ではないので、目的のサークルを探すのが難しい
   (体育・芸術・文科系・その他といった大きな 4 つのカテゴリーは存在するが、これでは
   検索ニーズを満たすのは難しい)
4. 検索する際、詳細画面のすべての文字に対して検索をかけているので、不適切な結果が
   返ってくる可能性がある。
5. 一覧ページから分かるサークル情報が少ない

### 2.2改善策

1. 検索KWだけでなく、開催場所や頻度などを検索条件に追加
2. カテゴリー大(体育、文化、芸術)を選択後、プルダウンでカテゴリー小を表示
3. 一覧
   (体育・芸術・文科系・その他といった大きな 4 つのカテゴリーは存在するが、これでは
   検索ニーズを満たすのは難しい)
4. 一覧ページにもサークルの名前意外の情報を盛り込む
   <br>

## 機能・利用の流れ

1. 分野を選択
   KWや分野(体育、文化、芸術)だけでなく、活動場所、活動日時でも検索が可能。なお、今回は分野を用いた際の検索例を示す。
2. カテゴリを選択
   入力したカテゴリ(大)に応じて、カテゴリ(小)では、カテゴリ(大)に入っている全サークルがプルダウンで提示される。その中で興味のあるキーワードを選択。<br/>
   <img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/search_category.png" width="525" height="300">

## 工夫した点

1. カテゴリを追加し、全サークルがカテゴリのどこかに分類されるようにした。
   そうすることで、「こんなサークル知らなかった！」という発見を促すことができる。
   興味のある・名称を知っているサークル検索以外のニーズも満たせると考える
   以下に運動カテゴリを選んだ時に、表示されるカテゴリ(小)を示す。<br/>
   <img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/ex_ath_category.png" width="450" height="470">

## 実際の画面

<img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/image_1.png" width="665" height="400">
<img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/image_2.png" width="665" height="450">
<img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/image_3.png" width="665" height="450">
<img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/image_4.png" width="665" height="450">
<img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/image_5.png" width="665" height="450">
<img src="https://raw.githubusercontent.com/tsukuba-cojt/tsukuba-cojt.github.io/main/src/image/results/2022/circle/image_6.png" width="665" height="450">

{% include "related_results.njk" %}
