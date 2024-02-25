<!--
title:   Google Cloud Storage から CSV ファイルを Looker Studio にアップロードする
tags:    LookerStudio,googlecloud
id:      5ab5a008662a6d23187d
private: false
-->
# 概要

Google Cloud Storage から CSV ファイルを Looker Studio にアップロードする方法について記載します。

# この記事によって出来ること

- Looker Studio に CSVデータをアップロードできる
- Google Cloud Storage から Looker Studio にデータをアップロードできる

# 補足

Looker Studio にデータをアップロードする方法には複数ありますが、本記事では Google Cloud Storage を使用する方法について記載します。


# Google Cloud Storage から CSV ファイルを Looker Studio にアップロードする流れ

以下の手順で行います。

1. データを Google Cloud Storage にアップロードする
1. データを Google Cloud Storage から Looker Studio にアップロードする


## データを Google Cloud Storage にアップロードする

Google Cloud コンソール等を通じて、Storage バケットを作成し、データをアップロードします。
![Screen Shot 2022-12-17 at 16.06.17.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/44715215-f6fa-b087-b225-7176c08d3a94.png)

Looker Studio へアップロードする際、データファイルのパスが必要になるため、確認しておきます。
![Screen Shot 2022-12-17 at 16.08.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/d2153f02-f1ca-8853-433c-3183fd2c44a1.png)

Looker Studio で Google Cloud Storage からデータをアップロードする際、以下のようにデータファイルのパスを指定する必要があります。

{Bucket_name}/{Folder_name}/{File_name}

本記事の場合は、"bucket_20221217/dam.csv" となります。


## データを Google Cloud Storage から Looker Studio にアップロードする

Looker Studio にて、データソースを作成します。
具体的な手順としては、左上の「作成ボタン」をクリックし、「データソース」を選択します。

![Screen Shot 2022-12-17 at 16.12.36.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/c9248de2-f9ea-baac-48ad-109329e7028c.png)

どこからデータをアップロードするかを指定するため、「コネクタ選択画面」にて「Google Cloud Storage」を選択します。

![Screen Shot 2022-12-17 at 16.12.44.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/91dfe120-5846-1e77-9487-da89928c3297.png)

「Looker Studioにデータへのアクセス権を許可してください」と表示されたら、「承認」ボタンをクリックします。
![Screen Shot 2022-12-17 at 16.12.55.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/a8481991-3a12-7e58-624f-43d5ca6fb93b.png)

アップロードする対象のファイルを指定するため、「GCS ターゲットパスの File Path」に、先程確認したデータファイルのパスを指定して、「接続」ボタンをクリックします。

![Screen Shot 2022-12-17 at 16.29.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/900dd8bd-7ddd-3986-e374-33980ebd2b88.png)

アップロードが完了すると、データの項目一覧が表示されます。
![Screen Shot 2022-12-17 at 16.30.35.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/75359997-f940-cf0b-9df1-3cf1b57cbdaa.png)

Google Cloud Storage からデータをアップロードすると、データセット名が「Google Cloud Storage」となるので、後日利用しやすいようにデータセット名を変更しておきます。

具体的な手順は、
左上の「Looker Studio」アイコンをクリックしてホーム画面を表示します。
![Screen Shot 2022-12-17 at 16.34.17.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/e7a24208-063f-e725-d64a-1ed283dbf7fa.png)

対象のデータセットの右端にある「３つのドット（︙）」をクリックし、「名前を変更」を選択し名前を変更します。
![Screen Shot 2022-12-17 at 16.38.18.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/86f919ae-6b67-d30f-ca28-aeb3eafd4884.png)

![Screen Shot 2022-12-17 at 16.39.11.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/2a91bda4-650f-ebc7-6e96-86a838d5d177.png)

以上です。