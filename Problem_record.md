# Practical Reinforcement Learning Using Python
這是Udemy上課筆記

8堂實作課
## Atari


### 問題紀錄
1. 一開始import gym時報錯, 查詢後發現是python 3.6和gym 0.20.0版本問題
* 解決方法有2:
    1. python 升到3.7
    2. gym 降板到0.15.7

* 降版作法:
``` cmd
pip install gym==0.15.7

```
* 參考:https://stackoverflow.com/questions/69520829/openai-gym-attributeerror-module-contextlib-has-no-attribute-nullcontext

2. 複雜的環境問題QQ

https://github.com/openai/gym/issues/1726
弄了老半天, 降板到 gym0.19.0
並重新install下面幾個套件
```
pip install gym[atari]
pip install autorom[accept-rom-license]
```
果然環境最麻煩


## 參考資料
https://hackmd.io/@shaoeChen/Bywb8YLKS/https%3A%2F%2Fhackmd.io%2F%40shaoeChen%2FHkH2hSKuS