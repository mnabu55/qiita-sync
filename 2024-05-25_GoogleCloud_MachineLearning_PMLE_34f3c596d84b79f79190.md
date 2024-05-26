<!--
title:   Google Cloud 認定 Professional Machine Learning Engineer資格認定に向けての取り組み
tags:    GoogleCloud,MachineLearning,PMLE
id:      34f3c596d84b79f79190
private: false
-->
# 要約

この度、**Google Cloud 認定 Professional Machine Learning Engineer** 試験に合格しましたので、その過程で得られた知見を整理しました。

**この記事で伝えたいこと**

- **生成AI時代の必須スキル、機械学習を学ぶことの重要性** ChatGPTなど、私たちの生活を変える生成AI。その裏側にある機械学習を学ぶことで、AIを使いこなし、新しいチャンスを掴むことができます
- **機械学習の習得・スキルの可視化を目指すなら、PMLE認定資格はおすすめ** Google Cloudが提供する Professional Machine Learning Engineer(PMLE)認定資格は、機械学習エンジニアとしてのスキルを証明し、キャリアアップに役立ちます

![Screenshot 2024-05-25 at 18.48.51.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/903417d8-917e-4778-57eb-feacbbc46e2c.png)


# 生成AI時代の必須スキル 機械学習

近年急速に利用が進んでいるChatGPTは、「機械学習」の進化が生み出した「生成AI」と呼ばれる技術の一例であり、生成AIは、私たちの生活やビジネスを大きく変えようとしています。

**機械学習を学ぶことは、この変化の波に乗り遅れないための第一歩です。**

機械学習を理解することで、

- **生成AIの仕組みを深く理解し、より効果的に活用できるようになります。**
- **AI技術を活用した新しいビジネスチャンスを見つけ出すことができます。**
- **AI時代に求められる人材としての価値を高めることができます。**


# Google認定資格 「Google Cloud - Professional Machine Learning Engineer(PMLE) 」とは

Google Cloud Platform (GCP) 上での機械学習ソリューションの設計、構築、運用に関する専門知識とスキルを認定するものです。試験対策を通じて、機械学習モデルの開発、データパイプラインの構築、MLOpsの実践、分散学習など、機械学習について、本番環境での運用まで含めた幅広い知識を深めることができます。

## 試験概要（試験形式、実施方法等）について
[Google Cloud Certification - Professional Machine Learning Engineer](https://cloud.google.com/learn/certification/machine-learning-engineer)

## 試験の評価項目について
https://cloud.google.com/learn/certification/guides/machine-learning-engineer


# 受験にむけての取り組み

学習に使ったリソースは、以下の２つです。期間は約４ヶ月かけて準備しました。

- 基礎教材
- 過去問題

## 基礎教材
Google Skill Boostの [Machine Learning Engineer Learning Path](https://www.cloudskillsboost.google/paths/17)で機械学習の基礎から応用まで体系的に学習しました。

なお、Google Skill Boostsのコースは教材の量が比較的多かったため、時間の都合で私は以下を学習した段階で過去問を解き、受験に挑みました。

コースActivity番号: 01(A Tour of Google Cloud Hands-on Labs) - 07, 10 - 13

## 過去問試験

試験合格に向けて、どのような問題が出題されるか傾向を把握するため、過去問をできるだけ多く解きました。教材には以下を使用しました。

- [Google 模擬試験](https://docs.google.com/forms/d/e/1FAIpQLSeYmkCANE81qSBqLW0g2X7RoskBX9yGYQu-m1TtsjMvHabGqg/viewform)
	無料であるが問題数が約20問程度なので、追加で下記のUdemyのコースを受講しました

- Udemy 過去問試験問題 [Google Professional Machine Learning Certification Exam 2024](https://www.udemy.com/course/google-professional-machine-learning-certification-exam-2023/)


# 資格勉強を通じて学んだこと

- アルゴリズムの検討や MLモデルの作成は、MLプロジェクト全体作業の約5%程度に過ぎず、MLプロジェクトは「モデルを作り、学習して予測」で終わりではない
- MLプロジェクトにおいて本質的に重要なことは、継続して運用すること。そのためには、運用をある程度自動化することが不可欠。MLOpsは重要なキーワード
- データ収集から予測までのパイプラインだけでなく、再学習 Continuous Training(CT)を行うパイプラインも重要
- トレーニングおよび本番環境におけるパイプライン構築において、Vertex AIは非常に有用なMLサービス
- 学習に関して、生成AI時代には分散学習の知識やスキルも必要になる
- 本番環境における End-to-End のパイプラインや分散学習の実装の必要性を考慮すると、 TFX(TensorFlow eXtended) や KubeFlow の習得を検討する価値はある


# 今後の展望
[Parul Gautamさんのツイート](https://twitter.com/Parul_Gautam7/status/1748935248874733797)にて、Data Engineer, Data Scientist, Data Analyst, Machine Learning Engineer の違いについて述べられています。
今回の認定資格学習を経て、私は、データ分析、データエンジニアリング、データサイエンスに加え、機械学習分野の知識やスキルを習得することができました。
今後は、これまでに得た知識やスキルをもとに、TFXや分散学習の実装、生成AIなどより発展的な領域にチャレンジしていきます。

![role.jpeg](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/55793/91584250-402c-5547-87a1-78551d916b31.jpeg)