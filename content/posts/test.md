+++
title = 'Test'
date = 2023-09-03T10:47:51-04:00
draft = false
+++

# Test code snippets

```python
from langroid.language_models.base import LLMMessage, Role
msg = LLMMessage(
        content="what is the capital of Bangladesh?",
        role=Role.USER,
      )
```

# Maybe better syntax highlighting using shortcode

```python {linenos=table,hl_lines=[2, "4-5"],linenostart=1}
from langroid.language_models.base import LLMMessage, Role
msg = LLMMessage(
        content="what is the capital of Bangladesh?",
        role=Role.USER,
      )
```

# Test math notation

A nice equation is $e^{i\pi} + 1 = 0$, which is known as Euler's identity.
Here is a cool equation too, and in display mode:

$$
e = mc^2
$$

# Latex with newlines

For math blocks that use `\\` for newlines, use the `math` shortcode like this:
```
{{</* math */>}}
$$
\begin{bmatrix}
a & b \\
c & d \\
e & f \\
\end{bmatrix}
$$
{{</* /math */>}}
```

which renders like this:

{{< math >}}
$$
\begin{bmatrix}
a & b \\
c & d \\
e & f \\
\end{bmatrix}
$$
{{< /math >}}

or a multi-line equation

{{< math >}}
$$
\begin{aligned}
\dot{x} & = \sigma(y-x) \\
\dot{y} & = \rho x - y - xz \\
\dot{z} & = -\beta z + xy
\end{aligned}
$$
{{< /math >}}

