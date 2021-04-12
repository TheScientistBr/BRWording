## `BRWording` - Text Analytics for Portuguese Wordings

Create an easy Text Analytics in *`One-Line-Code`*

<hr>

![](https://img.shields.io/badge/pypi-0.0.1-blue) ![](https://img.shields.io/badge/python-3.7|3.8|3.9-lightblue) ![](https://img.shields.io/badge/Licence-MIT-lightgray) ![](https://img.shields.io/badge/status-Beta-darkgreen) ![](https://img.shields.io/badge/pipeline-passed-green) ![](https://img.shields.io/badge/testing-passing-green) ![](https://img.shields.io/badge/TheScientist-APP-brown)


**Main Features:**

- Load `Excel`, `CSV` and `TXT` file types
- Stemming
- Lemmatization
- Stopwords
- TD-IDF
- Sentimental Analysis
- Graphical interpretation
- Word Cloud


<hr>

## How to Install

```shell
pip install BRWording
```

<BR>
<hr>
<BR>

## How to use

`sintax`:
```python
from brwording import brwording

w = brwording.wording()

w.load_file('data/crashcourse.txt',type='txt')
w.build_tf_idf(lemmatizer=True,stopwords=True)

w.tfidf

```

**Output**

|ID	|doc	|word	|f	|tf	|idf	|tf_idf	|sign|
+---+-------+-------+---+---+-------+-------+----+
|0	|doc-0	|bonito	|1	|1.0	|1.584963	|1.584963	|positive|
1	doc-0	gato	1	1.0	2.584963	2.584963	neutral
2	doc-1	cachorro	1	1.0	2.584963	2.584963	neutral
3	doc-1	feliz	1	1.0	1.584963	1.584963	positive
4	doc-2	animal	1	1.0	1.000000	1.000000	neutral

If want to see the sentimental Graphical interpretation

`sintax`:
```python

w.sentimental_graf()

```

if you want to create a wordcloud

`sintax`:
```python
w.word_cloud()


```
<hr>
<BR>

`enjoi!`
