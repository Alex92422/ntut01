# ntut01
# 黃世儲的程式紀錄

## 介紹

參加python體驗營，成果發表

## 成果展示

![](https://github.com/grand-coder/Alex92422/ntut01/raw/master/demo.png)

## 使用技術

名稱    |    說明
-------|-----------
Python | 使用語言
Flask  | 架設網站
repl.it | 線上寫程式環境
Heroku | 免費放網站的佛心公司
Github | 真正的佛心企業

## 範例代碼

```python
@app.route("/")
def root():
  ds = glob.glob("articles/*")
  result = []
  for d in ds:
    fs = glob.glob(d + "/*.txt")
    t = (d.split("/")[-1], len(fs))
    result.append(t)
  return render_template("index.html", d = result)
```

## 網址

[請點我](https://alex92422.herokuapp.com/)
