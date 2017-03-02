# DoubleVSFloat
平方根(sqrt)の計算速度を調べる。double型とfloat型で速度に違いが出るか？
測定結果

||x86|x64|
|:--:|:--:|:--:|
|double|735ミリ秒|1172ミリ秒|
|float|906ミリ秒|938ミリ秒|

x86 の方が double が速くて、x64 では float の計算が速かった。

x64 では float を引数にとる sqrtf が定義されているが、x86 では、sqrtf は内部で sqrt(double を引数にとる)が呼ばれていた。
