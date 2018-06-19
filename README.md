# batch_tips
バッチプログラムのTips






## 環境変数PATHをfor文でまわして１つずつ表示する

```for %i in ("%PATH:;=" "%") do @echo %~i```

※バッチプログラムの場合は %i を %%i に置き換える



## propertiesファイル(iniファイル)の内容を1行ずつ表示する

```for /f "usebackq eol=# tokens=1,* delims==" %i in (file.ini) do @echo i=%i j=%j```


    file.ini
```
    # xyz=123
    abc.txt=123,456,789
    xyz.csv=000=123
```







