# Qcom fix band NV setting
online calculate: https://dustinchen26.github.io/fix_band

## Description
```
● fix NR only => NV#80000 設 64，NV#10 設 71
● fix NR band => NV#74087 NR band preference
    要fix那些NR band，就將底下按鈕對應bit設為1，bits_1_64，bits_65_128，bits_129_192，bits_193_256，bits_257_320
    ex: fix N41 底下按鈕 41 的bit舉為1 => 計算出 1099511627776 , 填到 bits_1_64
    ex: fix N48 底下按鈕 48 的bit舉為1 => 計算出 140737488355328 , 填到 bits_1_64
    ex: fix N78 =>(78-64=14)底下按鈕 14 的bit舉為1 => 計算出 8192 , 填到 bits_65_128
    ex: fix N79 =>(79-64=15)底下按鈕 15 的bit舉為1 => 計算出 16384 , 填到 bits_65_128
```