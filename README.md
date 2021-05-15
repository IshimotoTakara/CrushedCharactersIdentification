# CrushedCharactersIdentification
日本で古くから使われていた「くずし字」を識別しよう．くずし字のクラスは10種類あるため，多クラス分類モデルを作成します．

## ProbSpace URL
https://prob.space/competitions/kuzushiji-mnist

## データの説明
[kmnist-test-imgs.npz](https://prob.space/competitions/kuzushiji-mnist/data/34)

[kmnist-train-labels.npz](https://prob.space/competitions/kuzushiji-mnist/data/35)

[kmnist-train-imgs.npz](https://prob.space/competitions/kuzushiji-mnist/data/36)

KMNIST(Kuzushiji-MNIST)は，日本語の「くずし字」のデータセットです．
国文学研究資料館（National Institute of Japanese Literature/ NIJL）が作成し，人文学オープンデータ共同利用センター（Center for Open Data in the Humanities / CODH）が公開しています．

各くずし字の画像データは，28×28の大きさで，グレースケールの画像データです．
くずし字の種類は，10種類で，お(o)，き(ki)，す(su)，つ(tsu)，な(na)，は(ha)，ま(ma)，や(ya)，れ(re)，を(wo)の10文字が含まれています．
データ数は，訓練データが60000枚，テストデータが10000枚の計70000枚です．

より詳細については，以下を参照してください．

https://arxiv.org/abs/1812.01718

## 評価方法
メトリック
このコンペティションは，accuracyによって評価されます．つまり，正解した予測と，全ての予測の比率です．
kmnist-test-imgs.npzに対して作成したモデルで予測を行い，その結果を次のフォーマットのcsvファイルで提出してください．

## 提出ファイルのフォーマット
![スクリーンショット 2021-05-14 7 08 26](https://user-images.githubusercontent.com/57268381/118193737-305c4180-b483-11eb-802e-7e689c559623.png)
