# page設定
description:{
    - objective: ユーザーフレンドリーで視覚的に魅力的なもつ鍋屋さんのウェブサイトを開発し、顧客を惹きつけて情報を提供する。
    - TASK: ホームページのレイアウト設計、メニュー機能の含有、場所の詳細、オンライン予約システムの導入。
}
input:{
    - 変数: レストラン名、メニュー項目、価格
    - 固定値: レストランの場所、連絡先情報
    - etc: 料理の画像、レストランの内装
}
functions:{
    - TOP: 店舗の文化的背景や人気の秘訣などのライティングと、もつ鍋や店主の画像を配置してデザインする。
    - Header:{
        - global navi: 選択可能なグローバルナビを実装する。{
            - 項目は[1.トップページ, 2.メニュー一覧, 3.店舗案内]
            - 全てにリンクを用意し、ページに遷移できるようにする。
        }
    }
    - main contents{
        - Menu Display: メニュー項目と価格を表示し、チェックボックス注文とConfirm buttonを設置する{
            - Confirm buttonのリンク先{
                - 予約確定の内容を顧客に知らせる、アナウンスページを用意する
                }
            }
        - Reservation System: 顧客がオンラインで簡単に予約できるシステムを設計・実装。
        - Location Information: 地図とアクセス方法と店舗の内装を含む詳細情報の提供。[GoogleMap]
    }
    - footer:{
        - 店舗名と店舗のロゴ、電話番号を配置する。
    }
}
restrictions:{
    - 言語は「全て日本語を用いる」こと。
    - 素材は全て生成すること。
    - カラーは食欲をそそる色や、もつ鍋を連想させる色使いをする。
    - 使用するメインカラーは3色までとする。
}
Dir:{
TOP(1.トップページ)/
    └── Header/
    └── main contents/
        └── Menu Display(2.メニュー一覧), Reservation System, Confirm button/
            └── 予約確定内容の表示ページ/
        └── Location Information(3.店舗案内)/
    └── footer/
}