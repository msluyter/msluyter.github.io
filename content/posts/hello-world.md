---
title: "Hello World"
date: 2026-03-27
draft: false
tags: ["meta", "python"]
summary: "A first test post to verify the blog setup, including syntax highlighting."
---

Welcome to my new blog, powered by [Hugo](https://gohugo.io/) and [PaperMod](https://github.com/adityatelange/hugo-PaperMod).

## Testing Syntax Highlighting

Here's a quick Python snippet to make sure code blocks render properly:

```python
from dataclasses import dataclass
from typing import Iterator


@dataclass
class FibSequence:
    """Generate Fibonacci numbers up to a limit."""
    limit: int

    def __iter__(self) -> Iterator[int]:
        a, b = 0, 1
        while a <= self.limit:
            yield a
            a, b = b, a + b


if __name__ == "__main__":
    fibs = FibSequence(limit=100)
    for n in fibs:
        print(n, end=" ")
    # Output: 0 1 1 2 3 5 8 13 21 34 55 89
```

Looks good!
