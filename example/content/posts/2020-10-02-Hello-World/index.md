---
title: "Hello World - My first blog"
tags: ["gatsby", "blog", "test1", "test2", "test3"]
date: 2020-10-02
cover: "./preview.png"
path: "posts/hello-world"
excerpt: I started to build this personal website yesterday.
---

I started to build this personal website yesterday.

LaTeX test:

$$x^3+y^3=z^3$$

Though I'm quite satisfied showing my work on [GitHub](https://github.com/sleepymalc), it turns out that I have much more want to show. For example, GitHub is extremely unfriendly to show `.pdf` files since the internal link (we call it *hyperlink* for those $\LaTeX$ geeks) doesn't work. This kind
of problem arises quite often. Besides, my only hobby these days is *photographing*, and as you may already know, no one will show their photos on GitHub!

Apart from all these, since I use $\LaTeX$ a **LOT** (yup, I'm one of those $\LaTeX$ Freaks), and the only way I know how to render $\LaTeX$ formula on GitHub is *ugly*, and it can only render fixed color texts, hence this makes me made my mind eventually.
For example, we can easily print out some beautiful formula like
<!-- $$\begin{tikzcd}
			S & {G_\alpha} \\
			{G_\beta} & {G_\alpha \ast_S G_\beta} \\
			&& X
			\arrow["{i_{\alpha \beta} }", from=1-1, to=1-2]
			\arrow["{i_{\beta \alpha} }"', from=1-1, to=2-1]
			\arrow[from=1-2, to=2-2]
			\arrow[from=2-1, to=2-2]
			\arrow["{\exists !}", dashed, from=2-2, to=3-3]
			\arrow[curve={height=-12pt}, from=1-2, to=3-3]
			\arrow[curve={height=12pt}, from=2-1, to=3-3]
		\end{tikzcd}$$ -->
which is just a simple [commutative diagram](https://en.wikipedia.org/wiki/Commutative_diagram) for [Seifert–Van Kampen theorem](https://en.wikipedia.org/wiki/Seifert%E2%80%93Van_Kampen_theorem), or like
$$
\lim\limits_{r \to 0} \frac{1}{m(B(x, r))}\int_{B(x, r)}\left\vert f(y) - f(x) \right\vert\,\mathrm{d}y = 0 \text{for a.e. \(x\)}
$$
for $f\in L^1$, which is the statement of [Lebesgue Differentiation Theorem](https://en.wikipedia.org/wiki/Lebesgue_differentiation_theorem).


## Gist Support

```json {numberLines: true}
{
  "openapi": "3.0.2",
  "info": {
    "title": "test",
    "description": "test",
    "version": "0.1.0"
  },
  "paths": {
    "/": {
      "get": {
        "summary": "test",
        "operationId": "test",
        "parameters": [
          {
            "required": false,
            "schema": {
              "allOf": [
                {
                  "$ref": "#/components/schemas/ArchiveType"
                }
              ],
              "default": "zip"
            },
            "name": "archiveType",
            "in": "query"
          }
        ],
        "responses": {
          "200": {
            "description": "Successful Response",
            "content": {
              "application/json": {
                "schema": {
                }
              }
            }
          }
        }
      }
    }
  },
  "components": {
    "schemas": {
      "ArchiveType": {
        "title": "ArchiveType",
        "enum": [
          "zip",
          "tar",
          "unknown"
        ],
        "type": "string",
        "description": "An enumeration."
      }
    }
  }
}
```


[//]: # (<script src="https://gist.github.com/tc-imba/76dc7e627a56ac84b5c1c14b08d90f1e.js"></script>)

`gist:tc-imba/76dc7e627a56ac84b5c1c14b08d90f1e`


[//]: # ()
[//]: # (`gist:weirdpattern/ce54fdb1e5621b5966e146026995b974#syntax.text`)


<iframe frameborder="0"
style="min-width: 200px; width: 60%; height: 460px;"
scrolling="no"
seamless="seamless"
srcdoc='<html><body><style type="text/css">.gist .gist-data { height: 400px; }</style><script src="https://gist.github.com/sundbry/5e0507d93d4c89023b2ba5f39f27f722.js"></script></body></html>'
/>