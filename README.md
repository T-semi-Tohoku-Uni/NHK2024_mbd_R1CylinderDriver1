# NHK2024_mbd_R1CylinderDriver1
R1のエアシリンダドライバその1
[参考](https://t-semi.esa.io/posts/57)

このドライバの担当は以下の通り
- アーム上下
- 苗ハンド1開閉
- 苗ハンド2開閉

**苗ハンドの展開はシリンダドライバその2**が担当

# ピン入出力
## 入力
無し
## 出力
![image](https://github.com/T-semi-Tohoku-Uni/NHK2024_mbd_R1CylinderDriver1/assets/43599353/16cb55ed-d136-4c9f-afee-7e2d2d6cc61b)
添付画像のJP1~JP6にそれぞれ出力

JP1: アーム上

JP2: アーム下

JP3: ハンド1開く

JP4: ハンド1閉じる

JP5: ハンド2開く

JP6: ハンド2閉じる



# CAN入出力
## 入力
### CANID_ARM_ELEVATOR 0x104
Data[0]が0で下
Data[0]が1で上
### CANID_HAND1 0x105 
Data[0]が0で開く
Data[0]が1で閉じる
### CANID_HAND2 0X106 
Data[0]が0で開く
Data[0]が1で閉じる
