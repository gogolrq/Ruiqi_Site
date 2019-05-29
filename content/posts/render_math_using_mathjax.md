---
title : "Using MathJax in Hugo"
date : "2019-05-16T16:33:15"
draft : false
mathjax : ture
---
<br>
## Examples
### Inline math:
$\sqrt{3x-1}+(1+x)^2$.

### Display math:
\begin{align}
(x+2)^2 &= x^2+2x+4\newline
&=(x+1)^2+3
\end{align}

## Issue with Subscript

After enabling MathJax, any math entered between proper markers (see the MathJax documentation) will be processed and typeset in the web page. One issue that comes up, however, with Markdown is that the underscore character "\_" is interpreted by Markdown as a way to wrap text in emph blocks while LaTeX (MathJax) interprets the underscore as a way to create a subscript. This “double speak” of the underscore can result in some unexpected and unwanted behavior. My suggestion is to simply use "\\_ " instead of "\_" in your LaTeX code.

Here is a example: \$\sum\\_{k=1}^n a\\_k\$ and the result is $\sum\_{k=1}^n a\_k$.
