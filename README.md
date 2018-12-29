# github_markdown
## What is this?
A tool for converting an ugly LaTeX expression such as:

$p(y=1 \mid f_1=1, f_2=1. f_6=0)$ 

into something like this:

![](https://tex.s2cms.ru/svg/%24p%28y%3D1%20%5Cmid%20f_1%3D1%2C%20f_2%3D1.%20f_6%3D0%29%24).

Github Markdown does not support LaTeX math mode natively.

## How do I get it?
Get it with PIP:

```python
pip install github-markdown
```

## How do I use it?
Have two files ready, one containing the markdown to be converted, and another one which the converted markdown is written to, can be empty or not, it does not matter.
```python
import github_markdown as gm

i = 'file_in.md'
o = 'file_out.md'

gm.markdown_texify(i,o)
```
