# pythondiary

## 專案介紹

沒什麼好介紹的

## 作者介紹

將靈魂之暗染紅，聆聽業火的慟哭!

## 成品展示

[網站網址(host by heroku)](https://final0817--onthesky123.repl.co/)

![](https://github.com/onthesky123/pythondiary/raw/master/photo-3.png)

## 使用技術

工具名稱 | 用途
---------|----------
Python 3 | 不需要解釋
Flask(python)    | 幫助我建立伺服器
HTML/CSS  | 網頁表示和排版
Heroku   | 託管網頁
Github   | 存放原始碼

## 程式碼片段

```python
@app.route("/")
def home():
    temp = glob.glob("articles/*")
    fill = []
    for t in temp:
        length = len(glob.glob(t + "/*.txt"))
        category = t.replace("articles/", "")
        f = (category, length)
        fill.append(f)
    return render_template("index.html", cat=fill)

```

