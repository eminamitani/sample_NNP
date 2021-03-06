# シンプルなニューラルネットワークポテンシャル

このリポジトリは、ニューラルネットワークポテンシャル（NNP）の仕組みを試して見るための簡単なサンプルを入れてあります。
64原子系の結晶Siの第一原理MD計算から取得したデータが`sample50.xyz`です。
このファイルを処理して、対称性関数と呼ばれるニューラルネットワークへの入力を作るプログラムが
`make_desc.ipynb`, `make_desc_large.ipynb`です。
後者は対称性関数の計算につかうハイパーパラメータを[論文](https://iopscience.iop.org/article/10.7567/1882-0786/ab36bc/meta)
に合わせてあります。

エネルギーの予想ができるNNPの最もシンプルなバージョンが`SimpleNNP.ipynb`です。
パラメータをチューニングしたものを使い、GPUで早く動かせるようにしてあるものが`SimpleNNP2.ipynb`です。

これらのサンプルを動かすためには、`ase, dscribe, pytorch`のパッケージ必要です。
