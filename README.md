# DoubleVSFloat
double型とfloat型の計算速度(sqrt)を測定する
測定結果

||x86|x64|
|:--:|:--:|:--:|
|double|735ミリ秒|1172ミリ秒|
|float|906ミリ秒|938ミリ秒|

x86 の方が double が速くて、x64 では float の計算が速かった。
