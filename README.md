# batch_tips
バッチプログラムのTips






## 環境変数PATHをfor文でまわして１つずつ表示する

```for %i in ("%PATH:;=" "%") do @echo %~i```

※バッチプログラムの場合は %i を %%i に置き換える













