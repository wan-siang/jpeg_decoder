# jpeg_decoder
* ref: https://github.com/yasoob/Baseline-JPEG-Decoder
* 彌補了yasoob的不足
  * 只能做到img resolution為8的倍數 -> 已可以做到任何解析度
  * 只能做到採樣率為 Y:Cb:Cr = 4:4:4 (mcu=8x8) -> 目前可做到 Y:Cb:Cr = 4:1:1 (mcu=16x16), Y:Cb:Cr = 2:1:1 (mcu=16x8), Y:Cb:Cr = 2:1:1 (mcu=8x16) 
  * 量化表(DefineQuantizationTable)僅可接受一次讀一個量化表 -> 可接受一次讀兩個
