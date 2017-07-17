XGBoost fizzbuzz
=========

XGBoostのフィズバズです

# やろうと思った動機
DeepLearningならばFizzBuzzの３の倍数と５の倍数と１５の倍数の時に、特定の動作をするというルールを獲得することは容易なのですが、他の機械学習アルゴリズムはどうでしょうか  

XGBoostはその決定木の性質と、勾配ブースティングの学習アルゴリズムからルールを獲得することは難しくないんじゃないかと思いました  

ただ、数値として扱ってしまうと、かなり厄介で、連続する値が大きい小さいなどで内部的に判別するのは容易ではありません  

## 具体的な数値データの取り扱い

数字を文字表現として皆して、各桁の数字を一つの特徴量として扱います  
