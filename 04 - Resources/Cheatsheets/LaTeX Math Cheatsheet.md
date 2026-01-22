---
title: LaTeX Math Cheatsheet
created: 22-01-2026 17:32
domain: docs
type: cheatsheet
tags:
  - engineering
  - docs
  - LaTeX
source_note: "[[LaTeX]]"
Links to your resource note related:
---
# ⚙️ LaTeX Math Cheatsheet

> **A Cheatsheet for LaTeX, using Markdown for markup. 

---
Special characters / Symbols
============================

> [!abstract] Math Accents
> | Description | Input | Rendered |
> |---|---|---|
> | Hat | `$\hat{a}$` | $\hat{a}$ |
> | Dot | `$\dot{a}$` | $\dot{a}$ |
> | Bar | `$\bar{a}$` | $\bar{a}$ |
> | Tilde | `$\tilde{a}$` | $\tilde{a}$ |
> | Vector | `$\vec{a}$` | $\vec{a}$ |

> [!summary] Capital Greek Letters
> |      LaTex |   Rendered |    LaTex | Rendered |
> | ---------: | ---------: | -------: | -------: |
> |   `\Gamma` |   $\Gamma$ | `\Delta` | $\Delta$ |
> |  `\Lambda` |  $\Lambda$ |   `\Phi` |   $\Phi$ |
> |      `\Pi` |      $\Pi$ |   `\Psi` |   $\Psi$ |
> |   `\Sigma` |   $\Sigma$ | `\Theta` | $\Theta$ |
> | `\Upsilon` | $\Upsilon$ |    `\Xi` |    $\Xi$ |
> |   `\Omega` |   $\Omega$ |          |          |

>[!summary] Lowercase Greek Letters
|      LaTex |   Rendered |     LaTex |  Rendered |
| ---------: | ---------: | --------: | --------: |
|   `\alpha` |   $\alpha$ |     `\nu` |     $\nu$ |
|    `\beta` |    $\beta$ |  `\kappa` |  $\kappa$ |
|   `\gamma` |   $\gamma$ | `\lambda` | $\lambda$ |
|   `\delta` |   $\delta$ |     `\mu` |     $\mu$ |
| `\epsilon` | $\epsilon$ |   `\zeta` |   $\zeta$ |
|     `\eta` |     $\eta$ |  `\theta` |  $\theta$ |
|    `\iota` |    $\iota$ |     `\xi` |     $\xi$ |
|      `\pi` |      $\pi$ |    `\rho` |    $\rho$ |
|   `\sigma` |   $\sigma$ |    `\tau` |    $\tau$ |
| `\upsilon` | $\upsilon$ |    `\phi` |    $\phi$ |
|     `\chi` |     $\chi$ |    `\psi` |    $\psi$ |
|   `\omega` |   $\omega$ |           |           |

> [!summary] Other Greek Letters
> | LaTex       |   Rendered | LaTex       |   Rendered |
> |-----------:|-----------:|------------:|-----------:|
> |`\digamma`  | $\digamma$ | `\varepsilon`| $\varepsilon$ |
> |`\varkappa` | $\varkappa$ | `\varphi`   | $\varphi$ |
> |`\varpi`    | $\varpi$ | `\varrho`   | $\varrho$ |
> |`\varsigma` | $\varsigma$ | `\vartheta` | $\vartheta$ |
> |`\eth`      | $\eth$ | `\hbar`     | $\hbar$ |

> [!summary] Calculus
> | Description | Input | Rendered |
> |---|---|---|
> | Partial Derivative | `$\partial$` | $\partial$ |
> | Nabla (Gradient) | `$\nabla$` | $\nabla$ |
> | Integral | `$\int_{a}^{b} f(x) \,dx$` | $\int_{a}^{b} f(x) \,dx$ |
> | Summation | `$\sum_{i=1}^{n} i^2$` | $\sum_{i=1}^{n} i^2$ |
> | Product | `$\prod_{n=1}^{\infty} p_n$` | $\prod_{n=1}^{\infty} p_n$ |

> [!summary] Set Theory
> | Description | Input | Rendered |
> |---|---|---|
> | Belongs to | `$\in$` | $\in$ |
> | Does not belong to | `$\notin$` | $\notin$ |
> | Subset | `$\subset$` | $\subset$ |
> | Superset | `$\supset$` | $\supset$ |
> | Subset or equal | `$\subseteq$` | $\subseteq$ |
> | Union | `$\cup$` | $\cup$ |
> | Intersection | `$\cap$` | $\cap$ |
> | Empty Set | `$\varnothing$` | $\varnothing$ |

> [!summary] Logic
> | Description | Input | Rendered |
> |---|---|---|
> | Conjunction (AND) | `$\wedge$` | $\wedge$ |
> | Disjunction (OR) | `$\vee$` | $\vee$ |
> | Negation | `$\neg` or `\not$` | $\neg$ |
> | For all | `$\forall$` | $\forall$ |
> | Exists | `$\exists$` | $\exists$ |
> | Does not exist | `$\nexists$` | $\nexists$ |
> | Top | `$\top$` | $\top$ |
> | Bottom / Contradiction | `$\bot$` | $\bot$ |

> [!summary] Relational & Miscellaneous Symbols
> | Description | Input | Rendered |
> |---|---|---|
> | Greater/Less than or equal |`$\geq` / `\leq$`| $\geq$ / $\leq$ |
> | Greater/Less than |`$\gg` / `\ll$`| $\gg$ / $\ll$ |
> | Equivalent | `$\equiv$` | $\equiv$ |
> | Not equal | `$\neq$` | $\neq$ |
> | Approximately | `$\approx$` | $\approx$ |
> | Proportional to | `$\propto$` | $\propto$ |
> | Parallel to | `\parallel` | $\parallel$ |
> | Perpendicular to | `$\perp$` | $\perp$ |
> | Arrows | `$\rightarrow` / `\Rightarrow$` | $\rightarrow$ / $\Rightarrow$ |
> | Infinity | `$\infty$` | $\infty$ |
> | Angle | `$\angle$` / `\measuredangle`| $\angle$ / $\measuredangle$ |

Advanced Formatting
===================

> [!example] Fractions, Binomials, and Matrices
> | Description | Input | Rendered |
> |---|---|---|
> | Fraction | `$\frac{a}{b}$` | $\frac{a}{b}$ |
> | Continued Fraction | `$`x = a_0 + \frac{1}{a_1 + \frac{1}{a_2 + \dotsb}}`$` | $x = a_0 + \frac{1}{a_1 + \frac{1}{a_2 + \dotsb}}$ |
> | Binomial Coefficient | `$\binom{n}{k}$` | $\binom{n}{k}$ |
> | Matrix (Parentheses) | `$\begin{pmatrix} a & b \\ c & d \end{pmatrix}$` | $\begin{pmatrix} a & b \\ c & d \end{pmatrix}$ |
> | Matrix (Brackets) | `$\begin{bmatrix} a & b \\ c & d \end{bmatrix}$` | $\begin{bmatrix} a & b \\ c & d \end{bmatrix}$ |
> | Matrix (Braces) | `$\begin{Bmatrix} a & b \\ c & d \end{Bmatrix}$` | $\begin{Bmatrix} a & b \\ c & d \end{Bmatrix}$ |
> | Matrix (Pipes) | `$\begin{vmatrix} a & b \\ c & d \end{vmatrix}$` | $\begin{vmatrix} a & b \\ c & d \end{vmatrix}$ |
> | Matrix (Double Pipes) | `$\begin{Vmatrix} a & b \\ c & d \end{Vmatrix}$` | $\begin{Vmatrix} a & b \\ c & d \end{Vmatrix}$ |

> [!note] Latin
> ##### No dot:  
> `\imath` $\rightarrow$ $\imath$,
> `\jmath` $\rightarrow$ $\jmath$
> ##### Hat:  
> `\hat{\imath}`  $\rightarrow$ $\hat{\imath}$,
> `\hat{\jmath}`  $\rightarrow$ $\hat{\jmath}$

> [!Example Expressions] 
|                       Input |                  Rendered |
| --------------------------: | ------------------------: |
|           `$a = b + c − d$` |           $a = b + c − d$ |
|    `$\sqrt{\frac{\pi}{2}}$` |    $\sqrt{\frac{\pi}{2}}$ |
| `$y = a x_1^2 + b x_2 + c$` | $y = a x_1^2 + b x_2 + c$ |

Named operators
===============
> [!operators] 
$\arccos$,
$\arcsin$,
$\arctan$,
$\arg$,
$\cos$,
$\cosh$,
$\cot$,
$\coth$,
$\deg$,
$\det$,
$\dim$,
$\exp$,
$\gcd$,
$\hom$,
$\inf$,
$\injlim$,
$\lg$,
$\lim$,
$\liminf$,
$\limsup$,
$\ln$,
$\log$,
$\max$,
$\min$,
$\Pr$,
$\projlim$,
$\sec$,
$\sin$,
$\sinh$,
$\sup$
