# 术语

## 关于量化

* 大写字母表示整数 tensor
* 小写字母表示浮点 tensor
* s 表示量化缩放系数
* z 表示量化零点偏移（本文先把问题简单化，只考虑对称量化，不考虑零点偏移）
* bit 表示量化类型位数
* 量化后数据范围 [quant_min, quant_max]
* 对称量化的 s = float_max / quant_max，其中 float_max 由 PTQ 确定，quant_max 由 bit 确定
* 量化（Q）：X = clamp([x/s]; quant_min, quant_max)
* 反量化（DQ）：x' = s * X ~= x
