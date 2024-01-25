+++
title = 'Passthrough tests'
date = 2024-01-15T12:33:14-08:00
draft = false
+++

## Equations not mangled by Goldmark

These equations do not contain ampersands, matching underscores, sequential backslashes, or delimiters beginning with a backslash, so they are not mangled by Goldmark.

### Inline with `$...$` delimiters

```text
// Example 1: delimiters on same line

Inline $x = {-b \pm \sqrt{b^2-4ac} \over 2a}$ equation
```

Inline $x = {-b \pm \sqrt{b^2-4ac} \over 2a}$ equation

```text
// Example 2: delimiters on their own lines

Inline $
x = {-b \pm \sqrt{b^2-4ac} \over 2a}
$ equation
```

Inline $
x = {-b \pm \sqrt{b^2-4ac} \over 2a}
$ equation

```text
// Example 3: delimiters split over two lines

Inline $x = {-b \pm \sqrt{b^2-4ac} \over 2a}
$ equation
```

Inline $x = {-b \pm \sqrt{b^2-4ac} \over 2a}
$ equation

```text
// Example 4: delimiters split over two lines

Inline $
x = {-b \pm \sqrt{b^2-4ac} \over 2a}$ equation
```

Inline $
x = {-b \pm \sqrt{b^2-4ac} \over 2a}$ equation

### Block with `$$...$$` delimiters

```text
// Example 5: delimiters on same line

Block $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}$$ equation
```

Block $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}$$ equation

```text
// Example 6: delimiters on their own lines

Block $$
x = {-b \pm \sqrt{b^2-4ac} \over 2a}
$$ equation
```

Block $$
x = {-b \pm \sqrt{b^2-4ac} \over 2a}
$$ equation

```text
// Example 7: delimiters split over two lines

Block $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}
$$ equation
```

Block $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}
$$ equation

```text
// Example 8: delimiters split over two lines

Block $$
x = {-b \pm \sqrt{b^2-4ac} \over 2a}$$ equation
```

Block $$
x = {-b \pm \sqrt{b^2-4ac} \over 2a}$$ equation

## Equations mangled by Goldmark

These equations contain ampersands, matching underscores, sequential backslashes, or delimiters beginning with a backslash, so they are mangled by Goldmark.

### Inline with `$...$` delimiters

```text
// Example 9: delimiters on same line

Inline $a^*=x-b^*$ equation
```

Inline $a^*=x-b^*$ equation

```text
// Example 10: delimiters on their own lines

Inline $
a^*=x-b^*
$ equation
```

Inline $
a^*=x-b^*
$ equation

```text
// Example 11: delimiters split over two lines

Inline $a^*=x-b^*
$ equation
```

Inline $a^*=x-b^*
$ equation

```text
// Example 12: delimiters split over two lines

Inline $
a^*=x-b^*$ equation
```

Inline $
a^*=x-b^*$ equation

### Block with `$$...$$` delimiters

```text
// Example 13: delimiters on same line

Block $$a^*=x-b^*$$ equation
```

Block $$a^*=x-b^*$$ equation

```text
// Example 14: delimiters on their own lines

Block $$
a^*=x-b^*
$$ equation
```

Block $$
a^*=x-b^*
$$ equation

```text
// Example 15: delimiters split over two lines

Block $$a^*=x-b^*
$$ equation
```

Block $$a^*=x-b^*
$$ equation

```text
// Example 16: delimiters split over two lines

Block $$
a^*=x-b^*$$ equation
```

Block $$
a^*=x-b^*$$ equation

### Inline with `\(...\)` delimiters

```text
// Example 17: delimiters on same line

Inline \(a^*=x-b^*\) equation
```

Inline \(a^*=x-b^*\) equation

```text
// Example 18: delimiters on their own lines

Inline \(
a^*=x-b^*
\) equation
```

Inline \(
a^*=x-b^*
\) equation

```text
// Example 19: delimiters split over two lines

Inline \(a^*=x-b^*
\) equation
```

Inline \(a^*=x-b^*
\) equation

```text
// Example 20: delimiters split over two lines

Inline \(
a^*=x-b^*\) equation
```

Inline \(
a^*=x-b^*\) equation

### Block with `\[...\]` delimiters

```text
// Example 21: delimiters on same line

Block \[a^*=x-b^*\] equation
```

Block \[a^*=x-b^*\] equation

```text
// Example 22: delimiters on their own lines

Block \[
a^*=x-b^*
\] equation
```

Block \[
a^*=x-b^*
\] equation

```text
// Example 23: delimiters split over two lines

Block \[a^*=x-b^*
\] equation
```

Block \[a^*=x-b^*
\] equation

```text
// Example 24: delimiters split over two lines

Block \[
a^*=x-b^*\] equation
```

Block \[
a^*=x-b^*\] equation

## Complex block equation mangled by Goldmark

### Block with `$$...$$` delimiters

```text
// Example 25

$$
\begin{array} {lcl}
  L(p,w_i) &=& \dfrac{1}{N}\Sigma_{i=1}^N(\underbrace{f_r(x_2
  \rightarrow x_1
  \rightarrow x_0)G(x_1
  \longleftrightarrow x_2)f_r(x_3
  \rightarrow x_2
  \rightarrow x_1)}_{sample\, radiance\, evaluation\, in\, stage2}
  \\\\\\ &=&
  \prod_{i=3}^{k-1}(\underbrace{\dfrac{f_r(x_{i+1}
  \rightarrow x_i
  \rightarrow x_{i-1})G(x_i
  \longleftrightarrow x_{i-1})}{p_a(x_{i-1})}}_{stored\,in\,vertex\, during\,light\, path\, tracing\, in\, stage1})\dfrac{G(x_k
  \longleftrightarrow x_{k-1})L_e(x_k
  \rightarrow x_{k-1})}{p_a(x_{k-1})p_a(x_k)})
\end{array}
$$
```

$$
\begin{array} {lcl}
  L(p,w_i) &=& \dfrac{1}{N}\Sigma_{i=1}^N(\underbrace{f_r(x_2
  \rightarrow x_1
  \rightarrow x_0)G(x_1
  \longleftrightarrow x_2)f_r(x_3
  \rightarrow x_2
  \rightarrow x_1)}_{sample\, radiance\, evaluation\, in\, stage2}
  \\\\\\ &=&
  \prod_{i=3}^{k-1}(\underbrace{\dfrac{f_r(x_{i+1}
  \rightarrow x_i
  \rightarrow x_{i-1})G(x_i
  \longleftrightarrow x_{i-1})}{p_a(x_{i-1})}}_{stored\,in\,vertex\, during\,light\, path\, tracing\, in\, stage1})\dfrac{G(x_k
  \longleftrightarrow x_{k-1})L_e(x_k
  \rightarrow x_{k-1})}{p_a(x_{k-1})p_a(x_k)})
\end{array}
$$

### Block with `\[...\]` delimiters

```text
// Example 26

\[
\begin{array} {lcl}
  L(p,w_i) &=& \dfrac{1}{N}\Sigma_{i=1}^N(\underbrace{f_r(x_2
  \rightarrow x_1
  \rightarrow x_0)G(x_1
  \longleftrightarrow x_2)f_r(x_3
  \rightarrow x_2
  \rightarrow x_1)}_{sample\, radiance\, evaluation\, in\, stage2}
  \\\\\\ &=&
  \prod_{i=3}^{k-1}(\underbrace{\dfrac{f_r(x_{i+1}
  \rightarrow x_i
  \rightarrow x_{i-1})G(x_i
  \longleftrightarrow x_{i-1})}{p_a(x_{i-1})}}_{stored\,in\,vertex\, during\,light\, path\, tracing\, in\, stage1})\dfrac{G(x_k
  \longleftrightarrow x_{k-1})L_e(x_k
  \rightarrow x_{k-1})}{p_a(x_{k-1})p_a(x_k)})
\end{array}
\]
```

\[
\begin{array} {lcl}
  L(p,w_i) &=& \dfrac{1}{N}\Sigma_{i=1}^N(\underbrace{f_r(x_2
  \rightarrow x_1
  \rightarrow x_0)G(x_1
  \longleftrightarrow x_2)f_r(x_3
  \rightarrow x_2
  \rightarrow x_1)}_{sample\, radiance\, evaluation\, in\, stage2}
  \\\\\\ &=&
  \prod_{i=3}^{k-1}(\underbrace{\dfrac{f_r(x_{i+1}
  \rightarrow x_i
  \rightarrow x_{i-1})G(x_i
  \longleftrightarrow x_{i-1})}{p_a(x_{i-1})}}_{stored\,in\,vertex\, during\,light\, path\, tracing\, in\, stage1})\dfrac{G(x_k
  \longleftrightarrow x_{k-1})L_e(x_k
  \rightarrow x_{k-1})}{p_a(x_{k-1})p_a(x_k)})
\end{array}
\]

## Other

### Two inline equations in the same paragraph

```text
// Example 27

Two inline equations $a^*=x-b^*$ in the $a^*=x-b^*$ same paragraph
```

Two inline equations $a^*=x-b^*$ in the $a^*=x-b^*$ same paragraph

### Two blocks equations in the same paragraph

```text
// Example 28

Two block equations $$a^*=x-b^*$$ in the $$a^*=x-b^*$$ same paragraph
```

Two block equations $$a^*=x-b^*$$ in the $$a^*=x-b^*$$ same paragraph

### A block equation and an inline equation in the same paragraph

```text
// Example 29

A block equation $$a^*=x-b^*$$ and an inline equation $a^*=x-b^*$ in the same paragraph
```

A block equation $$a^*=x-b^*$$ and an inline equation $a^*=x-b^*$ in the same paragraph

### Inline equations within other markdown elements

Unordered list

- Inline equation $a^*=x-b^*$ within list item
- Inline equation $a^*=x-b^*$ within list item

Description list

Inline equation $a^*=x-b^*$ within description term element (dt)
: Inline equation $a^*=x-b^*$ within description details element (dd)

[Inline equation $a^*=x-b^*$ within link text](https://katex.org)

#### Inline equation $a^*=x-b^*$ within heading

> Inline $a^*=x-b^*$ equation within blockquote

Inline equation `$a^*=x-b^*$` within backticks

    Inline equation $a^*=x-b^*$ within code block

```text
Inline equation $a^*=x-b^*$ within fenced code block
```

### Block equations within other markdown elements

Unordered list

- Block equation $$a^*=x-b^*$$ within list item
- Block equation $$a^*=x-b^*$$ within list item

Description list

Block equation $$a^*=x-b^*$$ within description term element (dt)
: Block equation $$a^*=x-b^*$$ within description details element (dd)

[Block equation $$a^*=x-b^*$$ within link text](https://katex.org)

#### Block equation $$a^*=x-b^*$$ within heading

> Block $$a^*=x-b^*$$ equation within blockquote

Block equation `$$a^*=x-b^*$$` within backticks

    Block equation $$a^*=x-b^*$$ within code block

```text
Block equation $$a^*=x-b^*$$ within fenced code block
```

### Inline equation with currency symbol in text

```text
The price is $10.00, but members get a discount. The final price is $p' = p(1-d)$.
```

The price is $10.00, but members get a discount. The final price is $p' = p(1-d)$.

```text
The price is $10.00, but members get a discount. The final price is \(p' = p(1-d)\).
```

The price is $10.00, but members get a discount. The final price is \(p' = p(1-d)\).

```text
The price is \\$10.00, but members get a discount. The final price is $p' = p(1-d)$.
```

The price is \\$10.00, but members get a discount. The final price is $p' = p(1-d)$.