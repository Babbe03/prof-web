---
title: "What Creates Long-term Retention?"
subtitle: "Understanding the core tenets of long-term retention"
excerpt: "The goal of teaching is to create an acquisition of knowledge in students. Yet, many professors repeat the same tactics without knowing their efficacy. For long-term retention students need variability, separation, and strategies. Without understanding what long-term retention is built off of, a professor can never teach properly."
#date: 2021-01-20
author: "Alison Hill"
draft: false
# layout options: single, single-sidebar
layout: single
categories:
- Retention
---

## Rendering mathematical equations

Examples from the [mathjax demo](https://www.mathjax.org/#demo).
But they work with `katex` as well.

### Rmarkdown

In `.Rmarkdown` documents, you can use either

```
$a \ne 0$
```

to get inline math: `\(a \ne 0\)`.
There is no conflict with using dollar symbols regularly, because `knitr` automatically escapes freestanding dollar symbols.

And you can use

```
$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$
```

to get a math paragraph:

$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

### md

In `.md` documents, you can **not** use the single dollar syntax.
The double dollar syntax still gives you a math paragraph.

```
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$
```

$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}$$

In order to get inline equations, use:

```
`\(a \ne 0\)`
or
\\(a \ne 0\\)
```

to get: `\(a \ne 0\)`.



