# <span id="page-15-0"></span>**【1-3】付録:ギリシャ文字一覧**

| 大文字 | 小文字 | 読み      | 大文字 | 小文字 | 読み      | 大文字 | 小文字 | 読み      |
|-----|-----|---------|-----|-----|---------|-----|-----|---------|
| Α   | α   | alpha   | Ι   | ι   | iota    | Ρ   | ρ   | rho     |
| Β   | β   | beta    | Κ   | κ   | kappa   | Σ   | σ   | sigma   |
| Γ   | γ   | gamma   | Λ   | λ   | lambda  | Τ   | τ   | tau     |
| Δ   | δ   | delta   | Μ   | μ   | mu      | Υ   | υ   | upsilon |
| Ε   | ε   | epsilon | Ν   | ν   | nu      | Φ   | φ   | phi     |
| Ζ   | ζ   | zeta    | Ξ   | ξ   | xi      | Χ   | χ   | chi     |
| Η   | η   | eta     | Ο   | ο   | omicron | Ψ   | ψ   | psi     |
| Θ   | θ   | theta   | Π   | π   | pi      | Ω   | ω   | omega   |

## 【第 2 講】 初等関数

<span id="page-16-1"></span><span id="page-16-0"></span>

### 【2-1】 はじめに

初等関数とは、代数関数（冪関数、多項式関数、有理関数など）、指数関数、対数関数、三角関数、逆三角関数、双曲線関数、逆双曲線関数とそれらの合成関数で作られる 1 変数関数のことである。数学の各分野はもちろん、理工学のあらゆる分野において応用される重要な関数である。本講座では一部の例外を除き、実数の範囲内で取り扱う。本講では、そのうち特に重要な指数関数、対数関数、三角関数とその性質、およびオイラーの公式を導いてそれらの関係を学ぶ。

<span id="page-16-2"></span>

### 【2-2】 指数・対数関数

#### 【2-2-1】 指数関数の定義と性質

実数を指数とした数（例えば  $2^{\sqrt{2}}$ ）は、具体的にどのようにして求められるか考えたことがあるだろうか？実はこれはそれほど単純な話ではない。第 1 講 イントロダクションで触れたように、実数は実は奥が深い。

まずは 2 の自然数乗（正の整数乗：**累乗**）から始めよう。以下  $n, m \in \mathbb{N}$ ,  $n, m > 0$  とする。

2 を  $n$  回掛け合わせた数を  $2^n$  と表記し、2 の  $n$  乗として定義する。

この時の 2 を**基数**、 $n$  を**指数**という。

定義から  $2^n \times 2^m = 2^{n+m}$ ,  $(2^n)^m = 2^{nm}$  が、また  $(2 \times 3)^n = 2^n \times 3^n$  等も成り立つ。

一般に非零の実数  $a, b \in \mathbb{R}$ ,  $a, b \neq 0$  の累乗についても同様に

$$a^n \times a^m = a^{n+m}, (a^n)^m = a^{nm}, (ab)^n = a^n b^n$$

が成り立つ。

これらの性質が、指数が整数の場合でも成立するような拡張を考える。

 $a^0 \times a^n = a^{0+n} = a^n$  より、 $a^0 \equiv 1$  また  $a^{-n} \times a^n = a^{-n+n} = a^0 = 1$  より  $a^{-n} \equiv 1/a^n$  とすれば、 $p, q \in \mathbb{Z}$  とし、指数が整数の場合でも同様に

$$a^p \times a^q = a^{p+q}, (a^p)^q = a^{pq}, (ab)^p = a^p b^p$$

が成り立つ。またこの拡張により

$$\frac{a^p}{a^q} = a^{p-q}, \quad \left(\frac{a}{b}\right)^p = \frac{a^p}{b^p}$$

も成り立つ。

指数が有理数の場合への拡張を考える。有理数でもこれらの性質が成り立つとすると、

$$\left(\frac{1}{a^2}\right)^2 = \frac{1}{a^2} = a \text{ より、} \frac{1}{a^2} \equiv \sqrt{a} \text{ とすればよいが、それが実数の範囲内で値を持つとすると、} a > 0$$

という制限をつける事になる。その上で一般に  $\left(a^{\frac{q}{p}}\right)^p = a^{\frac{pq}{p}} = a^q$  より、 $a^{\frac{q}{p}} \equiv \sqrt[p]{a^q}$  とする事で、 $r, s \in \mathbb{Q}$  として、指数が有理数でも同様に  $a, b \in \mathbb{R}, a, b > 0$  に対して

$$a^r \times a^s = a^{r+s}, \quad \frac{a^r}{a^s} = a^{r-s}, \quad (a^r)^s = a^{rs}, \quad (ab)^r = a^r b^r, \quad \left(\frac{a}{b}\right)^r = \frac{a^r}{b^r}$$

が成り立つ。

指数が実数の場合への拡張は、一筋縄ではいかない。例として、 $2^{\sqrt{2}}$  を考える。

 $\sqrt{2} = 1.41421356 \dots$  と無限に続く小数であるが、これを

 $1, 1.4, 1.41, 1.414, 1.4142, 1.41421, 1.414213, 1.4142135, 1.41421356, \dots$ 

として有限小数（有理数）の数列とみなし、

 $2^1, 2^{1.4}, 2^{1.41}, 2^{1.414}, 2^{1.4142}, 2^{1.41421}, 2^{1.414213}, 2^{1.4142135}, 2^{1.41421356} \dots$  という数列を考える。

この数列は、

$$\begin{array}{rcl} 2^1 & = & 2 \\ 2^{1.4} & = & 2.63901582 \dots \\ 2^{1.41} & = & 2.65737162 \dots \\ 2^{1.414} & = & 2.66474965 \dots \\ 2^{1.4142} & = & 2.66511908 \dots \\ 2^{1.41421} & = & 2.66513756 \dots \\ 2^{1.414213} & = & 2.66514310 \dots \\ 2^{1.4142135} & = & 2.66514402 \dots \\ 2^{1.41421356} & = & 2.66514413 \dots \\ \vdots & & \end{array}$$

というように一定の値に近づいていく事がわかる。

このように、指数が実数の場合は、その実数に近づく有理数の数列を用い、有理数乗の数列の極限として定義することになる<sup>9</sup>。

このような定義により、 $a, b \in \mathbb{R}, a, b > 0, \forall x, y \in \mathbb{R}$  に対しても

$$a^x \times a^y = a^{x+y}, \quad \frac{a^x}{a^y} = a^{x-y}, \quad (a^x)^y = a^{xy}, \quad (ab)^x = a^x b^x, \quad \left(\frac{a}{b}\right)^x = \frac{a^x}{b^x}$$

が成り立つ。これらの基本となる性質を**指数法則**という。

指数が実数にまで拡張され、任意の実数により連続した指数に対する値が得られるようになった。

基数  $a = 1$  の場合、全ての  $x$  に対して  $1^x = 1$  となるため、それ以外の  $0 < a < 1$  の場合と、 $1 < a$  の場合の  $a^x$  を**指数関数**として定義する。このときの  $a$  は基数でなく**底**と呼ばれる。

<sup>9</sup> 4 節にて違う定義を導く

指数法則より得られる指数関数の基本性質として

●  $1 < a$  の場合

- • 単調増加関数
- •  $x \rightarrow -\infty$  で  $x$  軸に漸近
- •  $x = 0$  の時、 $a^0 = 1$

●  $0 < a < 1$  の場合

- • 単調減少関数
- •  $x \rightarrow \infty$  で  $x$  軸に漸近
- •  $x = 0$  の時、 $a^0 = 1$

また定義域は実数全体、値域は正の実数全体となる。右図は指数関数  $y = a^x$  のグラフの例であり、上記の基本的な性質が読み取れる。

![](_page_18_Figure_42.jpeg)

**[2-2-2] 対数関数の定義と性質**

指数関数  $a^x$  は全ての正の実数を値域にとり、 $0 < a < 1$  ならば単調減少関数、 $1 < a$  ならば単調増加関数であるため、任意の正の実数  $Y$  に対して、 $Y = a^x$  となる実数  $x$  がただ一つ定まる。

この  $x$  を、 $Y$  に対する  $a$  を底とする**対数**といい、 $x = \log_a Y$  と表す。このときの  $Y$  を**真数**という。

![](_page_18_Figure_46.jpeg)

定義より、対数は指数法則に対応した以下の性質をもつ。

 $a, Y, Z \in \mathbb{R}$ ,  $a > 0, a \neq 1, Y, Z > 0$  に対し

(i)  $\log_a YZ = \log_a Y + \log_a Z$   
 $y = \log_a Y, z = \log_a Z$  とすると  $Y = a^y, Z = a^z$  であり、 $YZ = a^y a^z = a^{y+z}$   
 $\therefore \log_a YZ = y + z = \log_a Y + \log_a Z$  ■

(ii)  $\log_a \frac{Y}{Z} = \log_a Y - \log_a Z$   
 $y = \log_a Y, z = \log_a Z$  とすると  $Y = a^y, Z = a^z$  であり、 $Y/Z = a^y/a^z = a^{y-z}$   
 $\therefore \log_a \frac{Y}{Z} = y - z = \log_a Y - \log_a Z$  ■

(iii)  $\log_a Y^t = t \log_a Y$   
 $y = \log_a Y$  とすると  $Y = a^y$  であり、 $Y^t = (a^y)^t = a^{yt}$   
 $\therefore \log_a Y^t = yt = t \log_a Y$  ■

また  $b \in \mathbb{R}, b > 0, b \neq 1$  に対し底の変換公式と呼ばれる以下の性質をもつ。

(iv)  $\log_a Y = \frac{\log_b Y}{\log_b a}$ 

 $y = \log_a Y, z = \log_b Y, a = b^t$  とすると  $t = \log_b a, Y = b^z = a^y = (b^t)^y = b^{ty}, \therefore z = ty$ 

よって  $y = \frac{z}{t}$  より  $\log_a Y = \frac{\log_b Y}{\log_b a}$  ■

このように定義された対数に対し、 $y = \log_a x$  として**対数関数**を定義する。

定義より  $y = \log_a x$  に対して  $x = a^y = a^{\log_a x}$  また  $y = \log_a x = \log_a a^y$  となり、

 $y = \log_a x$  と  $y = a^x$  は互いに逆関数となる。

これらの定義により、対数関数は以下の性質を持つ。

底  $a \in \mathbb{R}, a > 0, a \neq 1$  に対し

•  $0 < a < 1$  のとき 単調減少関数

•  $1 < a$  のとき 単調増加関数

定義域は正の実数、値域は実数全体であり、 $x = 1$  のとき  $\log_a 1 = 0$  となる。

![](_page_19_Figure_31.jpeg)

![](_page_19_Figure_32.jpeg)

上の図は底  $a$  が  $0 < a < 1$  の場合と  $1 < a$  の場合の対数関数と指数関数のグラフの例で、上記性質の他、それぞれ  $y = x$  の点線に対して対称となっており逆関数の関係であることも読み取れる。

底  $a$  の対数関数とは何かを一言で言うと、「( $a$ 進数としたときの) 桁数を返す関数」となる。

**[2-2-3] 自然対数と自然指数**有用な対数の底として、**ネイピア数**と呼ばれる  $e$  が挙げられる。

ネイピア数  $e$  は、

$$e = \lim_{n \rightarrow \infty} \left(1 + \frac{1}{n}\right)^n \quad (2-2-1)$$

で定義される無理数で、その値は

$$e = 2.71828182846 \dots \quad (2-2-2)$$

となる。

ここで(2-2-1)式は、正の整数  $n$  による  $\left(1 + \frac{1}{n}\right)^n$  の値が、 $n$  がどんどん大きくなっていくにつれ一定の値（この場合は(2-2-2)の値）に近づいて行くときの「**極限**」を表しており、記号  $\lim$  は  $\lim_{n \rightarrow \infty}$  と読む。右図は  $\left(1 + \frac{1}{n}\right)^n$  の値を  $n$  が 1 から 100 までの範囲でグラフ化したもので、次第に近づいていく様子が見られる。

![](_page_20_Figure_30.jpeg)

ネイピア数  $e$  を底とする対数は、**自然対数**と呼ばれ、通常  $\log_e x = \ln x$  と表記される。また通常「指数関数」はネイピア数を底とした  $e^x$  の事を指す事が多い。この  $e^x$  は  $\exp(x)$  とも書かれ、自然対数との対比で自然指数と呼ぶ事もある。

「自然」という言葉は、指数関数  $e^x$  が微分しても（従って積分しても）同じ  $e^x$  となるなど、数学的な性質が他の底と比べてシンプルな事から来ており、数学や物理学を始め、理工系の殆どの分野で用いられている。

**[2-2-4] 応用例**上記のように指数関数は解析学との関わりが深く、微分の考え方を用いた微分方程式（パラメータを時間だとすると、今の情報から少し先の未来がどうなるかを記述する方程式）を解く際に活躍してくれる。また対数関数は、（指数関数の）裏方さん的な役割が多いが、人間の知覚や地震のマグニチュードなどの他、「エントロピー」を表し物理学の統計力学や情報理論などの分野で応用されている。

<span id="page-21-0"></span>

### 【2-3】 三角関数

#### 【2-3-1】 三角関数の定義と性質

右図のように半径 1 の単位円上の点  $(x, y)$  において原点と結んだ直線と  $x$  軸との反時計回りを正としたなす角（弧度法）を  $\theta$  とし、その大きさは  $\pm\pi, \pm2\pi$  を超えてもそのまま外挿されるとする時

$$\sin (\text{正弦:サイン}) : \sin \theta = y$$

$$\cos (\text{余弦:コサイン}) : \cos \theta = x$$

として、また  $x \neq 0$  の時、

$$\tan (\text{正接:タンジェント}) : \tan \theta = y/x$$

として定義する。これらを**三角関数**といい、以下の基本的な性質をもつ。

![](_page_21_Figure_42.jpeg)

定義より  $\sin \theta, \cos \theta$  は  $2\pi$  の周期、 $\tan \theta$  は  $\pi$  の周期を持つ周期関数、すなわち以下の関係が成り立つ( $n \in \mathbb{Z}$ )。

$$\begin{aligned} \sin(\theta + 2n\pi) &= \sin \theta \\ \cos(\theta + 2n\pi) &= \cos \theta \\ \tan(\theta + n\pi) &= \tan \theta \end{aligned}$$

 $\sin \theta, \cos \theta$  の定義域は実数全体、値域は  $-1$  以上  $1$  以下の実数となり、 $\sin \theta$  は奇関数 ( $\sin(-\theta) = -\sin \theta$ )  $\cos \theta$  は偶関数 ( $\cos(-\theta) = \cos \theta$ ) である。

また定義よりいわゆる位相のずれとして

$$\sin\left(\theta + \frac{\pi}{2}\right) = \cos \theta, \quad \cos\left(\theta - \frac{\pi}{2}\right) = \cos\left(\frac{\pi}{2} - \theta\right) = \sin \theta$$

が成り立つ。

![](_page_21_Figure_49.jpeg)

 $\tan \theta$  の定義域は  $\frac{\pi}{2} + n\pi$  ( $n \in \mathbb{Z}$ ) を除く実数全体、値域は実数全体であり、 $-\frac{\pi}{2} < \theta < \frac{\pi}{2}$  で単調増加関数となる。

#### 【2-3-2】 三角関数の主な公式

上記基本性質の他に、以下のような性質が公式化されている。このうち加法定理が最も基本的な性質であり、他は加法定理（と上記基本性質）から容易に導かれる。ここでは各公式を列挙し、その証明は本講の付録 4 に記載する。

● 加法定理 (複号同順) (角の和の三角関数を元の角の三角関数で表す)
$$\begin{aligned}\sin(\alpha \pm \beta) &= \sin \alpha \cos \beta \pm \cos \alpha \sin \beta \\ \cos(\alpha \pm \beta) &= \cos \alpha \cos \beta \mp \sin \alpha \sin \beta \\ \tan(\alpha \pm \beta) &= \frac{\tan \alpha \pm \tan \beta}{1 \mp \tan \alpha \tan \beta}\end{aligned}\quad (2-3-1)$$

● 倍角の公式 (2 倍角の三角関数を元の角の三角関数で表す)
$$\begin{aligned}\sin 2\alpha &= 2 \sin \alpha \cos \alpha \\ \cos 2\alpha &= \cos^2 \alpha - \sin^2 \alpha \\ &= 1 - 2 \sin^2 \alpha \\ &= 2 \cos^2 \alpha - 1 \\ \tan 2\alpha &= \frac{2 \tan \alpha}{1 - \tan^2 \alpha}\end{aligned}\quad (2-3-2)$$

● 半角の公式 (半角の三角関数を元の角の三角関数で表す)
$$\begin{aligned}\sin^2 \frac{\alpha}{2} &= \frac{1 - \cos \alpha}{2} \\ \cos^2 \frac{\alpha}{2} &= \frac{1 + \cos \alpha}{2} \\ \tan^2 \frac{\alpha}{2} &= \frac{1 - \cos \alpha}{1 + \cos \alpha}\end{aligned}\quad (2-3-3)$$

● 積和の公式 (三角関数の積を三角関数の和で表す)
$$\begin{aligned}\sin \alpha \cos \beta &= \frac{1}{2} \{\sin(\alpha + \beta) + \sin(\alpha - \beta)\} \\ \cos \alpha \cos \beta &= \frac{1}{2} \{\cos(\alpha + \beta) + \cos(\alpha - \beta)\} \\ \sin \alpha \sin \beta &= -\frac{1}{2} \{\cos(\alpha + \beta) - \cos(\alpha - \beta)\}\end{aligned}\quad (2-3-4)$$

● 和積の公式 (三角関数の和を三角関数の積で表す)
$$\begin{aligned}\sin x + \sin y &= 2 \sin \frac{x+y}{2} \cos \frac{x-y}{2} \\ \sin x - \sin y &= 2 \cos \frac{x+y}{2} \sin \frac{x-y}{2} \\ \cos x + \cos y &= 2 \cos \frac{x+y}{2} \cos \frac{x-y}{2} \\ \cos x - \cos y &= -2 \sin \frac{x+y}{2} \sin \frac{x-y}{2}\end{aligned}\quad (2-3-5)$$

● 合成の公式 (同じ角の三角関数の和を一つの三角関数で表す)
$$\begin{aligned}a \sin \theta + b \cos \theta &= \sqrt{a^2 + b^2} \sin(\theta + \alpha) \\ \cos \alpha &= \frac{a}{\sqrt{a^2 + b^2}}, \sin \alpha = \frac{b}{\sqrt{a^2 + b^2}} \\ a \sin \theta + b \cos \theta &= \sqrt{a^2 + b^2} \cos(\theta - \beta) \\ \sin \beta &= \frac{a}{\sqrt{a^2 + b^2}}, \cos \beta = \frac{b}{\sqrt{a^2 + b^2}}\end{aligned}\quad (2-3-6)$$

**[2-3-3] ド・モアブルの定理**

複素平面上の大きさ 1 の複素数の極形式  $z = \cos \theta + i \sin \theta$  を考える。これは単位円上の点の  $x, y$  座標値として定義された三角関数を複素平面上にそのまま対応させたものとなる。

この表記での複素数  $z_1 = \cos \alpha + i \sin \alpha$ ,  $z_2 = \cos \beta + i \sin \beta$  の積は、加法定理を用いると

$$\begin{aligned} z_1 z_2 &= (\cos \alpha + i \sin \alpha)(\cos \beta + i \sin \beta) \\ &= (\cos \alpha \cos \beta - \sin \alpha \sin \beta) + i(\sin \alpha \cos \beta + \cos \alpha \sin \beta) \\ &= \cos(\alpha + \beta) + i \sin(\alpha + \beta) \end{aligned} \quad (2 - 3 - 7)$$

となり、これは大きさ 1 の複素数の積がその偏角の和の複素数となる事を意味し、加法定理が複素平面上でこのように表されていることになる。幾何学的には大きさ 1、偏角  $\alpha$  の複素数の積が複素平面上での角度  $\alpha$  の回転を表していると解釈できる（下図左）。

![](_page_23_Figure_23.jpeg)

特に  $\alpha = \beta = \theta$  の場合は、

$$\begin{aligned} (\cos \theta + i \sin \theta)^2 &= \cos^2 \theta - \sin^2 \theta + i2 \sin \theta \cos \theta \\ &= \cos 2\theta + i \sin 2\theta \end{aligned}$$

となり、2 倍角の公式を表すと共に、 $(\cos \theta + i \sin \theta)^2 = \cos 2\theta + i \sin 2\theta$  という関係となる。

さらに(2-3-7)式で  $\alpha = \theta, \beta = 2\theta$  とすると、これは  $\cos \theta + i \sin \theta$  の3乗にあたり、

$$\begin{aligned} (\cos \theta + i \sin \theta)^3 &= (4 \cos^3 \theta - 3 \cos \theta) + i(3 \sin \theta - 4 \sin^3 \theta) \\ &= \cos 3\theta + i \sin 3\theta \end{aligned}$$

となり、3 倍角の公式を表し、また  $(\cos \theta + i \sin \theta)^3 = \cos 3\theta + i \sin 3\theta$  が成り立つ。

より高次についても同様となり、帰納的に以下の関係が成り立つ事が分かる（上図右）。

$$(\cos \theta + i \sin \theta)^n = \cos n\theta + i \sin n\theta \quad (2 - 3 - 8)$$

これをド・モアブルの定理という。

**[2-3-4] 応用例**三角関数は幾何学とのつながりが深く、周期性を利用した回転や振動、波動の表現として用いられている。またベクトルの基底としてフーリエ級数展開への応用も本講座でも説明する。

<span id="page-24-0"></span>**[2-4] 指数関数の別定義**ネイピア数の定義 (2-2-1) 式を深掘りしてみよう。今、 $\left(1 + \frac{x}{n}\right)^n$  という式を考える。 $\frac{x}{n} = \frac{1}{m}$  とすると  $n = mx$  より  $\left(1 + \frac{x}{n}\right)^n = \left(1 + \frac{1}{m}\right)^{mx} = \left\{\left(1 + \frac{1}{m}\right)^m\right\}^x$  と書けて、この式で  $x$  を一定とした  $n \rightarrow \infty$  すなわち  $m \rightarrow \infty$  の極限をとると、 $\left\{\left(1 + \frac{1}{m}\right)^m\right\}^x \rightarrow (e)^x$  ( $m \rightarrow \infty$ ) がいえることになる。そこで以下の式を指数関数の新たな定義としよう ( $x = 1$  の場合はネイピア数の定義に帰着する)。

$$e^x = \lim_{n \rightarrow \infty} \left(1 + \frac{x}{n}\right)^n \quad (2-4-1)$$

この定義が意味をなすには、まず極限値が収束する必要がある<sup>10</sup>。

この極限値を評価するため、有限項  $\left(1 + \frac{x}{n}\right)^n$  について考えてみよう。このような  $(a+b)^n$  の形の式を展開するには、二項定理を用いる<sup>11</sup>。展開すると、

$$\begin{aligned} & \left(1 + \frac{x}{n}\right)^n \\ &= 1 + n \left(\frac{x}{n}\right) + \frac{n(n-1)}{2!} \left(\frac{x}{n}\right)^2 + \frac{n(n-1)(n-2)}{3!} \left(\frac{x}{n}\right)^3 + \frac{n(n-1)(n-2)(n-3)}{4!} \left(\frac{x}{n}\right)^4 + \dots \\ &= 1 + x + \frac{(1-\frac{1}{n})}{2!} x^2 + \frac{(1-\frac{1}{n})(1-\frac{2}{n})}{3!} x^3 + \frac{(1-\frac{1}{n})(1-\frac{2}{n})(1-\frac{3}{n})}{4!} x^4 + \dots \end{aligned}$$

となる。各分子の括弧内の  $1/n$  や  $2/n$  等の項は  $n \rightarrow \infty$  の極限で 0 となるので、その極限で各分子は 1 となり

$$\begin{aligned} e^x &= \lim_{n \rightarrow \infty} \left(1 + \frac{x}{n}\right)^n \\ &= 1 + x + \frac{1}{2!} x^2 + \frac{1}{3!} x^3 + \frac{1}{4!} x^4 + \dots \end{aligned} \quad (2-4-2)$$

となる (この級数は任意の  $x$  の値で収束する事が知られている)。実際にこの級数のふるまいを見てみようよう (次頁にて)。

<sup>10</sup> 指数関数を初めてこの形で定式化したのが、オイラーだったそうな。厳密には極限値が収束するうえに、この定義に基づき、指数法則が成り立つことを示す必要がある。

<sup>11</sup> 付録 1 : 二項定理 (二項展開) 参照

右図は(2-4-2)式の右辺を

 $e_n(x) \equiv 1 + x + \dots + \frac{1}{n!} x^n$ として、 $n$  次の項までの和で近似したときの様子を 20 次の項までグラフ化したものであり、次第に  $\exp(x)$  の値に近づいていく様子が分かる。

(2-4-1)式 (あるいは(2-4-2)式) で底  $e$  の指数関数  $e^x$  を定義することで、わざわざ  $e$  の有理数乗の極限という形を経ずに実数乗を直接定義することができることになる。

![](_page_25_Figure_22.jpeg)

なお(2-4-2)式は、指数関数  $e^x$  の  $x = 0$  の周りでのいわゆるテーラー展開 (マクローリン展開) の結果と等しいが、指数関数の場合、微分を使わなくともこのように二項展開した極限として得ることができる。

<span id="page-25-0"></span>**【2-5】 [▼A] オイラーの公式**

(2-3-8)式のド・モアブルの定理  $\cos n\theta + i \sin n\theta = (\cos \theta + i \sin \theta)^n$  (こおいて、 $n\theta = x$  と置くと  $\theta = \frac{x}{n}$  と書けるので、

$$\cos x + i \sin x = \left( \cos \frac{x}{n} + i \sin \frac{x}{n} \right)^n \quad (2-5-1)$$

と書ける。この式で  $x$  を一定とする  $n \rightarrow \infty$  ( $\theta \rightarrow 0$ ) の極限をとることを考えると、

$$\cos \frac{x}{n} \rightarrow 1, \quad \sin \frac{x}{n} \rightarrow \frac{x}{n} \quad (n \rightarrow \infty) \quad (2-5-2)$$

より<sup>12</sup>、

$$\begin{aligned} \cos x + i \sin x &= \lim_{n \rightarrow \infty} \left( \cos \frac{x}{n} + i \sin \frac{x}{n} \right)^n \\ &= \lim_{n \rightarrow \infty} \left( 1 + \frac{ix}{n} \right)^n \end{aligned} \quad (2-5-3)$$

と書けるが、この式は(2-4-1)式で  $x$  を (形式的に)  $ix$  としたものと等しい。

そこで、(2-4-2)式で  $x$  を  $ix$  として置き換え、指数が純虚数となる指数関数を

<sup>12</sup> 付録 3 :  $\sin \theta / \theta \rightarrow 1$  ( $\theta \rightarrow 0$ ) の証明 参照

$$e^{ix} = 1 + ix + \frac{(ix)^2}{2!} + \frac{(ix)^3}{3!} + \frac{(ix)^4}{4!} + \dots \quad (2-5-4)$$

として定義する<sup>13</sup>。これにより、

$$e^{i\theta} = \lim_{n \rightarrow \infty} \left(1 + \frac{i\theta}{n}\right)^n$$

と書けて、これと (2-5-3) 式と合わせると

$$e^{i\theta} = \cos \theta + i \sin \theta \quad (2-5-5)$$

が成り立つ<sup>14</sup>。

この(2-5-5)式は、有名な**オイラーの公式**と呼ばれるもので、指数関数と三角関数の驚くべき関係を端的に表している。

オイラーの公式により、三角関数の加法定理である (2-3-7) 式：

$$(\cos \alpha + i \sin \alpha)(\cos \beta + i \sin \beta) = \cos(\alpha + \beta) + i \sin(\alpha + \beta)$$

は、

$$e^{i\alpha} e^{i\beta} = e^{i(\alpha+\beta)} \quad (2-5-6)$$

となり、純虚数での指数法則が成り立つことを意味する。

これにより逆に三角関数の加法定理を瞬時に出せる（証明できるという意味ではない）。

$$\begin{aligned} \cos(\alpha \pm \beta) + i \sin(\alpha \pm \beta) &= e^{i(\alpha \pm \beta)} = e^{i\alpha} e^{\pm i\beta} = (\cos \alpha + i \sin \alpha)(\cos \beta \pm i \sin \beta) \\ &= (\cos \alpha \cos \beta \mp \sin \alpha \sin \beta) + i(\sin \alpha \cos \beta \pm \cos \alpha \sin \beta) \\ &\therefore \begin{cases} \cos(\alpha \pm \beta) = \cos \alpha \cos \beta \mp \sin \alpha \sin \beta \\ \sin(\alpha \pm \beta) = \sin \alpha \cos \beta \pm \cos \alpha \sin \beta \end{cases} \end{aligned}$$

またド・モアブルの定理  $(\cos \theta + i \sin \theta)^n = \cos n\theta + i \sin n\theta$  は、

$$(e^{i\theta})^n = e^{in\theta} \quad (2-5-7)$$

と書けることになり、これも指数法則の純虚数への拡張に対応している（ただし  $n$  は整数）。

オイラーの公式による指数関数と三角関数の繋がりは、指数関数の基本性質である指数法則と、三角関数の基本的な性質である加法定理、ド・モアブルの定理としても繋がっているという深いつながりであることが分かる。解析学と幾何学の橋渡しを担う重要な役割をもつ。

本講座では第6講で行列版、第8講でクォータニオン版として各講の付録にて再登場する。

$$\begin{cases} \cos x = 1 - \frac{1}{2!}x^2 + \frac{1}{4!}x^4 - \frac{1}{6!}x^6 + \frac{1}{8!}x^8 - \dots \\ \sin x = x - \frac{1}{3!}x^3 + \frac{1}{5!}x^5 - \frac{1}{7!}x^7 + \frac{1}{9!}x^9 - \dots \end{cases} \quad (2-5-8)$$

<sup>13</sup> この辺りの話をきちっとする解析接続というモノがあるが、本講座では立ち入らない

<sup>14</sup> (2-5-4) 式において  $i^2 = -1$  より (2-5-5) 式と実部・虚部を比較して以下も成り立つ。

<span id="page-27-0"></span>**【2-6】 付録 1 : 二項定理 (二項展開)**

 $(a+b)^n$  を展開したものを**二項展開**と言う。二項展開の各項の係数を考えるにあたり、まずは  $n$  の値が小さい場合に実際に展開してみよう。

$$\begin{aligned} (a+b)^0 &= 1 \\ (a+b)^1 &= a+b \\ (a+b)^2 &= a^2 + 2ab + b^2 \\ (a+b)^3 &= a^3 + 3a^2b + 3ab^2 + b^3 \\ (a+b)^4 &= a^4 + 4a^3b + 6a^2b^2 + 4ab^3 + b^4 \end{aligned}$$

係数のみに注目すると

![](_page_27_Diagram_25.jpeg)

といういわゆるパスカルの三角形と呼ばれるものになる。この三角形をなす各数は、それぞれ左上、右上の数の和となっている（左端は右上のみ、右端は左上のみの数をそのまま受け継ぐ）。

実際、 $(a+b)^4 = (a+b)(a+b)^3 = (a+b)(a^3 + 3a^2b + 3ab^2 + b^3)$  を展開すれば、 $a^4$  となるのは  $a \times a^3$  の組み合わせのみ。 $a^3b$  となるのは  $b \times a^3$  と  $a \times 3a^2b$  の組み合わせで、その係数は 1 と 3 を合わせた 4 となる。また  $a^2b^2$  となるのは  $b \times 3a^2b$  と  $a \times 3ab^2$  の組み合わせで、その係数は 3 と 3 を合わせた 6 となり、このような関係が一般に成り立つことになる。

このことを、展開後の各項の係数を  $c_k^{(n)} a^{n-k} b^k$  のようにして数式で表すと以下のようになる。

$$(a+b)^n = c_0^{(n)} a^n + c_1^{(n)} a^{n-1}b + c_2^{(n)} a^{n-2}b^2 + \dots + c_{n-1}^{(n)} ab^{n-1} + c_n^{(n)} b^n$$

および

$$(a+b)^{n+1} = c_0^{(n+1)} a^{n+1} + c_1^{(n+1)} a^n b + c_2^{(n+1)} a^{n-1}b^2 + \dots + c_n^{(n+1)} ab^n + c_{n+1}^{(n+1)} b^{n+1}$$

に対して

$$c_0^{(n+1)} = c_0^{(n)} (= c_0^{(0)} = 1), \quad c_k^{(n+1)} = c_{k-1}^{(n)} + c_k^{(n)}, \quad c_{n+1}^{(n+1)} = c_n^{(n)} (= c_0^{(0)} = 1) \quad (2-6-1)$$

という関係が任意の  $n > 0$  に対して成り立つ。

この 二項展開の一般項を表すものが**二項定理**と呼ばれるもので、以下のような式となる<sup>15</sup>。

$$(a+b)^n = \sum_{k=0}^n c_k a^{n-k} b^k \quad (2-6-2)$$

 $(a+b)^n$  は  $(a+b)$  が  $n$  個掛け合わされたものであり、展開された際の  $a^{n-k} b^k$  の項は、 $n$  個ある  $(a+b)(a+b) \dots (a+b)$  の中から  $k$  個の  $b$  を選ぶ組み合わせの数だけあることになるので（選ばれなかった  $n-k$  個からは必ず  $a$  が選ばれる）その係数は「 $n$  個の中から  $k$  個を取り出

<sup>15</sup> 式の右辺は総和記号と呼ばれるもので表されている。付録 2 : 総和記号 参照

す組み合わせの数」を表す  ${}_nC_k$  ( $\binom{n}{k}$ )とも書かれる) となり、(2-6-2)式を得る。

この  ${}_nC_k$  の値は以下のようにして求まる。

 $n$  個から  $k$  個を取り出す最初の 1 個目は  $n$  通りの選び方があり、2 個目は  $n-1$  通り、最後の  $k$  個目は  $n-k+1$  通り選び方があり、組み合わせると  $n(n-1)(n-2)\cdots(n-k+1) = \frac{n!}{(n-k)!}$  通りとなるが、 $k$  個を取り出す順番にはよらないので、最終的な値は  ${}_nC_k = \frac{n!}{(n-k)!k!}$  通りとなる。

(2-6-1) 式の  $c_k^{(n)}$  は (2-6-2) 式の  ${}_nC_k$  に対応するものであり、(2-6-1) 式が  $c_k^{(n)} = {}_nC_k = \frac{n!}{(n-k)!k!}$  として実際に成り立つことは  $0! \equiv 1$  に注意して以下のように示される。

$${}_{n+1}C_0 = \frac{(n+1)!}{(n+1)!0!} = 1, \quad {}_nC_0 = \frac{n!}{n!0!} = 1, \quad {}_{n+1}C_{n+1} = \frac{(n+1)!}{0!(n+1)!} = 1, \quad {}_nC_n = \frac{n!}{0!n!} = 1$$

$$\begin{aligned} {}_{n+1}C_k &= \frac{(n+1)!}{(n+1-k)!k!} = \frac{(n+1)n!}{(n-k+1)!k!} = \frac{\{(n-k+1)+k\}n!}{(n-k+1)!k!} \\ &= \frac{n!}{(n-k)!k!} + \frac{n!}{(n-k+1)!(k-1)!} = {}_nC_k + {}_nC_{k-1} \quad \blacksquare \end{aligned}$$

<span id="page-28-0"></span>

### 【2-7】 付録 2 : 総和記号

数列の総和を示す記号を**総和記号**といいギリシャ文字の大文字のΣ (シグマ) で表す。

通常以下のように

$$\sum_{i=1}^n a_i \equiv a_1 + a_2 + \cdots + a_n$$

を意味する。 $a_1 + a_2 + \cdots + a_n$  の表記は具体的ではあるが、式中で頻繁に出てくると冗長で式全体の可読性を損なうため、このようなコンパクトな表記法が存在する。慣れると式の見通しが良くなりとても便利（かつ、めっちゃ強力）なので、ぜひ慣れて頂きたい。本講座内でもよく使われる。

総和記号の主な性質をあげた。比較的複雑な式の場合、これらを駆使して式変形が行われる。

(i) 線形性

$$\sum_{i=1}^n (a_i + b_i) = \sum_{i=1}^n a_i + \sum_{i=1}^n b_i, \quad \sum_{i=1}^n ka_i = k \sum_{i=1}^n a_i$$

(ii) 和の順番

基本的には内側から順に和を取る。以下はその例で

$$\begin{aligned} \sum_{i=1}^n \sum_{j=1}^i a_j &= \sum_{i=1}^n (a_1 + a_2 + \cdots + a_i) \\ &= (a_1) + (a_1 + a_2) + (a_1 + a_2 + a_3) + \cdots + (a_1 + a_2 + \cdots + a_n) \end{aligned}$$

(iii) 多重和の交換 (和の順番の入れ替え)

(ii) 和の順番 の例のように添字の範囲に依存性がある等の場合を除き)

添字が独立している場合 (有限和では) 和の順番に依らない。

$$\sum_{i=1}^n \sum_{j=1}^m a_{ij} = \sum_{j=1}^m \sum_{i=1}^n a_{ij}$$

例) 以下の 2 式は等しい

$$\sum_{i=1}^2 \sum_{j=1}^3 a_{ij} = \sum_{i=1}^2 (a_{i1} + a_{i2} + a_{i3}) = (a_{11} + a_{12} + a_{13}) + (a_{21} + a_{22} + a_{23})$$

$$\sum_{j=1}^3 \sum_{i=1}^2 a_{ij} = \sum_{j=1}^3 (a_{1j} + a_{2j}) = (a_{11} + a_{21}) + (a_{12} + a_{22}) + (a_{13} + a_{23})$$

応用) 添字の範囲が共通な場合など、一つの総和記号に複数の添字をまとめる略記法

$$\sum_{i,j=1}^n a_{ij} \equiv \sum_{i=1}^n \sum_{j=1}^n a_{ij}$$

(iv) 和の対象の分解・結合

乗法の分配則 :  $(a+b)(c+d) = ac + ad + bc + bd$  に基づく

$$\sum_{i=1}^n a_i \sum_{j=1}^m b_j = \sum_{i=1}^n \sum_{j=1}^m a_i b_j$$

例) 以下の 2 式は等しい

$$\sum_{i=1}^2 a_i \sum_{j=1}^3 b_j = (a_1 + a_2)(b_1 + b_2 + b_3) = a_1 b_1 + a_1 b_2 + a_1 b_3 + a_2 b_1 + a_2 b_2 + a_2 b_3$$

$$\sum_{i=1}^2 \sum_{j=1}^3 a_i b_j = \sum_{i=1}^2 (a_i b_1 + a_i b_2 + a_i b_3) = a_1 b_1 + a_1 b_2 + a_1 b_3 + a_2 b_1 + a_2 b_2 + a_2 b_3$$

<span id="page-29-0"></span>**【2-8】 付録 3 :  $\sin \theta / \theta \rightarrow 1$  ( $\theta \rightarrow 0$ ) の証明**

 $0 < \theta < 1$  の時に  $\frac{\sin \theta}{\theta} \rightarrow 1$  ( $\theta \rightarrow 0$ ) となることを示す。

図は  $|\overline{OA}| = |\overline{OB}| = 1$  内角  $\theta$  の扇型  $OAB$  で、 $B$  から  $\overline{OA}$  に下ろした垂線の足を  $D$ 、 $A$  から伸ばした接線と  $\overline{OB}$  を伸ばした直線との交点を  $C$  とする。

図より  $|\overline{BD}| = \sin \theta$ 、 $|\overline{CA}| = \tan \theta$  となる。

 $\triangle OAB$ , 扇型  $OAB$ ,  $\triangle OAC$  の面積はそれぞれ  $\frac{1}{2} \sin \theta$ ,  $\frac{1}{2} \theta$ ,  $\frac{1}{2} \tan \theta$  となり、図よりその大小関係は  $\frac{1}{2} \sin \theta < \frac{1}{2} \theta < \frac{1}{2} \tan \theta$  となる。これにより  $\sin \theta < \theta$  および  $\theta < \frac{\sin \theta}{\cos \theta}$  がいえて、これからさらに  $\cos \theta < \frac{\sin \theta}{\theta} < 1$  がいえ、 $\theta \rightarrow 0$  のとき  $\cos \theta \rightarrow 1$  と、はさみうちの原理より  $\frac{\sin \theta}{\theta} \rightarrow 1$  となる。■  
またこれにより  $\cos \theta \rightarrow 1$ ,  $\sin \theta \rightarrow \theta$  ( $\theta \rightarrow 0$ ) となることがいえる。

![](_page_29_Diagram_41.jpeg)

<span id="page-30-0"></span>**【2-9】 付録 4 : 三角関数の各公式の証明**

○加法定理 (2-3-1) 式の証明

【証明】

図のように単位円上の 2 点 A,B を x 軸からのなす角が  $\alpha, \beta$  となるように  
とると、それぞれの座標値は  $A(\cos \alpha, \sin \alpha), B(\cos \beta, \sin \beta)$  となる。

 $\overline{AB}$ の長さの 2 乗は余弦定理により

$$\begin{aligned} |\overline{AB}|^2 &= |\overline{OA}|^2 + |\overline{OB}|^2 - 2|\overline{OA}||\overline{OB}| \cos(\alpha - \beta) \\ &= 1 + 1 - 2 \cos(\alpha - \beta) \\ &= 2(1 - \cos(\alpha - \beta)) \end{aligned}$$

一方、座標値によっても求められ

$$\begin{aligned} |\overline{AB}|^2 &= (\cos \alpha - \cos \beta)^2 + (\sin \alpha - \sin \beta)^2 \\ &= \cos^2 \alpha + \sin^2 \alpha + \cos^2 \beta + \sin^2 \beta \\ &\quad - 2 \cos \alpha \cos \beta - 2 \sin \alpha \sin \beta \\ &= 2\{1 - (\cos \alpha \cos \beta + \sin \alpha \sin \beta)\} \\ \therefore \cos(\alpha - \beta) &= \cos \alpha \cos \beta + \sin \alpha \sin \beta \quad (#1) \end{aligned}$$

(#1)式より

$$\begin{aligned} \cos(\alpha + \beta) &= \cos\{\alpha - (-\beta)\} \\ &= \cos \alpha \cos(-\beta) + \sin \alpha \sin(-\beta) \\ &= \cos \alpha \cos \beta - \sin \alpha \sin \beta \quad (#2) \end{aligned}$$

基本性質  $\cos\left(\frac{\pi}{2} - \theta\right) = \sin \theta$  および (#1)式より

$$\begin{aligned} \sin(\alpha + \beta) &= \cos\left\{\frac{\pi}{2} - (\alpha + \beta)\right\} \\ &= \cos\left\{\left(\frac{\pi}{2} - \alpha\right) - \beta\right\} \\ &= \cos\left(\frac{\pi}{2} - \alpha\right) \cos \beta + \sin\left(\frac{\pi}{2} - \alpha\right) \sin \beta \\ &= \sin \alpha \cos \beta + \cos \alpha \sin \beta \quad (#3) \end{aligned}$$

(#3)式より

$$\begin{aligned} \sin(\alpha - \beta) &= \sin\{\alpha + (-\beta)\} \\ &= \sin \alpha \cos(-\beta) + \cos \alpha \sin(-\beta) \\ &= \sin \alpha \cos \beta - \cos \alpha \sin \beta \quad (#4) \end{aligned}$$

(#1),(#2),(#3),(#4)式より

$$\begin{aligned} \tan(\alpha \pm \beta) &= \frac{\sin(\alpha \pm \beta)}{\cos(\alpha \pm \beta)} \\ &= \frac{\sin \alpha \cos \beta \pm \cos \alpha \sin \beta}{\cos \alpha \cos \beta \mp \sin \alpha \sin \beta} \\ &= \frac{\tan \alpha \pm \tan \beta}{1 \mp \tan \alpha \tan \beta} \quad (#5) \end{aligned}$$

以上、(#1),(#2),(#3),(#4),(#5)式より (2-3-1) 式は示された。■

![](_page_30_Figure_38.jpeg)

### ○倍角の公式 (2-3-2) 式の証明

#### 【証明】

加法定理 (2-3-1) において、 $\beta = \alpha$  とする。

$$\sin 2\alpha = \sin \alpha \cos \alpha + \cos \alpha \sin \alpha = 2 \sin \alpha \cos \alpha \quad (#1)$$

$$\sin^2 \alpha + \cos^2 \alpha = 1 \text{ も用いて}$$

$$\begin{aligned} \cos 2\alpha &= \cos \alpha \cos \alpha - \sin \alpha \sin \alpha = \cos^2 \alpha - \sin^2 \alpha \\ &= 1 - 2 \sin^2 \alpha = 2 \cos^2 \alpha - 1 \quad (#2) \end{aligned}$$

$$\tan 2\alpha = \frac{\tan \alpha + \tan \alpha}{1 - \tan \alpha \tan \alpha} = \frac{2 \tan \alpha}{1 - \tan^2 \alpha} \quad (#3)$$

以上、(#1),(#2),(#3)式より (2-3-2) 式は示された。■

### ○半角の公式 (2-3-3) 式の証明

#### 【証明】

倍角の公式  $\cos 2\alpha = 1 - 2 \sin^2 \alpha = 2 \cos^2 \alpha - 1$  において、 $\alpha \rightarrow \alpha/2$  に置き換えると

$$\cos \alpha = 1 - 2 \sin^2 \frac{\alpha}{2}, \quad \cos \alpha = 2 \cos^2 \frac{\alpha}{2} - 1$$

それぞれ整理して

$$\sin^2 \frac{\alpha}{2} = \frac{1 - \cos \alpha}{2}, \quad \cos^2 \frac{\alpha}{2} = \frac{1 + \cos \alpha}{2} \quad (#1)$$

この(#1)式を辺々割ると

$$\tan^2 \frac{\alpha}{2} = \frac{\sin^2 \frac{\alpha}{2}}{\cos^2 \frac{\alpha}{2}} = \frac{1 - \cos \alpha}{1 + \cos \alpha} \quad (#2)$$

以上、(#1),(#2)より (2-3-3) 式は示された。■

○積和の公式 (2-3-4) の証明【証明】加法定理  $\sin(\alpha + \beta) = \sin \alpha \cos \beta + \cos \alpha \sin \beta$ ,  $\sin(\alpha - \beta) = \sin \alpha \cos \beta - \cos \alpha \sin \beta$  を

$$\text{辺々足すと } \sin(\alpha + \beta) + \sin(\alpha - \beta) = 2 \sin \alpha \cos \beta$$

$$\therefore \sin \alpha \cos \beta = \frac{1}{2}\{\sin(\alpha + \beta) + \sin(\alpha - \beta)\} \quad (#1)$$

加法定理  $\cos(\alpha + \beta) = \cos \alpha \cos \beta - \sin \alpha \sin \beta$ ,  $\cos(\alpha - \beta) = \cos \alpha \cos \beta + \sin \alpha \sin \beta$  を

$$\text{辺々足すと } \cos(\alpha + \beta) + \cos(\alpha - \beta) = 2 \cos \alpha \cos \beta$$

$$\therefore \cos \alpha \cos \beta = \frac{1}{2}\{\cos(\alpha + \beta) + \cos(\alpha - \beta)\} \quad (#2)$$

同様に辺々引くと  $\cos(\alpha + \beta) - \cos(\alpha - \beta) = -2 \sin \alpha \sin \beta$ 

$$\therefore \sin \alpha \sin \beta = -\frac{1}{2}\{\cos(\alpha + \beta) - \cos(\alpha - \beta)\} \quad (#3)$$

以上、(#1),(#2),(#3)より (2-3-4)式は示された。■

○和積の公式 (2-3-5) の証明【証明】積和の公式  $\sin \alpha \cos \beta = \frac{1}{2}\{\sin(\alpha + \beta) + \sin(\alpha - \beta)\}$  に、 $\alpha = \frac{x+y}{2}, \beta = \frac{x-y}{2}$  を代入すると

$$\sin \frac{x+y}{2} \cos \frac{x-y}{2} = \frac{1}{2} \left\{ \sin \left( \frac{x+y}{2} + \frac{x-y}{2} \right) + \sin \left( \frac{x+y}{2} - \frac{x-y}{2} \right) \right\} = \frac{1}{2} (\sin x + \sin y)$$

$$\therefore \sin x + \sin y = 2 \sin \frac{x+y}{2} \cos \frac{x-y}{2} \quad (#1)$$

同様に  $\alpha = \frac{x-y}{2}, \beta = \frac{x+y}{2}$  を代入すると

$$\sin \frac{x-y}{2} \cos \frac{x+y}{2} = \frac{1}{2} \left\{ \sin \left( \frac{x-y}{2} + \frac{x+y}{2} \right) + \sin \left( \frac{x-y}{2} - \frac{x+y}{2} \right) \right\} = \frac{1}{2} (\sin x + \sin(-y))$$

$$\therefore \sin x - \sin y = 2 \cos \frac{x+y}{2} \sin \frac{x-y}{2} \quad (#2)$$

積和の公式  $\cos \alpha \cos \beta = \frac{1}{2}\{\cos(\alpha + \beta) + \cos(\alpha - \beta)\}$  に、 $\alpha = \frac{x+y}{2}, \beta = \frac{x-y}{2}$  を代入すると

$$\cos \frac{x+y}{2} \cos \frac{x-y}{2} = \frac{1}{2} \left\{ \cos \left( \frac{x+y}{2} + \frac{x-y}{2} \right) + \cos \left( \frac{x+y}{2} - \frac{x-y}{2} \right) \right\} = \frac{1}{2} (\cos x + \cos y)$$

$$\therefore \cos x + \cos y = 2 \cos \frac{x+y}{2} \cos \frac{x-y}{2} \quad (#3)$$

積和の公式  $\sin \alpha \sin \beta = -\frac{1}{2}\{\cos(\alpha + \beta) - \cos(\alpha - \beta)\}$  に、 $\alpha = \frac{x+y}{2}, \beta = \frac{x-y}{2}$  を代入すると

$$\sin \frac{x+y}{2} \sin \frac{x-y}{2} = -\frac{1}{2} \left\{ \cos \left( \frac{x+y}{2} + \frac{x-y}{2} \right) - \cos \left( \frac{x+y}{2} - \frac{x-y}{2} \right) \right\} = -\frac{1}{2} (\cos x - \cos y)$$

$$\therefore \cos x - \cos y = -2 \sin \frac{x+y}{2} \sin \frac{x-y}{2} \quad (#4)$$

○合成の公式 (2-3-6) の証明

【証明】

$$a \sin \theta + b \cos \theta = \sqrt{a^2 + b^2} \left( \frac{a}{\sqrt{a^2 + b^2}} \sin \theta + \frac{b}{\sqrt{a^2 + b^2}} \cos \theta \right)$$

となるが、 $\left( \frac{a}{\sqrt{a^2 + b^2}} \right)^2 + \left( \frac{b}{\sqrt{a^2 + b^2}} \right)^2 = 1$  なので、ある角  $\alpha, \beta$  ( $-\pi \leq \alpha, \beta \leq \pi$ ) を用いて

$$\frac{a}{\sqrt{a^2 + b^2}} = \cos \alpha, \frac{b}{\sqrt{a^2 + b^2}} = \sin \alpha \text{ または } \frac{a}{\sqrt{a^2 + b^2}} = \sin \beta, \frac{b}{\sqrt{a^2 + b^2}} = \cos \beta$$

と書くことができる。

以下、加法定理を用いると

前者の場合

$$a \sin \theta + b \cos \theta = \sqrt{a^2 + b^2} (\cos \alpha \sin \theta + \sin \alpha \cos \theta) = \sqrt{a^2 + b^2} \sin(\theta + \alpha)$$

後者の場合

$$a \sin \theta + b \cos \theta = \sqrt{a^2 + b^2} (\sin \beta \sin \theta + \cos \beta \cos \theta) = \sqrt{a^2 + b^2} \cos(\theta - \beta)$$

となる。以上により (2-3-6) 式は示された。■

## 【第3講】ベクトル

<span id="page-34-1"></span><span id="page-34-0"></span>

### 【3-1】はじめに

ベクトルは、言うまでもなく理学・工学あらゆる分野で応用されており、その性質を理解し使いこなせることが求められる。また幾何ベクトルとしてのベクトルだけでなく、抽象化することで他にもさまざまなモノがベクトルとして認識され、ベクトルで得られた様々な知見が応用されている。ベクトルの概念はもともと線形性<sup>16</sup>を持っており、行列と共に線形代数の基礎をなし、応用範囲はさらに広がっている。

本講では、まず幾何ベクトルの性質を振り返り、抽象化の結果ベクトルとして仲間入りした例を紹介、またベクトルの線形性にも着目しながら線形代数の基礎の基礎を学んでいく。

<span id="page-34-2"></span>

### 【3-2】ベクトルがもつ性質

#### 【3-2-1】ベクトル自体がもつ性質

幾何ベクトルとは、平面あるいは空間内の「大きさ」と「向き」を持った量とされ、

始点  $P$  から終点  $Q$  へ向かう「有向線分」 $\vec{PQ}$  として定義された。また互いに大きさと向きが等しい（つまり平行移動して一致する）ベクトルは同一視されることから、始点や終点を省略した  $\vec{a} = \vec{PQ}$  などとも表記していた。

これから幾何ベクトル以外にもベクトルの概念を広げていくので、ベクトルを表す記号を  $a$  のように太文字で書き、以降特に必要のない限り、統一して用いることとする。

幾何ベクトルに対し、以下のような演算：**加法とスカラー積**が定義される。

![](_page_34_Picture_29.jpeg)

・加法：ベクトル  $a$  の終点に、加えるベクトル  $b$  の始点を一致させるように平行移動させたとき、  $a$  の始点から  $b$  の終点に向かうベクトルとして定義され、  $a + b$  と表す。

・スカラー積：ベクトル  $a$  の大きさを  $k$  倍(実数)したものとなる。

 $k < 0$  の場合：逆向き、 $k = 0$  の場合：零ベクトルとなる。

加法： $a + b$       スカラー積： $a \rightarrow ka$ 

当たり前過ぎて意識しないが、この加法とスカラー積を任意のベクトルに対して行った結果がまたベクトルとなるという閉じた演算になっている点が重要となる。

加法には以下の性質がある事が図により示される。

<sup>16</sup> 例：関数  $f(x)$  が  $f(x + y) = f(x) + f(y)$ ,  $f(kx) = kf(x)$  という性質を持つとき、線形であるという

![](_page_35_Diagram_46.jpeg)

交換則  
 $a + b = b + a$ 

![](_page_35_Diagram_48.jpeg)

結合則  
 $(a + b) + c = a + (b + c)$ 

![](_page_35_Diagram_50.jpeg)

零ベクトルの存在  
 $a + 0 = a$ 

![](_page_35_Diagram_52.jpeg)

逆ベクトルの存在  
 $a + (-a) = 0$ 

またスカラー積には以下の性質がある事が下図により示される。

これらをまとめた結果が以下となる。

● 幾何ベクトルの性質

加法

- (i)  $a + b = b + a$  (交換則)
- (ii)  $(a + b) + c = a + (b + c)$  (結合則)
- (iii)  $a + 0 = a$  (零ベクトルの存在)
- (iv)  $a + (-a) = 0$  (逆ベクトルの存在)

![](_page_35_Diagram_59.jpeg)

分配則

 $k(a + b) = ka + kb$   
 (3 - 2 - 1)

スカラー積

- (v)  $k(a + b) = ka + kb$  (分配則)

**[3-2-2] ベクトルの組がもつ性質**

● 線形結合（または一次結合）の定義

ベクトルの組  $a_1, a_2, \dots, a_m$  とスカラー  $k_1, k_2, \dots, k_m$  において、以下のようなスカラー積されたベクトルの和をこれらのベクトルの  $(k_1, k_2, \dots, k_m)$  を係数とする）**線形結合**（一次結合）という。

 $k_1 a_1 + k_2 a_2 + \dots + k_m a_m$  (3 - 2 - 2)

例として 3 次元空間内で考えてみる。図は 3 次元空間における 2 本のベクトル  $a_1, a_2$  での、係数  $k_1, k_2$  による線形結合を示している。図をみると、 $a_1, a_2$  が「乗っている」平面上に  $k_1 a_1, k_2 a_2, k_1 a_1 + k_2 a_2$  の各ベクトルが全て同様に「乗っている」ことが直観的に分かる。

![](_page_35_Diagram_69.jpeg)

また係数  $k_1, k_2$  の値を連続的に変化させていけば、線形結合されたベクトル  $k_1 a_1 + k_2 a_2$  がその平面上の全ての点を「指しそうだ」という事も見て取れる。この場合ベクトル  $a_1, a_2$  が「張る」平面という表現をする。

ここでもう一本のベクトル  $a_3$  を加えてみる。

![](_page_36_Picture_20.jpeg)

上図の左側では  $a_3$  は  $a_1, a_2$  が張る平面上にあり、右側では平面上にない向きをもつとする。

新たな線形結合  $k_1 a_1 + k_2 a_2 + k_3 a_3$  は左側と右側で明らかに異なる結果となる。

左側では、ベクトル  $a_3$  は  $a_1, a_2$  の線形結合で表され ( $a_3 = k_1 a_1 + k_2 a_2$  となる、少なくともどちらかは 0 でない  $k_1, k_2$  が存在する)、3 本のベクトルは  $a_3$  が加わる前と同じ平面を張る。右側では、ベクトル  $a_3$  は  $a_1, a_2$  の線形結合で表すことができず ( $a_3 = k_1 a_1 + k_2 a_2$  となる  $k_1, k_2$  が存在しない)、3 本のベクトルは  $a_3$  が加わる前と異なり 3 次元空間を張ることになる。この違いを以下のように定式化する。

●線形独立と線形従属 (または一次独立、一次従属)

あるベクトルの組  $a_1, a_2, \dots, a_m$  に対して、スカラー  $c_1, c_2, \dots, c_m$  を用いて

$$c_1 a_1 + c_2 a_2 + \dots + c_m a_m = \mathbf{0} \quad (3-2-3)$$

という式を考えると、この式は

$$c_1 = c_2 = \dots = c_m = 0 \quad (3-2-4)$$

という自明な解を持つが、(3-2-3)式が

・唯一この自明な解(3-2-4)しか持たない場合：

これらのベクトルの組は線形独立 (一次独立) であるという。

・そうでない場合 (他に解をもつ場合)：

これらのベクトルの組は線形従属 (一次従属) であるという。

定義よりベクトルの組の中に零ベクトルが一つでもあると線形従属となることに注意。

線形結合の例であげた 3 本のベクトル  $a_1, a_2, a_3$  について、このことを確認してみよう。

まずこの例の  $a_1, a_2$  は線形独立であることがわかる。もし線形従属なら、 $c_1 a_1 + c_2 a_2 = \mathbf{0}$  の式は、 $c_1, c_2$  の少なくともどちらかは 0 でない事になり、これは  $a_1 = -\frac{c_2}{c_1} a_2$  または  $a_2 = -\frac{c_1}{c_2} a_1$  と書けることを意味している。これでは「平面」を張ることはできないので、 $a_1, a_2$  は線形独立である。これに  $a_3$  を加えた場合、次のようになる。

左側の例では、少なくともどちらかは 0 でない  $k_1, k_2$  を用いて  $a_3 = k_1 a_1 + k_2 a_2$  と表すことができた。これは  $k_1 a_1 + k_2 a_2 - a_3 = 0$  と書けるので、(3-2-3)式が  $c_1 = k_1, c_2 = k_2, c_3 = -1$  という解を持つことを意味している。従って左側の例は線形従属となる。

右側の例で、 $c_1 a_1 + c_2 a_2 + c_3 a_3 = 0$  を考える。もし  $c_3 \neq 0$  なら、 $a_3 = -\frac{c_1}{c_3} a_1 - \frac{c_2}{c_3} a_2$  と書け、 $a_3$  が  $a_1, a_2$  の線形結合で表せないことに矛盾、従って  $c_3 = 0$  となり、 $c_1 a_1 + c_2 a_2 = 0$  を得るが、 $a_1, a_2$  は線形独立だったので  $c_1 = c_2 = 0$  となる。従って右側の例は線形独立となる。

#### ●基底、次元、座標系

上記の例のように線形独立なベクトルの組は、線形結合により2本なら「平面」を、3本なら「空間」を張る。この線形独立なベクトルの組が「平面」や「空間」上の任意のベクトルを線形結合で表せるとき、「平面」や「空間」の**基底**と呼ぶ。この線形結合での表し方は一意となる。

• 線形独立なベクトルの組によるベクトルの線形結合での表し方は一意 (3 - 2 - 5)

 $\therefore a = c_1 a_1 + \dots + c_n a_n = c'_1 a_1 + \dots + c'_n a_n$  のとき  $(c_1 - c'_1) a_1 + \dots + (c_n - c'_n) a_n = 0$  となり  
 $a_1, \dots, a_n$  は線形独立なので  $c_1 - c'_1 = 0, \dots, c_n - c'_n = 0 \therefore c'_1 = c_1, \dots, c'_n = c_n$  がいえる。■

また張られる「平面」や「空間」に対して基底のとり方は無数にあるが、どのようなとり方をしてもその数は同じであり、この数を**次元**という。上記は4次元以上の高次元でも成り立つ。

 $n$ 次元空間の各点を指すベクトルを基底の線形結合で表すとその係数は一意となるので、この係数の組を用いて各点を表すことができる。これを**座標系**といい、その係数の組を**座標値**という。ここまで幾何ベクトルの場合、暗に直交座標系を張れることを前提としてきた。例えば平面の場合、 $e_x = (1,0), e_y = (0,1)$  のような自然な直交座標系をなす基底を選ぶことができる。このような基底を**標準基底**（あるいは**正規直交基底**）という。

<span id="page-37-0"></span>

### 【3-3】内積

#### 【3-3-1】定義

ベクトル  $a = \sum_{i=1}^n a_i e_i, b = \sum_{j=1}^n b_j e_j$  ( $e_i$  は標準基底) において<sup>17</sup>

$$a \cdot b \equiv \sum_{i=1}^n a_i b_i \tag{3-3-1}$$

となるスカラー値をベクトルの（標準）**内積**という。（※なお本講ではベクトルの成分が実数である実ベクトルのみを取り扱う。）

自身との内積の値が  $a \cdot a = \sum_{i=1}^n a_i^2 \geq 0$  であり、0になるのは  $a = 0$  の時のみとなる事よりベクトルの**ノルム**（大きさ）を以下のように定義する。

<sup>17</sup> (x,y)でなく(1,2)で表す。初見で分かりにくい場合は、nを2や3として総和を展開してみよう。

$$\|a\| \equiv \sqrt{a \cdot a} \quad (\|a\| = 0 \Leftrightarrow a = 0) \quad (3-3-2)$$

また標準基底同士の内積は

$$e_i \cdot e_j = \delta_{ij} \quad (3-3-3)$$

となる<sup>18</sup>。ここで  $\delta_{ij}$  はクロネッカーのデルタと呼ばれる記号で以下のように定義される。

$$\delta_{ij} = \begin{cases} 1 & \text{if } i = j \\ 0 & \text{if } i \neq j \end{cases} \quad (3-3-4)$$

これらより、ベクトル  $a = \sum_{i=1}^n a_i e_i, b = \sum_{j=1}^n b_j e_j$  の内積は

$$a \cdot b = \left( \sum_{i=1}^n a_i e_i \right) \cdot \left( \sum_{j=1}^n b_j e_j \right) = \sum_{i,j=1}^n a_i b_j e_i \cdot e_j = \sum_{i,j=1}^n a_i b_j \delta_{ij} = \sum_{i=1}^n a_i b_i \quad (3-3-5)$$

となり当然（標準）内積の定義と一致する。またベクトルと標準基底との内積は

$$e_i \cdot a = e_i \cdot \left( \sum_{j=1}^n a_j e_j \right) = \sum_{j=1}^n a_j e_i \cdot e_j = \sum_j a_j \delta_{ij} = a_i \quad (3-3-6)$$

となるように、ベクトルにおけるその標準基底の成分を取り出す事に相当する。

### [3-3-2] 代数的性質

定義から明らかに成り立つ、以下の基本的な代数的性質がある。

- (i)  $a \cdot b = b \cdot a$
- (ii)  $a \cdot (b + c) = a \cdot b + a \cdot c$
- (iii)  $a \cdot (kb) = k a \cdot b$  ( $k$  はスカラー値) (3-3-7)
- (iv)  $a \cdot a \geq 0$  (等号は  $a = 0$  のときのみ)

(※(ii),(iii) の性質を合わせて線形性、また内積記号の左側でも成り立つことから**双線形性**という)

### [3-3-3] 幾何学的意味

幾何ベクトルにおいては、以下のような幾何学的意味をもつ。

#### ● 内積 $a \cdot b$

図のように、なす角が  $\theta$  のベクトル  $a, b$  において、 $a - b$  のノルムの 2 乗を考える。

$$\begin{aligned} \|a - b\|^2 &= (a - b) \cdot (a - b) \\ &= a \cdot a + b \cdot b - 2a \cdot b \\ &= \|a\|^2 + \|b\|^2 - 2a \cdot b \end{aligned}$$

一方、余弦定理より

$$\|a - b\|^2 = \|a\|^2 + \|b\|^2 - 2\|a\|\|b\| \cos \theta$$

両式より

$$a \cdot b = \|a\|\|b\| \cos \theta \quad (3-3-8)$$

![](_page_38_Picture_51.jpeg)

この式より、0 でないベクトル同士の内積が 0 となる場合、それらのベクトルは直交する事が分かる。

<sup>18</sup> むしろ、これは標準基底あるいは正規直交基底が満たすべき性質となる

#### ●円の接線の方程式

図のような、点  $O$  を中心とした半径  $r_0$  の円に点  $P_0$  で接する接線の方程式を考える。

この接線上の任意の点を  $P$  とし、それぞれの位置ベクトルを

$$\vec{OP_0} = \mathbf{r}_0, \vec{OP} = \mathbf{r} \text{ とする。このとき題意より } \|\mathbf{r}_0\| = r_0 \text{ である。}$$

 $\mathbf{r}_0$  はこの接線に対する法線ベクトルでもあり、

接線を表すベクトル  $\mathbf{r} - \mathbf{r}_0$  と直交するので

$$\mathbf{r}_0 \cdot (\mathbf{r} - \mathbf{r}_0) = 0$$

が成り立つ。従って

$$\mathbf{r}_0 \cdot \mathbf{r} = r_0^2$$

が求める式となる。

座標系を入れて座標値で表記すると、点  $O$  を原点として

点  $P(x, y), P_0(x_0, y_0)$  とすると

$$x_0x + y_0y = r_0^2$$

となる。

![](_page_39_Picture_49.jpeg)

(3-3-9)

#### ●球面の接平面の方程式

また上記はそのまま球面に接する接平面の方程式に拡張される。

すなわち上記において、円→球面、接線→接平面に

読み替えれば、そのまま成立する事がわかる（確かめよう）。

座標値では、点  $P(x, y), P_0(x_0, y_0) \rightarrow P(x, y, z), P_0(x_0, y_0, z_0)$ 

と読み替えることになり、

$$x_0x + y_0y + z_0z = r_0^2$$

となる。

点  $O, P_0, P$  を含む平面で切断すると、円と接線の関係になる（部分空間）からこのような事ができるのだが、もう一つ重要なことはベクトルの式が座標系によらずに成り立つからである。

![](_page_39_Picture_60.jpeg)

<span id="page-39-0"></span>

### 【3-4】抽象化されたベクトルの概念と例

これまで幾何ベクトルの性質を振り返ってきた。線形独立性や基底などのベクトルの組が持つ重要な性質は、(3-2-1)式にまとめられているような和とスカラー積の性質から導かれていることが分かる。逆に和とスカラー積が定義され、これらの性質を満たせば、線形独立性なども持つことになる。そこで (3-2-1)式の性質に、スカラー積の性質として

$$(vi) \quad (k+l)\mathbf{a} = k\mathbf{a} + l\mathbf{a} \quad (\text{分配則})$$

$$(vii) \quad k(l\mathbf{a}) = (kl)\mathbf{a} \quad (\text{結合則})$$

$$(viii) \quad 1\mathbf{a} = \mathbf{a} \quad (\text{単位元})$$

一積を定義できる対象をベクトルとみなすことで、ベクトルの概念が広げられる。ベクトルの集合のことを**ベクトル空間**といい、位置づけた公理を**ベクトル空間の公理**という。

また内積は、ベクトルの大きさやベクトル間の角度に関わる量であった。これも同様に内積の性質(3-3-7)式を公理とし、その性質を満たすような、上記のベクトル空間に自然に導入できる内積を定義して用いることとなる。内積が導入されたベクトル空間を**計量ベクトル空間**という。

拡張されたベクトル（ベクトル空間）の例をあげる。各公理を満たすことの確認は読者に任せる。

● 例 1 n 次元実数ベクトル空間 :  $\mathbb{R}^n$  (実数を n 個組にしたもの : 行列でのベクトル)

$$\text{ベクトル } \mathbf{a} = \begin{bmatrix} a_1 \\ a_2 \\ \vdots \\ a_n \end{bmatrix}, \mathbf{b} = \begin{bmatrix} b_1 \\ b_2 \\ \vdots \\ b_n \end{bmatrix}, \text{ スカラー } k \in \mathbb{R} \text{ に対して}$$

$$\text{和 } \mathbf{a} + \mathbf{b} = \begin{bmatrix} a_1 \\ a_2 \\ \vdots \\ a_n \end{bmatrix} + \begin{bmatrix} b_1 \\ b_2 \\ \vdots \\ b_n \end{bmatrix} \equiv \begin{bmatrix} a_1 + b_1 \\ a_2 + b_2 \\ \vdots \\ a_n + b_n \end{bmatrix} \quad \text{スカラー積 } k\mathbf{a} = k \begin{bmatrix} a_1 \\ a_2 \\ \vdots \\ a_n \end{bmatrix} \equiv \begin{bmatrix} ka_1 \\ ka_2 \\ \vdots \\ ka_n \end{bmatrix}$$

と定義することでベクトル空間の公理を満たす。ベクトルの成分を縦に並べたものである。

$$\text{標準基底 } \mathbf{e}_1 = \begin{bmatrix} 1 \\ 0 \\ \vdots \\ 0 \end{bmatrix}, \mathbf{e}_2 = \begin{bmatrix} 0 \\ 1 \\ \vdots \\ 0 \end{bmatrix}, \dots, \mathbf{e}_n = \begin{bmatrix} 0 \\ 0 \\ \vdots \\ 1 \end{bmatrix}$$

内積  $\mathbf{a} \cdot \mathbf{b} = a_1 b_1 + a_2 b_2 + \dots + a_n b_n$  も自然に定められる。

● 例 2 複素数の集合  $\mathbb{C}$ 

複素平面上で複素数の和はベクトルの和のような性質をもっていた。

ベクトル  $\mathbf{a} = a_1 + ia_2, \mathbf{b} = b_1 + ib_2, \text{ スカラー } k \in \mathbb{R}$  に対して

$$\text{和 } \mathbf{a} + \mathbf{b} = (a_1 + ia_2) + (b_1 + ib_2) \equiv (a_1 + b_1) + i(a_2 + b_2)$$

$$\text{スカラー積 } k\mathbf{a} = k(a_1 + ia_2) \equiv ka_1 + i ka_2$$

と定義することでベクトル空間の公理を満たす。

基底  $\mathbf{e}_1 = 1, \mathbf{e}_2 = i$ 

$$\text{内積 } \mathbf{a} \cdot \mathbf{b} \equiv \frac{1}{2}(\mathbf{a}\bar{\mathbf{b}} + \mathbf{b}\bar{\mathbf{a}}) = \frac{1}{2}\{(a_1 + ia_2)(b_1 - ib_2) + (b_1 + ib_2)(a_1 - ia_2)\} = a_1 b_1 + a_2 b_2$$

と定める。

(注 : 本講では内積の値も実数としたいので、このように定義した。複素数値を許す場合は

通常  $\mathbf{a} \cdot \mathbf{b} \equiv \mathbf{a}\bar{\mathbf{b}}$  と定義される。その場合、内積の性質も複素数に拡張される。)

● 例 3 [▼B] 1 変数実数値関数の集合 (少し高度な例)

和  $(f + g)(x) \equiv f(x) + g(x), \text{ スカラー積 } (kf)(x) \equiv kf(x), \text{ 内積 } \int f(x)g(x)dx$ 

と定めることでベクトル空間の公理を満たし、自然な内積として利用できる。基底として三角関数を用いる例を、第 6 講行列 III にて応用例として取り上げる。

<span id="page-41-0"></span>

### 【3-5】外積

#### 【3-5-1】定義<sup>19</sup>

ベクトルの外積は、3次元でのみ定義されるものであり、成分で表すと以下のようになる。

$$\mathbf{a} = a_1\mathbf{e}_1 + a_2\mathbf{e}_2 + a_3\mathbf{e}_3, \mathbf{b} = b_1\mathbf{e}_1 + b_2\mathbf{e}_2 + b_3\mathbf{e}_3 \quad \text{(において } (\mathbf{e}_1, \mathbf{e}_2, \mathbf{e}_3 \text{ は標準基底))}$$

$$\mathbf{a} \times \mathbf{b} \equiv (a_2b_3 - a_3b_2)\mathbf{e}_1 + (a_3b_1 - a_1b_3)\mathbf{e}_2 + (a_1b_2 - a_2b_1)\mathbf{e}_3 \quad (3-5-1)$$

となるベクトルをベクトルの**外積**という（規則性を見やすくするため添字は1,2,3とした）。

この定義を観察すると、成分と基底の積  $a_i b_k e_i$  の添字の組が  $(i, j, k) = (1,2,3), (2,3,1), (3,1,2)$  の場合が正、 $(1,3,2), (2,1,3), (3,2,1)$  の場合が負 の符号がついていることが分かる。

この正負の組は、どの2つの数字をその () 内で入れ替えても互いに移り変わる。

また最初の項  $(a_2b_3 - a_3b_2)\mathbf{e}_1$  に対して、1→2, 2→3, 3→1 とサイクリックに添字を入れ替えると第2項  $(a_3b_1 - a_1b_3)\mathbf{e}_2$  に、もう一度入れ替えると第3項  $(a_1b_2 - a_2b_1)\mathbf{e}_3$  に、さらに入れ替えると第1項に戻る。従って、外積の定義全体がサイクリックな添字の入れ替えで不変（入れ替えについて対称）となることが分かる。このような規則性を活かした成分表記に大変有用（且つ強力）な記法（**Levi-Civita**（**レヴィ=チヴィタ**）記号）があるので付録1にて紹介する。

#### 【3-5-2】代数的性質

定義より明らかに成り立つ、以下の基本的な代数的性質がある。

(i)  $\mathbf{a} \times \mathbf{b} = -\mathbf{b} \times \mathbf{a} \quad \therefore \mathbf{a} \times \mathbf{a} = \mathbf{0}$ 

(ii)  $(\mathbf{a} + \mathbf{b}) \times \mathbf{c} = \mathbf{a} \times \mathbf{c} + \mathbf{b} \times \mathbf{c} \quad (3-5-2)$ 

(iii)  $(k\mathbf{a}) \times \mathbf{b} = k(\mathbf{a} \times \mathbf{b})$  ( $k$  はスカラー値)

また上記基本性質以外に、以下のような公式が成り立つ。ここでは公式の記載にとどめ、その証明は付録2に掲載する。各証明は成分表記で地道に行う方法と、Levi-Civita 記号を用いて劇的にシンプル(且つ機械的)に示す方法の2種類で行う。いずれも上記定義で述べた規則性に基づく。

●スカラー三重積  $\mathbf{a} \cdot (\mathbf{b} \times \mathbf{c})$  で成り立つ公式

$$\mathbf{a} \cdot (\mathbf{b} \times \mathbf{c}) = \mathbf{b} \cdot (\mathbf{c} \times \mathbf{a}) = \mathbf{c} \cdot (\mathbf{a} \times \mathbf{b}) \quad (3-5-3)$$

●ベクトル三重積  $\mathbf{a} \times (\mathbf{b} \times \mathbf{c})$  で成り立つ公式

$$\mathbf{a} \times (\mathbf{b} \times \mathbf{c}) = (\mathbf{a} \cdot \mathbf{c})\mathbf{b} - (\mathbf{a} \cdot \mathbf{b})\mathbf{c} \quad (3-5-4)$$

●外積同士の内積  $(\mathbf{a} \times \mathbf{b}) \cdot (\mathbf{c} \times \mathbf{d})$  で成り立つ公式

$$(\mathbf{a} \times \mathbf{b}) \cdot (\mathbf{c} \times \mathbf{d}) = (\mathbf{a} \cdot \mathbf{c})(\mathbf{b} \cdot \mathbf{d}) - (\mathbf{a} \cdot \mathbf{d})(\mathbf{b} \cdot \mathbf{c}) \quad (3-5-5)$$

<sup>19</sup> 初めて外積を学ぶ読者は幾何学的意味から入る方が分かりやすいとは思う。[3-5-3] 参照。ただしこれを定義として成分表示 (3-5-1) を導くには (3-5-2)(ii) を幾何学的に示す必要があり初学者にはかえって難解かと思われる。

**[3-5-3] 幾何学的意味**

幾何ベクトルにおいては、以下のような幾何学的な意味を持つ。

●外積  $a \times b$ 

![](_page_42_Figure_26.jpeg)

・大きさ : ベクトルとしての  $a \times b$  のノルムの 2 乗により、 $a, b$  のなす角を  $\theta$  とすると

$$\begin{aligned} \|a \times b\|^2 &= (a \times b) \cdot (a \times b) \\ &= (a \cdot a)(b \cdot b) - (a \cdot b)^2 && (\because (3 - 5 - 5)) \\ &= \|a\|^2 \|b\|^2 (1 - \cos^2 \theta) \\ &= \|a\|^2 \|b\|^2 \sin^2 \theta \\ \therefore \|a \times b\| &= \|a\| \|b\| \sin \theta \end{aligned}$$

これは、ベクトル  $a, b$  が張る平行四辺形の面積と等しい。

・方向 :  $a \times b$  に対して、 $a, b$  とそれぞれ内積をとると

$$a \cdot (a \times b) = b \cdot (a \times a) = 0, \quad b \cdot (a \times b) = a \cdot (b \times b) = 0 \quad (\because (3 - 5 - 3))$$

より、 $a \times b$  は  $a, b$  どちらとも直交する。また定義より標準基底に対して

$$e_x \times e_y = e_z, \quad e_y \times e_z = e_x, \quad e_z \times e_x = e_y$$

が成り立つ事より、図のように、 $a$  を  $b$  に向けて回した時に右ねじが進む方を向く。

●スカラー三重積  $a \cdot (b \times c)$ 

![](_page_42_Figure_36.jpeg)

ベクトル  $a$  と  $b \times c$  との内積は、そのなす角を  $\theta$  とすると  $\|a\| \|b \times c\| \cos \theta$  であるが、 $\|b \times c\|$  に  $\|a\| \cos \theta$  を掛けたものと見ることもでき、これはベクトル  $b, c$  が張る平行四辺形の面積に、ベクトル  $a$  の高さを掛けたものと等しい。従って、スカラー三重積の値は、3 本のベクトルが張る平行六面体の符号付き体積と見なせる。

その符号はベクトル  $a$  と  $b \times c$  との向きの関係で決まり、図のようになす角  $\theta$  が  $\pi/2$  以下の場合に正となり、内積の符号を表す  $\cos \theta$  の符号が反映されることになる。またスカラー三重積の性質(3-5-3)式はこの幾何学的意味から向き付けに注意して成り立つことが分かる。

ベクトルの外積は、第 8 講 回転の表現 II で学ぶクォータニオンの積から自然に生まれたもので、煎じ詰めるとその意味で 3 次元でしか定義できない<sup>20</sup>。また  $n$  次元に拡張可能な外積に似た概念のひとつに「外積代数」<sup>21</sup>と呼ばれるものがあるが、それに近いものを次節にて学ぶ。

<sup>20</sup> 生まれる詳細は第 8 講で。ちなみにクォータニオン（四元数）の次は 8 次元での八元数が定義でき、7 次元空間では外積的なものは定義できるそうな。

<sup>21</sup> この節の外積（cross product）とは異なる「外積」であり、exterior product の訳語である。

<span id="page-43-0"></span>

### 【3-6】 n 本のベクトルが張る n 次元体積

応用として n 次元空間で n 本のベクトルが張る n 次元の体積に相当する「関数」を考える<sup>22</sup>。

外積の幾何学的意味の項で見たように、2 次元の場合は外積の大きさ、3 次元の場合はスカラー三重積にあたる量であり、これを n 次元に拡張したい。

#### 【3-6-1】 2 次元 : 2 次元体積 (面積)

![](_page_43_Picture_42.jpeg)

以下、図のようなベクトル  $a, b$  が張る面積を値にもつ、ベクトルを変数とする「関数」を  $D(a, b)$  とし、その性質を考える。

![](_page_43_Picture_44.jpeg)

(i) ベクトルの和に対して

 $a = a_1 + a_2$  のとき図のように平行四辺形  $OE'D'B$  と  $OEDB$  は底辺  $OB$  が共通で高さが等しいので、面積も等しい (面積 :  $D(a_1, b)$ )。  
 $CD'E'A$  と  $CDEA$  も同様 (面積 :  $D(a_2, b)$ )。従って

$$D(a_1 + a_2, b) = D(a_1, b) + D(a_2, b) \quad (b \text{ についても同様})$$

![](_page_43_Picture_48.jpeg)

(ii) スカラー積に対して

 $a$  を  $k$  倍すると面積も  $k$  倍となる

$$D(ka, b) = kD(a, b) \quad (b \text{ についても同様})$$

![](_page_43_Picture_52.jpeg)

(iii) 同じベクトルが張る面積は 0

$$D(a, a) = 0$$

またこれにより

$$\begin{aligned} 0 &= D(a + b, a + b) && (\because (iii)) \\ &= D(a, a + b) + D(b, a + b) && (\because (i)) \\ &= D(a, a) + D(a, b) + D(b, a) + D(b, b) && (\because (i)) \\ &= D(a, b) + D(b, a) && (\because (iii)) \\ \therefore D(b, a) &= -D(a, b) \end{aligned}$$

この面積は符号付きとなり、符号は張るベクトルの向き付けによる。

![](_page_43_Picture_58.jpeg)

(iv) 標準基底が張る面積を 1 とする

$$D(e_1, e_2) = 1$$

面積の大きさの単位および向き付けの定義となる。

<sup>22</sup> 次講以降の行列のダンジョンで戦うための武器を作る。今のうちに武器の経験値を上げておこう。

実はこの 4 つの性質 : ((i),(ii)は  $b$  についても同様)

- (i)  $D(\mathbf{a}_1 + \mathbf{a}_2, b) = D(\mathbf{a}_1, b) + D(\mathbf{a}_2, b)$  (3 - 6 - 1)
- (ii)  $D(k\mathbf{a}, b) = kD(\mathbf{a}, b)$  (3 - 6 - 2)
- (iii)  $D(\mathbf{a}, \mathbf{a}) = 0 \quad \therefore D(b, \mathbf{a}) = -D(\mathbf{a}, b)$  (3 - 6 - 3)
- (iv)  $D(\mathbf{e}_1, \mathbf{e}_2) = 1$  (3 - 6 - 4)

で、 $D(\mathbf{a}, b)$  の値は一意に定まる。実際、 $\mathbf{a} = a_1\mathbf{e}_1 + a_2\mathbf{e}_2$ ,  $b = b_1\mathbf{e}_1 + b_2\mathbf{e}_2$  のとき

$$\begin{aligned} D(\mathbf{a}, b) &= D(a_1\mathbf{e}_1 + a_2\mathbf{e}_2, b_1\mathbf{e}_1 + b_2\mathbf{e}_2) \\ &= D(a_1\mathbf{e}_1, b_1\mathbf{e}_1) + D(a_1\mathbf{e}_1, b_2\mathbf{e}_2) + D(a_2\mathbf{e}_2, b_1\mathbf{e}_1) + D(a_2\mathbf{e}_2, b_2\mathbf{e}_2) && (\because (i)) \\ &= a_1b_1D(\mathbf{e}_1, \mathbf{e}_1) + a_1b_2D(\mathbf{e}_1, \mathbf{e}_2) + a_2b_1D(\mathbf{e}_2, \mathbf{e}_1) + a_2b_2D(\mathbf{e}_2, \mathbf{e}_2) && (\because (ii)) \\ &= a_1b_2D(\mathbf{e}_1, \mathbf{e}_2) + a_2b_1D(\mathbf{e}_2, \mathbf{e}_1) && (\because (iii)) \\ &= (a_1b_2 - a_2b_1)D(\mathbf{e}_1, \mathbf{e}_2) && (\because (iiii)) \\ &= a_1b_2 - a_2b_1 && (\because (iv)) \end{aligned}$$

となるが、これは幾何学的に求まる符号付き面積  $\mathbf{a} \times \mathbf{b}$  の値を成分で表したものと一致する。

( $\mathbf{a} = (a_1, a_2, 0), \mathbf{b} = (b_1, b_2, 0)$  のときの  $\mathbf{a} \times \mathbf{b}$  の大きさとなる)

**[3-6-2] 3 次元 : 3 次元体積 (体積)**

![](_page_44_Picture_42.jpeg)

3 次元に素直に拡張する。この体積を表す  $D(\mathbf{a}, \mathbf{b}, \mathbf{c})$  も同様に以下の性質を持つ。((i)以外は明らか。(i)も  $b, c$  が張る平行四辺形の面積に  $\mathbf{a}_1, \mathbf{a}_2$  の高さを掛けた体積の和として成り立つ。)

![](_page_44_Picture_44.jpeg)

- (i)  $D(\mathbf{a}_1 + \mathbf{a}_2, \mathbf{b}, \mathbf{c}) = D(\mathbf{a}_1, \mathbf{b}, \mathbf{c}) + D(\mathbf{a}_2, \mathbf{b}, \mathbf{c})$  (3 - 6 - 5)
- (ii)  $D(k\mathbf{a}, \mathbf{b}, \mathbf{c}) = kD(\mathbf{a}, \mathbf{b}, \mathbf{c})$  (3 - 6 - 6)
- (iii)  $D(\mathbf{a}, \mathbf{a}, \mathbf{b}) = 0 \quad \therefore D(\mathbf{b}, \mathbf{a}, \mathbf{c}) = -D(\mathbf{a}, \mathbf{b}, \mathbf{c})$  (3 - 6 - 7)
- (iv)  $D(\mathbf{e}_1, \mathbf{e}_2, \mathbf{e}_3) = 1$  (3 - 6 - 8)

((i),(ii)は  $b, c$  についても同様。(iii)はどの 2 つが同じでも、どの 2 つを入れ替えてもという意味)

性質(iii),(iv)より、 $D(\mathbf{e}_i, \mathbf{e}_j, \mathbf{e}_k)$  ( $1 \leq i, j, k \leq 3$ ) は  $i, j, k$  の値が全て異なるとき非零の値をもち、変数部分が  $\mathbf{e}_1, \mathbf{e}_2, \mathbf{e}_3$  からの並び替えで符号が変わるだけで以下のような値をもつことになる。

$$D(\mathbf{e}_i, \mathbf{e}_j, \mathbf{e}_k) = \begin{cases} +1 & \text{if } (i, j, k) = (1,2,3), (2,3,1), (3,1,2) \\ -1 & \text{if } (i, j, k) = (1,3,2), (2,1,3), (3,2,1) \\ 0 & \text{other} \end{cases} \quad (3 - 6 - 9)$$

これは (3-7-1) 式である Levi-Civita 記号  $\varepsilon_{ijk}$  と全く同じことがわかる。

また同じように上記 4 つの性質のみで  $D(\mathbf{a}, \mathbf{b}, \mathbf{c})$  の値は一意に定まる。

実際  $\mathbf{a} = \sum_{i=1}^3 a_i \mathbf{e}_i, \mathbf{b} = \sum_{j=1}^3 b_j \mathbf{e}_j, \mathbf{c} = \sum_{k=1}^3 c_k \mathbf{e}_k$  のとき

$$\begin{aligned} D(\mathbf{a}, \mathbf{b}, \mathbf{c}) &= D \left( \sum_{i=1}^3 a_i \mathbf{e}_i, \sum_{j=1}^3 b_j \mathbf{e}_j, \sum_{k=1}^3 c_k \mathbf{e}_k \right) = \sum_{i,j,k=1}^3 a_i b_j c_k D(\mathbf{e}_i, \mathbf{e}_j, \mathbf{e}_k) \\ &= a_1 \sum_{j,k=1}^3 b_j c_k D(\mathbf{e}_1, \mathbf{e}_j, \mathbf{e}_k) + a_2 \sum_{j,k=1}^3 b_j c_k D(\mathbf{e}_2, \mathbf{e}_j, \mathbf{e}_k) + a_3 \sum_{j,k=1}^3 b_j c_k D(\mathbf{e}_3, \mathbf{e}_j, \mathbf{e}_k) \\ &= a_1(b_2 c_3 - b_3 c_2) D(\mathbf{e}_1, \mathbf{e}_2, \mathbf{e}_3) + a_2(b_3 c_1 - b_1 c_3) D(\mathbf{e}_2, \mathbf{e}_3, \mathbf{e}_1) + a_3(b_1 c_2 - b_2 c_1) D(\mathbf{e}_3, \mathbf{e}_1, \mathbf{e}_2) \\ &= \{a_1(b_2 c_3 - b_3 c_2) + a_2(b_3 c_1 - b_1 c_3) + a_3(b_1 c_2 - b_2 c_1)\} D(\mathbf{e}_1, \mathbf{e}_2, \mathbf{e}_3) \\ &= a_1(b_2 c_3 - b_3 c_2) + a_2(b_3 c_1 - b_1 c_3) + a_3(b_1 c_2 - b_2 c_1) \quad (3 - 6 - 10) \end{aligned}$$

**[3-6-3] n 次元 : n 次元体積**

n 次元に素直に拡張して

$$(i) \quad D(\mathbf{a}_1, \dots, \mathbf{a}_{i_1} + \mathbf{a}_{i_2}, \dots, \mathbf{a}_n) = D(\mathbf{a}_1, \dots, \mathbf{a}_{i_1}, \dots, \mathbf{a}_n) + D(\mathbf{a}_1, \dots, \mathbf{a}_{i_2}, \dots, \mathbf{a}_n) \quad (3-6-11)$$

$$(ii) \quad D(\mathbf{a}_1, \dots, k\mathbf{a}_i, \dots, \mathbf{a}_n) = kD(\mathbf{a}_1, \dots, \mathbf{a}_i, \dots, \mathbf{a}_n) \quad (3-6-12)$$

$$(iii) \quad D(\mathbf{a}_1, \dots, \mathbf{a}_i, \dots, \mathbf{a}_i, \dots, \mathbf{a}_n) = 0 \\ \therefore D(\mathbf{a}_1, \dots, \mathbf{a}_j, \dots, \mathbf{a}_i, \dots, \mathbf{a}_n) = -D(\mathbf{a}_1, \dots, \mathbf{a}_i, \dots, \mathbf{a}_j, \dots, \mathbf{a}_n) \quad (3-6-13)$$

$$(iv) \quad D(\mathbf{e}_1, \mathbf{e}_2, \dots, \mathbf{e}_n) = 1 \quad (3-6-14)$$

これまでと同様にこの関数値はこの 4 つの性質で一意に定まり、「n 次元体積」に相当する<sup>23</sup>。

3 次と同様  $D(\mathbf{e}_{i_1}, \mathbf{e}_{i_2}, \dots, \mathbf{e}_{i_n})$  は 性質(iii),(iv)より  $\mathbf{e}_1, \mathbf{e}_2, \dots, \mathbf{e}_n$  からの並び替えで値が決まり<sup>24</sup>、

$$D(\mathbf{e}_{i_1}, \mathbf{e}_{i_2}, \dots, \mathbf{e}_{i_n}) = \begin{cases} +1 & (i_1, i_2, \dots, i_n) \text{ が } (1, 2, \dots, n) \text{ の偶置換} \\ -1 & (i_1, i_2, \dots, i_n) \text{ が } (1, 2, \dots, n) \text{ の奇置換} \\ 0 & \text{other} \end{cases} \quad (3-6-15)$$

となり、これは (3-7-6) 式である拡張 Levi-Civita 記号  $\varepsilon_{i_1 i_2 \dots i_n}$  と全く同じとなる。

性質 (i),(ii) のことを**多重線形性**、性質 (iii) のことを**交代性**という。

性質 (i), (ii), (iii) を用いて、後に重要となる性質を 2 つ導く。

● あるベクトルのスカラー積を他のベクトルに加えても「関数」の値は変わらない

$$D(\mathbf{a}_1, \dots, \mathbf{a}_{i-1}, \mathbf{a}_i + k\mathbf{a}_j, \dots, \mathbf{a}_j, \dots, \mathbf{a}_n) = D(\mathbf{a}_1, \dots, \mathbf{a}_{i-1}, \mathbf{a}_i, \dots, \mathbf{a}_j, \dots, \mathbf{a}_n) \quad (3-6-16)$$

【証明】  $D(\mathbf{a}_1, \dots, \mathbf{a}_i + k\mathbf{a}_j, \dots, \mathbf{a}_j, \dots, \mathbf{a}_n) = D(\mathbf{a}_1, \dots, \mathbf{a}_i, \dots, \mathbf{a}_j, \dots, \mathbf{a}_n) + kD(\mathbf{a}_1, \dots, \mathbf{a}_j, \dots, \mathbf{a}_j, \dots, \mathbf{a}_n)$   
 $= D(\mathbf{a}_1, \dots, \mathbf{a}_i, \dots, \mathbf{a}_j, \dots, \mathbf{a}_n) \quad \blacksquare$ 

● 線形従属なベクトルの組に対しては 0 となる（張る体積は 0）

$$\mathbf{a}_1, \mathbf{a}_2, \dots, \mathbf{a}_n \text{ が線形従属} \Rightarrow D(\mathbf{a}_1, \mathbf{a}_2, \dots, \mathbf{a}_n) = 0 \quad (3-6-17)$$

【証明】 線形従属なので、あるベクトルは他の線形結合で書ける。

例えば  $\mathbf{a}_1 = k_2 \mathbf{a}_2 + \dots + k_n \mathbf{a}_n$  と書けたとすると（他の場合も同様）

$$D(\mathbf{a}_1, \mathbf{a}_2, \dots, \mathbf{a}_n) = k_2 D(\mathbf{a}_2, \mathbf{a}_2, \dots, \mathbf{a}_n) + \dots + k_n D(\mathbf{a}_n, \mathbf{a}_2, \dots, \mathbf{a}_n) = 0 \quad \blacksquare$$

またこの対偶として「 $D(\mathbf{a}_1, \mathbf{a}_2, \dots, \mathbf{a}_n) \neq 0 \Rightarrow \mathbf{a}_1, \mathbf{a}_2, \dots, \mathbf{a}_n$  は線形独立」が直ちにいえる。

この「関数」には線形代数がいつぱい詰まっている。次講以降で活躍する。

<sup>23</sup> 数学的な厳密さよりも武器を作ることを目的としている。そもそも「n 次元体積」の定義すらしていないことに注意。（これに踏み込むと話が進まないw 興味のある人は(将来)「Gram 行列式」「微分形式」とかで調べてみよう）次講で(n 次元目の高さ)×(n-1 次元体積)と解釈できる話をする。ここでは、これを用いて「n 次元体積」としよう。ど一しても論理体系が気になる人は（内積のように）この 4 つの性質をこの「関数」の公理と位置づけて考え、別途「n 次元体積」となることを示す立場を取ろう。

<sup>24</sup> 偶置換、奇置換は、[3-7-2] 拡張 Levi-Civita 記号 および 付録 3 参照

<span id="page-46-0"></span>**【3-7】 付録 1 : Levi-Civita 記号<sup>25</sup>[3-7-1] Levi-Civita 記号 (3次の場合)**● 定義
$$\varepsilon_{ijk} = \begin{cases} +1 & \text{if } (i,j,k) = (1,2,3), (2,3,1), (3,1,2) \\ -1 & \text{if } (i,j,k) = (1,3,2), (2,1,3), (3,2,1) \\ 0 & \text{other} \end{cases} \quad (3-7-1)$$

この記号を使うとベクトルの外積は

$$\mathbf{a} \times \mathbf{b} = \sum_{i,j,k=1}^3 \varepsilon_{ijk} a_j b_k \mathbf{e}_i \quad (3-7-2)$$

または単に成分表記で

$$(\mathbf{a} \times \mathbf{b})_i = \sum_{j,k=1}^3 \varepsilon_{ijk} a_j b_k \quad (3-7-3)$$

と書ける。

実際(3-7-2)式を展開してみると

$$\begin{aligned} \sum_{i,j,k=1}^3 \varepsilon_{ijk} a_j b_k \mathbf{e}_i &= \sum_{j,k=1}^3 \varepsilon_{1jk} a_j b_k \mathbf{e}_1 + \sum_{j,k=1}^3 \varepsilon_{2jk} a_j b_k \mathbf{e}_2 + \sum_{j,k=1}^3 \varepsilon_{3jk} a_j b_k \mathbf{e}_3 \\ &= (a_2 b_3 - a_3 b_2) \mathbf{e}_1 + (a_3 b_1 - a_1 b_3) \mathbf{e}_2 + (a_1 b_2 - a_2 b_1) \mathbf{e}_3 \end{aligned}$$

となり、外積の定義 (3-5-1) 式と一致する。

● 基本性質 (各添字の値が 1,2,3 のどれであっても成り立つことを確かめるとわかりやすい)

- (i)  $\varepsilon_{ijk} = -\varepsilon_{ikj}$  どの 2 つの添字を入れ替えても符号が変わる
- (ii)  $\varepsilon_{iij} = 0$  添字が同じだと 0 (3-7-4)
- (iii)  $\varepsilon_{ijk} = \varepsilon_{jki}$  添字のサイクリックな入れ替えで不変

● [▼C] Levi-Civita 記号の積
$$\sum_{i=1}^3 \varepsilon_{ijk} \varepsilon_{ilm} = \delta_{jl} \delta_{km} - \delta_{jm} \delta_{kl} \quad (3-7-5)$$

概要を説明する。左辺を展開した第一項  $\varepsilon_{1jk} \varepsilon_{1lm}$  に着目すると、添字  $j, k$  および  $l, m$  がそれぞれ 2, 3 か 3, 2 の場合に非零となり、その組み合わせが  $(2,3)(2,3), (3,2)(3,2)$  の場合に正、 $(2,3)(3,2), (3,2)(2,3)$  の場合に負の符号となる。すなわち 添字の組み合わせとして、 $j = l, k = m$  の場合に +1、 $j = m, k = l$  の場合に -1 となり、それ以外では 0 となる。総和の他の項  $\varepsilon_{2jk} \varepsilon_{2lm}, \varepsilon_{3jk} \varepsilon_{3lm}$  についても同様の事が言えて、これらをまとめたものが上記の式となる。導出は行列式を学んだあと行列 II の講の付録で行う。

<sup>25</sup> エディントンのイプシロンとも呼ばれる (らしい)

**[3-7-2] 拡張 Levi-Civita 記号 (n 次の場合)**

●定義

$$\varepsilon_{i_1 i_2 \dots i_n} = \begin{cases} +1 & (i_1, i_2, \dots, i_n) \text{ が } (1, 2, \dots, n) \text{ の偶置換} \\ -1 & (i_1, i_2, \dots, i_n) \text{ が } (1, 2, \dots, n) \text{ の奇置換} \\ 0 & \text{other} \end{cases} \quad (3-7-6)$$

●偶置換と奇置換

 $(i_1, i_2, \dots, i_n)$  が  $(1, 2, \dots, n)$  の順番を並び替えしたものとする。任意の 2 つの数字の入れ替えを**互換**という。 $(1, 2, \dots, n)$  から互換を繰り返し  $(i_1, i_2, \dots, i_n)$  の並びにするとき、偶数回の互換で達成できる場合を**偶置換**、奇数回の場合を**奇置換**という。この偶奇性は互換のやり方によらない<sup>26</sup>。3 次での例 : 1, 2, 3 の数字の並び方は  $3!=6$  通りあり、 $(1, 2, 3)$  から互換を繰り返し行うと偶奇性により 2 種類に分かれる。 $(1, 2, 3), (2, 3, 1), (3, 1, 2)$  : 偶置換  $(1, 3, 2), (2, 1, 3), (3, 2, 1)$  : 奇置換 (実際に確かめよう) 3 次では通常の Levi-Civita 記号に帰着することがわかる。

●基本性質

- (i)  $\varepsilon_{i_1, \dots, i_j, \dots, i_k, \dots, i_n} = -\varepsilon_{i_1, \dots, i_k, \dots, i_j, \dots, i_n}$  添字の入れ替えで符号が変わる
- (ii)  $\varepsilon_{i_1, \dots, i_j, \dots, i_k, \dots, i_n} = 0$  同じ添字で 0 (3-7-7)

<span id="page-47-0"></span>**[3-8] 付録 2 : 外積の公式の証明**

●成分表記による証明 : ややこしそうに見えるが規則性がつかめれば見た目ほどではない<sup>27</sup>。

○スカラー三重積  $a \cdot (b \times c)$  で成り立つ公式

$$a \cdot (b \times c) = b \cdot (c \times a) = c \cdot (a \times b)$$

3 式をそれぞれ成分表記で展開する。

$$\begin{aligned} a \cdot (b \times c) &= a_1(b_2c_3 - b_3c_2) + a_2(b_3c_1 - b_1c_3) + a_3(b_1c_2 - b_2c_1) \\ &= a_1b_2c_3 + a_2b_3c_1 + a_3b_1c_2 - a_1b_3c_2 - a_2b_1c_3 - a_3b_2c_1 \end{aligned}$$

$$\begin{aligned} b \cdot (c \times a) &= b_1(c_2a_3 - c_3a_2) + b_2(c_3a_1 - c_1a_3) + b_3(c_1a_2 - c_2a_1) \\ &= a_1b_2c_3 + a_2b_3c_1 + a_3b_1c_2 - a_1b_3c_2 - a_2b_1c_3 - a_3b_2c_1 \end{aligned}$$

$$\begin{aligned} c \cdot (a \times b) &= c_1(a_2b_3 - a_3b_2) + c_2(a_3b_1 - a_1b_3) + c_3(a_1b_2 - a_2b_1) \\ &= a_1b_2c_3 + a_2b_3c_1 + a_3b_1c_2 - a_1b_3c_2 - a_2b_1c_3 - a_3b_2c_1 \end{aligned}$$

よって 3 式が等しいことが示された。■

<sup>26</sup> 付録 3 : 置換と転倒数の偶奇性 参照のこと

<sup>27</sup> 証明そのものよりも、この規則性を掴むことを目的としている。パズル感覚で楽しんでほしい

○ベクトル三重積  $\mathbf{a} \times (\mathbf{b} \times \mathbf{c})$  で成り立つ公式<sup>28</sup>

$$\mathbf{a} \times (\mathbf{b} \times \mathbf{c}) = (\mathbf{a} \cdot \mathbf{c})\mathbf{b} - (\mathbf{a} \cdot \mathbf{b})\mathbf{c}$$

$$\begin{aligned} \mathbf{a} \times (\mathbf{b} \times \mathbf{c}) &= \{a_2(b_1c_2 - b_2c_1) - a_3(b_3c_1 - b_1c_3)\}\mathbf{e}_1 \\ &\quad + \{a_3(b_2c_3 - b_3c_2) - a_1(b_1c_2 - b_2c_1)\}\mathbf{e}_2 \\ &\quad + \{a_1(b_3c_1 - b_1c_3) - a_2(b_2c_3 - b_3c_2)\}\mathbf{e}_3 \\ &= \{(a_2c_2 + a_3c_3)b_1 - (a_2b_2 + a_3b_3)c_1\}\mathbf{e}_1 \\ &\quad + \{(a_1c_1 + a_3c_3)b_2 - (a_1b_1 + a_3b_3)c_2\}\mathbf{e}_2 \\ &\quad + \{(a_1c_1 + a_2c_2)b_3 - (a_1b_1 + a_2b_2)c_3\}\mathbf{e}_3 \\ &= \{(a_1c_1 + a_2c_2 + a_3c_3)b_1 - (a_1b_1 + a_2b_2 + a_3b_3)c_1\}\mathbf{e}_1 \\ &\quad + \{(a_1c_1 + a_2c_2 + a_3c_3)b_2 - (a_1b_1 + a_2b_2 + a_3b_3)c_2\}\mathbf{e}_2 \\ &\quad + \{(a_1c_1 + a_2c_2 + a_3c_3)b_3 - (a_1b_1 + a_2b_2 + a_3b_3)c_3\}\mathbf{e}_3 \\ &= \{(\mathbf{a} \cdot \mathbf{c})b_1 - (\mathbf{a} \cdot \mathbf{b})c_1\}\mathbf{e}_1 + \{(\mathbf{a} \cdot \mathbf{c})b_2 - (\mathbf{a} \cdot \mathbf{b})c_2\}\mathbf{e}_2 + \{(\mathbf{a} \cdot \mathbf{c})b_3 - (\mathbf{a} \cdot \mathbf{b})c_3\}\mathbf{e}_3 \\ &= (\mathbf{a} \cdot \mathbf{c})\mathbf{b} - (\mathbf{a} \cdot \mathbf{b})\mathbf{c} \quad \blacksquare \end{aligned}$$

○外積同士の内積  $(\mathbf{a} \times \mathbf{b}) \cdot (\mathbf{c} \times \mathbf{d})$  で成り立つ公式

$$(\mathbf{a} \times \mathbf{b}) \cdot (\mathbf{c} \times \mathbf{d}) = (\mathbf{a} \cdot \mathbf{c})(\mathbf{b} \cdot \mathbf{d}) - (\mathbf{a} \cdot \mathbf{d})(\mathbf{b} \cdot \mathbf{c})$$

$$\begin{aligned} (\mathbf{a} \times \mathbf{b}) \cdot (\mathbf{c} \times \mathbf{d}) &= (a_2b_3 - a_3b_2)(c_2d_3 - c_3d_2) + (a_3b_1 - a_1b_3)(c_3d_1 - c_1d_3) + (a_1b_2 - a_2b_1)(c_1d_2 - c_2d_1) \\ &= a_2b_3c_2d_3 + a_3b_2c_3d_2 + a_3b_1c_3d_1 + a_1b_3c_1d_3 + a_1b_2c_1d_2 + a_2b_1c_2d_1 \\ &\quad - (a_2b_3c_3d_2 + a_3b_2c_2d_3 + a_3b_1c_1d_3 + a_1b_3c_3d_1 + a_1b_2c_2d_1 + a_2b_1c_1d_2) \\ &= a_1c_1b_2d_2 + a_1c_1b_3d_3 + a_2c_2b_1d_1 + a_2c_2b_3d_3 + a_3c_3b_1d_1 + a_3c_3b_2d_2 \\ &\quad - (a_1d_1b_2c_2 + a_1d_1b_3c_3 + a_2d_2b_1c_1 + a_2d_2b_3c_3 + a_3d_3b_1c_1 + a_3d_3b_2c_2) \\ &= \{a_1c_1(b_2d_2 + b_3d_3) + a_2c_2(b_1d_1 + b_3d_3) + a_3c_3(b_1d_1 + b_2d_2)\} \\ &\quad - \{a_1d_1(b_2c_2 + b_3c_3) + a_2d_2(b_1c_1 + b_3c_3) + a_3d_3(b_1c_1 + b_2c_2)\} \end{aligned}$$

この式に  $0 = (a_1c_1b_1d_1 + a_2c_2b_2d_2 + a_3c_3b_3d_3) - (a_1d_1b_1c_1 + a_2d_2b_2c_2 + a_3d_3b_3c_3)$ 

を加える

$$\begin{aligned} &= [\{a_1c_1(b_1d_1 + b_2d_2 + b_3d_3) + a_2c_2(b_1d_1 + b_2d_2 + b_3d_3) + a_3c_3(b_1d_1 + b_2d_2 + b_3d_3)\} \\ &\quad - \{a_1d_1(b_1c_1 + b_2c_2 + b_3c_3) + a_2d_2(b_1c_1 + b_2c_2 + b_3c_3) + a_3d_3(b_1c_1 + b_2c_2 + b_3c_3)\}] \\ &= (a_1c_1 + a_2c_2 + a_3c_3)(b_1d_1 + b_2d_2 + b_3d_3) - (a_1d_1 + a_2d_2 + a_3d_3)(b_1c_1 + b_2c_2 + b_3c_3) \\ &= (\mathbf{a} \cdot \mathbf{c})(\mathbf{b} \cdot \mathbf{d}) - (\mathbf{a} \cdot \mathbf{d})(\mathbf{b} \cdot \mathbf{c}) \quad \blacksquare \end{aligned}$$

<sup>28</sup> 基底  $\mathbf{e}_1$  の成分のみに着目、残りはサイクリックな添字の入れ替えで成り立つ

●Levi-Civita 記号を用いた証明<sup>29</sup> (各総和記号の添字は全て 1 から 3 まで動く)

○スカラー三重積 :  $\mathbf{a} \cdot (\mathbf{b} \times \mathbf{c}) = \mathbf{b} \cdot (\mathbf{c} \times \mathbf{a}) = \mathbf{c} \cdot (\mathbf{a} \times \mathbf{b})$ 

$$\begin{aligned} \mathbf{a} \cdot (\mathbf{b} \times \mathbf{c}) &= \sum_i a_i \sum_{j,k} \varepsilon_{ijk} b_j c_k = \sum_{i,j,k} \varepsilon_{ijk} a_i b_j c_k \\ \mathbf{b} \cdot (\mathbf{c} \times \mathbf{a}) &= \sum_j b_j \sum_{k,i} \varepsilon_{jki} c_k a_i = \sum_{i,j,k} \varepsilon_{jki} a_i b_j c_k = \sum_{i,j,k} \varepsilon_{ijk} a_i b_j c_k \quad (\because (3-7-4)(iii)) \\ \mathbf{c} \cdot (\mathbf{a} \times \mathbf{b}) &= \sum_k c_k \sum_{i,j} \varepsilon_{kij} a_i b_j = \sum_{i,j,k} \varepsilon_{kij} a_i b_j c_k = \sum_{i,j,k} \varepsilon_{ijk} a_i b_j c_k \quad \blacksquare \end{aligned}$$

○[▼C] ベクトル三重積 :  $\mathbf{a} \times (\mathbf{b} \times \mathbf{c}) = (\mathbf{a} \cdot \mathbf{c})\mathbf{b} - (\mathbf{a} \cdot \mathbf{b})\mathbf{c}$ 

$$\begin{aligned} \mathbf{a} \times (\mathbf{b} \times \mathbf{c}) &= \sum_{i,j,k} \varepsilon_{ijk} a_j \left( \sum_{l,m} \varepsilon_{klm} b_l c_m \right) \mathbf{e}_i \\ &= \sum_{i,j,l,m} \sum_k \varepsilon_{kij} \varepsilon_{klm} a_j b_l c_m \mathbf{e}_i \quad (\because (3-7-4)(iii)) \\ &= \sum_{i,j,l,m} (\delta_{il} \delta_{jm} - \delta_{im} \delta_{jl}) a_j b_l c_m \mathbf{e}_i \quad (\because (3-7-5)) \\ &= \sum_{i,j} \{(a_j c_j) b_i - (a_j b_j) c_i\} \mathbf{e}_i \\ &= (\mathbf{a} \cdot \mathbf{c})\mathbf{b} - (\mathbf{a} \cdot \mathbf{b})\mathbf{c} \quad \blacksquare \end{aligned}$$

○[▼C] 外積同士の内積 :  $(\mathbf{a} \times \mathbf{b}) \cdot (\mathbf{c} \times \mathbf{d}) = (\mathbf{a} \cdot \mathbf{c})(\mathbf{b} \cdot \mathbf{d}) - (\mathbf{a} \cdot \mathbf{d})(\mathbf{b} \cdot \mathbf{c})$ 

$$\begin{aligned} (\mathbf{a} \times \mathbf{b}) \cdot (\mathbf{c} \times \mathbf{d}) &= \sum_i \left( \sum_{j,k} \varepsilon_{ijk} a_j b_k \right) \left( \sum_{l,m} \varepsilon_{ilm} c_l d_m \right) \\ &= \sum_{j,k,l,m} \sum_i \varepsilon_{ijk} \varepsilon_{ilm} a_j b_k c_l d_m \\ &= \sum_{j,k,l,m} (\delta_{jl} \delta_{km} - \delta_{jm} \delta_{kl}) a_j b_k c_l d_m \quad (\because (3-7-5)) \\ &= \sum_{j,k} (a_j c_j b_k d_k - a_j d_j b_k c_k) \\ &= (\mathbf{a} \cdot \mathbf{c})(\mathbf{b} \cdot \mathbf{d}) - (\mathbf{a} \cdot \mathbf{d})(\mathbf{b} \cdot \mathbf{c}) \quad \blacksquare \end{aligned}$$

<sup>29</sup> こういうのが代数の威力の片鱗の片鱗でござる。総和記号に不慣れな場合は、第 2 講の付録 2 参照。

<span id="page-50-0"></span>**【3-9】付録3:置換と転倒数の偶奇性**置換の偶奇性（偶数・奇数のどちらかということ）はその本来の形で定義し、互換のやり方によらないことを証明しようとすると、 $n$  次の対称群の話となり準備含めそれなりの頁数を要する。大抵の線形代数の教科書にも書いてあると思うので、ここでは転倒数というものの偶奇性と置換の偶奇性の関係を調べる。なお対称群とはどういうものなのか一見の価値はあると思うので、未見の読者は折をみて調べて頂きたい<sup>30</sup>。

●転倒数の定義1から $n$ までの数字の並び  $1, 2, \dots, n$  を任意に並び替えしたものを  $i_1, i_2, \dots, i_n$  としたとき、このなかの  $i_j, i_k$  が、 $j < k$  にもかかわらず  $i_j > i_k$  となるとき、この  $i_j, i_k$  は転倒しているといい、全ての転倒している2つの数字の組数の合計をその数字の並びの**転倒数**という。

→要するに左から順にみていったとき、自分の右側に自分より小さな数がいくつあるか？

その合計のこと。任意の数字の並びに対してその転倒数は一意に定まり、並び替えの手順には依らないことがわかる。

例)  $1, 2, 3$  : 転倒している数はない→転倒数 0       $1, 3, 2$  : 3 と 2 が転倒       $\rightarrow$  転倒数 1  
 $2, 3, 1$  : 2 と 1, 3 と 1 が転倒 →転倒数 2       $2, 1, 3$  : 2 と 1 が転倒       $\rightarrow$  転倒数 1  
 $3, 1, 2$  : 3 と 1, 3 と 2 が転倒 →転倒数 2       $3, 2, 1$  : 3 と 2, 3 と 1, 2 と 1 が転倒→転倒数 3

●転倒数の符号の定義 $i_1, i_2, \dots, i_n$  の転倒数が偶数のときを  $+1$ 、奇数のときを  $-1$  として転倒数の符号を定義し、 $\varepsilon(i_1, i_2, \dots, i_n)$  と記す。

$$\text{例) } \varepsilon(1,2,3) = \varepsilon(2,3,1) = \varepsilon(3,1,2) = +1, \quad \varepsilon(1,3,2) = \varepsilon(2,1,3) = \varepsilon(3,2,1) = -1$$

●隣り合う2つの数字の入れ替え（隣接互換）に対する性質 $i_1, i_2, \dots, i_n$  に対し、どの隣り合う2つの数字を入れ替えても転倒数の符号は変わる。

（つまり  $\varepsilon(i_1, \dots, i_{k+1}, i_k, \dots, i_n) = -\varepsilon(i_1, \dots, i_k, i_{k+1}, \dots, i_n)$  となる）

【証明】: 任意の隣り合う数字を  $i_k, i_{k+1}$  とする。この2つの数字を入れ替えるとき、2つ以外の他の数字に対する転倒数は変わらないことがわかる。この2つの数字の組が  $i_k < i_{k+1}$  ならば入れ替えると転倒数は1増える。逆に  $i_k > i_{k+1}$  ならば入れ替えると転倒数は1減る。以上によりいずれにしても転倒数の符号は変わることがわかる。 ■

<sup>30</sup> ごく始めの部分について次講の付録2で触れる

#### ●任意の2つの数字の入れ替え（互換）に対する性質

 $i_1, i_2, \dots, i_n$  に対し、どの2つの数字を入れ替えても転倒数の符号は変わる。

(つまり  $\varepsilon(i_1, \dots, i_{j+k}, \dots, i_j, \dots, i_n) = -\varepsilon(i_1, \dots, i_j, \dots, i_{j+k}, \dots, i_n)$  となる)

【証明】: 入れ替える数字の組を  $i_j, i_{j+k}$  ( $k > 0$ ) とする。今  $i_j$  を次々と右隣の数字と入れ替えて  $\dots, i_{j-1}, i_j, i_{j+1}, \dots, i_{j+k-1}, i_{j+k}, i_{j+k+1}, \dots$  ←から(☆)の並びにすると  $k$  回隣接互換したことになる。  $\dots, i_{j-1}, i_{j+1}, \dots, i_{j+k-1}, i_{j+k}, i_j, i_{j+k+1}, \dots$  (☆) さらに  $i_{j+k}$  を次々と左隣と入れ替えて(★)の並び  $\dots, i_{j-1}, i_{j+k}, i_{j+1}, \dots, i_{j+k-1}, i_j, i_{j+k+1}, \dots$  (★) まで行ったとすると  $k-1$  回隣接互換したことになる。これにより  $i_j, i_{j+k}$  の互換が達成され、合計で  $2k-1$  回の奇数回 隣接互換したので転倒数の符号は変わる。また転倒数は一意に定まるので互換のやり方には依らないことがわかる。 ■

#### ●置換の偶奇性と転倒数の偶奇性

 $i_1, i_2, \dots, i_n$  が  $1, 2, \dots, n$  の偶/奇置換であるとは、 $1, 2, \dots, n$  に対して互換を繰り返し偶/奇数回で  $i_1, i_2, \dots, i_n$  に到達できる場合のことと定義した。今、この過程を転倒数と比較しながらたどれば、転倒数の定義より  $1, 2, \dots, n$  の転倒数は偶数 (0) で、上記互換に対する性質より互換のたびに転倒数の偶奇性も同じように変わっていくことから、任意の  $i_1, i_2, \dots, i_n$  に対する置換の偶奇性と転倒数の偶奇性は一致することがわかる。 さらに  $i_1, i_2, \dots, i_n$  に対する転倒数は一意に定まるので、置換および転倒数の偶奇性は互換のやり方に依らないことがわかる。

#### ● $D(e_{i_1}, \dots, e_{i_n})$ および $\varepsilon_{i_1 \dots i_n}$ の符号について

「関数」  $D(e_{i_1}, \dots, e_{i_n})$  は  $i_1, \dots, i_n$  が全て異なるときに 0 以外の値をもち、 $1, \dots, n$  のときに  $+1$  となり、どの  $e_i, e_j$  を入れ替えても符号が変わる性質を持っていた。上記の偶奇性の議論を当てはめると、 $i_1, \dots, i_n$  が全て異なるとき置換および転倒数の偶奇性による符号の変化と一致することがわかる。また  $D(e_{i_1}, \dots, e_{i_n})$  と拡張 Levi-Civita 記号  $\varepsilon_{i_1 \dots i_n}$  を同一視できることになる。

#### ●演習 : 4次の置換・転倒数の偶奇性の具体例による確認

下記は4つの数字の並び  $4!=24$  個を置換・転倒数の符号により組分けしたものであり、() 内はそれぞれの転倒数を示す。これを用いた本付録内容の確認を、理解を深めるための演習とする。

$$\begin{aligned} +1: & \begin{cases} 1234 & (0) & 1342 & (2) & 1423 & (2) & 2143 & (2) & 2314 & (2) & 2431 & (4) \\ 3124 & (2) & 3241 & (4) & 3412 & (4) & 4132 & (4) & 4213 & (4) & 4321 & (6) \end{cases} \\ -1: & \begin{cases} 1243 & (1) & 1324 & (1) & 1432 & (3) & 2134 & (1) & 2341 & (3) & 2413 & (3) \\ 3142 & (3) & 3214 & (3) & 3421 & (5) & 4123 & (3) & 4231 & (5) & 4312 & (5) \end{cases} \end{aligned}$$

なお、先頭が1である  $1234(0), 1342(2), 1423(2)$  と  $1243(1), 1324(1), 1432(3)$  の各転倒数とその偶奇性は1を除いた  $234(0), 342(2), 423(2)$  と  $243(1), 324(1), 432(3)$  のと同じで、さらに各数字から1を引いた  $123(0), 231(2), 312(2)$  と  $132(1), 213(1), 321(3)$  の各転倒数とその偶奇性とも等しい。次講にて、このことを用いる。

## 【第 4 講】 行列 I : 連立一次方程式

<span id="page-52-1"></span><span id="page-52-0"></span>

### 【4-1】 はじめに

本講ではまず連立一次方程式を加減法（消去法）で解くことから始めて、掃き出し法（ガウスの消去法）と呼ばれる系統的な解法を学ぶ。実は線形代数は連立一次方程式を系統的に解く研究に端を発するものであり、そこには線形代数の本質の一端が潜んでいる。本講では、ひたすら連立一次方程式をいじくり回し、前講の最後に用意した「関数」も用い、行列式・行列を定義して考察を続ける。

ちなみに連立一次方程式を効率的に解くことは、現代においても計算科学における重要な研究テーマのひとつであると聞いたら驚く人もいるかと思う。もちろん 2 元や 3 元連立といったことではなく、とてつもなく大規模な話である<sup>31</sup>。そこで使われる手法はさまざまであるが、掃き出し法はその最初の第一歩にあたる。

<span id="page-52-2"></span>

### 【4-2】 掃き出し法

#### 【4-2-1】 連立一次方程式の加減法による解法

以下の三元連立一次方程式を加減法で解く。

$$\begin{cases} x + y + 2z = 9 \\ 2x + y + 3z = 13 \\ x + 2y + 4z = 17 \end{cases}$$

毎回  $x$  や  $y, z$  を書く必要ないよね？

$$\begin{bmatrix} 1 & 1 & 2 & 9 \\ 2 & 1 & 3 & 13 \\ 1 & 2 & 4 & 17 \end{bmatrix}$$

・ 第 2 式と第 3 式から第 1 式のそれぞれ 2 倍・ 1 倍を引く

$$\begin{cases} x + y + 2z = 9 \\ -y - z = -5 \\ y + 2z = 8 \end{cases}$$

$$\begin{bmatrix} 1 & 1 & 2 & 9 \\ 0 & -1 & -1 & -5 \\ 0 & 1 & 2 & 8 \end{bmatrix}$$

・ 第 2 式を(-1)倍

$$\begin{cases} x + y + 2z = 9 \\ y + z = 5 \\ y + 2z = 8 \end{cases}$$

$$\begin{bmatrix} 1 & 1 & 2 & 9 \\ 0 & 1 & 1 & 5 \\ 0 & 1 & 2 & 8 \end{bmatrix}$$

・ 第 3 式から第 2 式を引く

$$\begin{cases} x + y + 2z = 9 \\ y + z = 5 \\ z = 3 \end{cases}$$

$$\begin{bmatrix} 1 & 1 & 2 & 9 \\ 0 & 1 & 1 & 5 \\ 0 & 0 & 1 & 3 \end{bmatrix}$$

・ 第 1 式と第 2 式から第 3 式のそれぞれ 2 倍・ 1 倍を引く

$$\begin{cases} x + y = 3 \\ y = 2 \\ z = 3 \end{cases}$$

$$\begin{bmatrix} 1 & 1 & 0 & 3 \\ 0 & 1 & 0 & 2 \\ 0 & 0 & 1 & 3 \end{bmatrix}$$

・ 第 1 式から第 2 式を引く

$$\begin{cases} x = 1 \\ y = 2 \\ z = 3 \end{cases}$$

$$\begin{bmatrix} 1 & 0 & 0 & 1 \\ 0 & 1 & 0 & 2 \\ 0 & 0 & 1 & 3 \end{bmatrix}$$

<sup>31</sup> 何千万元連立とか。凄つ：偏微分方程式を離散化したものや、「ビッグデータ」の解析手法 等々々々

左側は加減法を用いて実際に解いたもので、右側はその係数と右辺の定数項のみを書き出したものである。右側はひとまず置いといて、加減法の解き方を振り返ってみよう。

連立方程式なので、各式を辺々「加減」しても成り立たなければならない。加減法はこの性質を利用して、**各式ごとに担当する変数以外の変数を消去していき、最終的に各式の左辺が単独な各変数となるようにすること**で、右辺に解を得る手法である。上記を実現するにあたり、

- ある式の両辺を定数倍（0以外で負値を含む）する
- ある式の両辺の定数倍（0以外で負値を含む）を別の式の両辺に加える

の２つの式変形が基本となり、これらを駆使しながら解くことになる。

上記の例をみると、必要な情報は左辺の各式における各変数の係数と、右辺の定数項だということが分かる。その観点で各係数と定数項のみを抽出して書かれたものが右側の表記となり、掃き出し法とは右側の表記で加減法をやることに他ならない。

### **[4-2-2] 掃き出し法と行基本変形**

右側の表記  $\left( \begin{array}{ccc|c} 1 & 1 & 2 & 9 \\ 2 & 1 & 3 & 13 \\ 1 & 2 & 4 & 17 \end{array} \right)$  は、元の式の係数が書かれている縦棒の左側部分を**係数行列**、右辺

定数項にあたる縦棒の右側を含めた全体を**拡大係数行列**という。横に並んだ数字・文字を**行**、縦に並んだ数字・文字を**列**と呼ぶ。この例では係数行列のみで見れば第 1 行は 1 1 2、第 3 列は 2

3 となる。また係数行列の各行で左からみて最初の 0 でない値をもつ成分を**主成分**という。

1. ↑
2. ↑

掃き出し法では「式変形」にあたるものは**行基本変形**と呼ばれ、行基本変形を駆使して実現すべき係数行列を簡約行列といい、この行、列、主成分の用語を使うと以下のように定義される。

## ●行基本変形の定義

- ある行を定数倍（0 以外で負値を含む）する
- ある行の定数倍（0 以外で負値を含む）を別の行に加える (4 − 2 − 1)
- （必要に応じて）ある行と別の行を入れ替える

### ●簡約行列の定義(各主成分は各式に残す各変数の係数にあたる)

- 各主成分の値は 1
- 主成分をもつ列の主成分以外の値は 0 (4 - 2 - 2)
- 各行は下側にいくほど主成分は右側にある
- 全ての成分が 0 となる行はそうでない行の下側にある

違う例で掃き出し法を確認してみよう。右側と見比べると何をしているのかよく分かると思う。

| $\begin{bmatrix} 1 & -1 & 3 &   & 3 \\ -1 & 1 & -2 &   & -5 \\ 2 & -3 & 4 &   & 8 \end{bmatrix}$ | $\begin{cases} x - y + 3z = 8 \\ -x + y - 2z = -5 \\ 2x - 3y + 4z = 8 \end{cases}$ |
|--------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
|--------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|

「2 行目 ( $r_2$ ) と3 行目 ( $r_3$ ) を入れ替えた」という行基本変形を意味する<sup>32</sup>。

$$\begin{bmatrix} 1 & -1 & 3 & 8 \\ 0 & 0 & 1 & 3 \\ 0 & -1 & -2 & -8 \end{bmatrix} \begin{matrix} r_2 + r_1 \\ r_3 - 2r_1 \end{matrix} \quad \begin{cases} x - y + 3z = 8 \\ z = 3 \\ -y - 2z = -8 \end{cases}$$

$$\begin{bmatrix} 1 & -1 & 3 & 8 \\ 0 & -1 & -2 & -8 \\ 0 & 0 & 1 & 3 \end{bmatrix} \begin{matrix} r_2 \leftrightarrow r_3 \\ \end{matrix} \quad \begin{cases} x - y + 3z = 8 \\ -y - 2z = -8 \\ z = 3 \end{cases}$$

$$\begin{bmatrix} 1 & -1 & 3 & 8 \\ 0 & 1 & 2 & 8 \\ 0 & 0 & 1 & 3 \end{bmatrix} \begin{matrix} r_2 \times (-1) \\ \\ \end{matrix} \quad \begin{cases} x - y + 3z = 8 \\ y + 2z = 8 \\ z = 3 \end{cases}$$

$$\begin{bmatrix} 1 & -1 & 0 & -1 \\ 0 & 1 & 0 & 2 \\ 0 & 0 & 1 & 3 \end{bmatrix} \begin{matrix} r_1 - 3r_3 \\ r_2 - 2r_3 \\ \end{matrix} \quad \begin{cases} x - y = -1 \\ y = 2 \\ z = 3 \end{cases}$$

$$\begin{bmatrix} 1 & 0 & 0 & 1 \\ 0 & 1 & 0 & 2 \\ 0 & 0 & 1 & 3 \end{bmatrix} \begin{matrix} r_1 + r_2 \\ \\ \end{matrix} \quad \begin{cases} x = 1 \\ y = 2 \\ z = 3 \end{cases}$$

### [4-2-3] 不定解、解なしとなる場合

連立一次方程式において方程式が全て独立でない場合、その解は不定もしくは不能（解なし）となった。例として

$$\begin{cases} x + y + 2z = 1 \\ 3x + 2y + 3z = 2 \\ 2x + y + z = 1 + a \end{cases}$$

を考える。この連立方程式の第3式は、第2式から第1式を引いたものの右辺定数項に  $a$  を足したものとなっており、独立な式が一つ減るので  $a = 0$  の場合 解は不定となる。

 $a \neq 0$  の場合は連立させる式が共通の解を持たない事になり連立方程式としては解なし、つまり不能となる。掃き出し法ではどのように振る舞うのだろうか。実際に解いてみよう。

$$\begin{bmatrix} 1 & 1 & 2 & 1 \\ 3 & 2 & 3 & 2 \\ 2 & 1 & 1 & 1 + a \end{bmatrix} \quad \begin{cases} x + y + 2z = 1 \\ 3x + 2y + 3z = 2 \\ 2x + y + z = 1 + a \end{cases}$$

$$\begin{bmatrix} 1 & 1 & 2 & 1 \\ 0 & -1 & -3 & -1 \\ 0 & -1 & -3 & -1 + a \end{bmatrix} \begin{matrix} r_2 - 3r_1 \\ r_3 - 2r_1 \end{matrix} \quad \begin{cases} x + y + 2z = 1 \\ -y - 3z = -1 \\ -y - 3z = -1 + a \end{cases}$$

$$\begin{bmatrix} 1 & 1 & 2 & 1 \\ 0 & 1 & 3 & 1 \\ 0 & -1 & -3 & -1 + a \end{bmatrix} \begin{matrix} r_2 \times (-1) \\ \\ \end{matrix} \quad \begin{cases} x + y + 2z = 1 \\ y + 3z = 1 \\ -y - 3z = -1 + a \end{cases}$$

$$\begin{bmatrix} 1 & 1 & 2 & 1 \\ 0 & 1 & 3 & 1 \\ 0 & 0 & 0 & a \end{bmatrix} \begin{matrix} r_3 + r_2 \\ \\ \end{matrix} \quad \begin{cases} x + y + 2z = 1 \\ y + 3z = 1 \\ 0 = a \end{cases}$$

となり、3 行目が元の式で表すと左辺は 0、右辺は  $a$  となった。さらに続けると

<sup>32</sup>  $r$  は 行を表す row の意。この書き方はいろいろと流儀があると思う。なお「このように各列の主成分以外の値を 0 にしていくことを『掃き出す』と称している」という説が有力。

$$\begin{bmatrix} 1 & 0 & -1 \\ 0 & 1 & 3 \\ 0 & 0 & 0 \end{bmatrix} \begin{bmatrix} 0 \\ 1 \\ a \end{bmatrix} r_1 - r_2 \quad \left\{ \begin{array}{l} x = -z = 0 \\ y + 3z = 1 \\ 0 = a \end{array} \right.$$

と簡約行列となり、確かに 3 変数に対して独立な式が 2 つであることを意味している。

 $a \neq 0$  の場合、**不能**（連立方程式としては解無し）となる。

 $a = 0$  の場合、解は**不定**となりパラメータ  $t$  を用いて例えば  $z = t$  とした場合は

$$\begin{cases} x = t \\ y = -3t + 1 \\ z = t \end{cases} \text{ あるいはパラメータを消去して } \begin{cases} x = z \\ y = -3z + 1 \end{cases}$$

という解となる。このようなパラメータの数（この場合は 1）は解の自由度と呼ばれる。

以上のように簡約行列となった時点での「主成分の数」（=「主成分がある行/列の数」=「成分が全て 0 となった行以外の行の数」）を（係数行列の）**rank**（階数）といい上記の例では 2 となる。これは元の連立方程式で独立な式の数を意味することになる。元の変数の数（ $n$ ）に対して同じだけ独立な式の数（rank）があれば解が定まり（一意性は後程述べる）、少なければ不能か不定となり、不定の場合は 解の自由度 =  $n - \text{rank}$  という関係となる（付録 2 参照）。また行基本変形の様子を観察すると直接数値を加減しあうのは同じ列の間だけであり、**rank** は係数行列部分のみで決まり定数項の値に依らず同じ手順で掃き出せる構造であることがわかる。

※幾何学的解釈：3 元 1 次方程式  $ax + by + cz = d$  は 3 次元空間における平面の方程式とみることもできた。平面の法線ベクトルを  $\mathbf{n} = (a, b, c)$ 、平面上のある点を  $\mathbf{r}_0 = (x_0, y_0, z_0)$ 、平面上の任意の点を  $\mathbf{r} = (x, y, z)$  とすると、平面の方程式は  $\mathbf{n} \cdot (\mathbf{r} - \mathbf{r}_0) = 0$  であり、これは  $ax + by + cz = ax_0 + by_0 + cz_0$  となり右辺を  $d$  として与式を得る。式より右辺の定数項が変わると、平面は法線ベクトルの方向（逆向きも含む）に平行移動することがわかる(付録 3 参照)。

![](_page_55_Picture_29.jpeg)

上図は 3 元連立 1 次方程式を 3 平面の交わりとして幾何学的に解釈したもので、図の (a) は 3 平面が一点で交わり、連立方程式の解が定まる場合に相当する。(b) は 1 直線で交わり、上記の例の連立方程式が自由度 1 の不定解を持つ場合に相当する。(c) は 3 平面が共通部分を持たず不能となる例であり上記の例の連立方程式で定数項  $a \neq 0$  に相当する。(d) は独立な式が 1 つ（rank=1）で解の自由度が 2 に相当する。このように係数行列の行を（法線）ベクトルとみなした場合、それらの線形独立性が連立方程式の独立性を決めていそうなことが読み取れる。（各面の法線ベクトルを考察せよ。ヒント：2 平面が平行な場合は法線も平行、直線で交わる場合両法線は直線に垂直となる。）次項ではこれとは違う見かたで連立一次方程式を考察する。

**[4-2-4] 連立一次方程式の違う見かた**

簡単のために 2 元連立一次方程式で考えよう。以下の連立方程式をこんな風にみてみよう。

$$\begin{cases} x + 2y = 5 \\ 2x + 5y = 12 \end{cases} \quad x \begin{bmatrix} 1 \\ 2 \end{bmatrix} + y \begin{bmatrix} 2 \\ 5 \end{bmatrix} = \begin{bmatrix} 5 \\ 12 \end{bmatrix} \quad (4-2-3)$$

連立方程式の解は  $x = 1, y = 2$  となり、2 式は独立な式であることもわかる。

 $\begin{bmatrix} 1 \\ 2 \end{bmatrix}, \begin{bmatrix} 2 \\ 5 \end{bmatrix}, \begin{bmatrix} 5 \\ 12 \end{bmatrix}$  は、成分がそれぞれ (1,2), (2,5), (5,12) の数ベクトルであり、それぞれ変数  $x, y$  の係数と右辺定数項に相当する。変数  $x, y$  を係数のベクトルに対するスカラー積とみれば、

$$\begin{bmatrix} x \\ 2x \end{bmatrix} + \begin{bmatrix} 2y \\ 5y \end{bmatrix} = \begin{bmatrix} 5 \\ 12 \end{bmatrix} \quad \therefore \begin{bmatrix} x + 2y \\ 2x + 5y \end{bmatrix} = \begin{bmatrix} 5 \\ 12 \end{bmatrix}$$

となり元の連立方程式を再現し、(4-2-3)式は係数列のベクトル  $\begin{bmatrix} 1 \\ 2 \end{bmatrix}, \begin{bmatrix} 2 \\ 5 \end{bmatrix}$  の線形結合で定数項ベクトルを表せるか？を意味し、解が定まるこの場合はベクトルの組は線形独立である。

別の例として独立でない連立方程式も考えてみよう。

$$\begin{cases} x + 2y = 5 \\ 3x + 6y = 15 \end{cases} \quad x \begin{bmatrix} 1 \\ 3 \end{bmatrix} + y \begin{bmatrix} 2 \\ 6 \end{bmatrix} = \begin{bmatrix} 5 \\ 15 \end{bmatrix} \quad (4-2-4)$$

下式は上式の 3 倍で、答えは  $x = -2t + 5, y = t$  となり、独立ではない式であることがわかる。

また係数の列のベクトル  $\begin{bmatrix} 1 \\ 3 \end{bmatrix}, \begin{bmatrix} 2 \\ 6 \end{bmatrix}$  は  $\begin{bmatrix} 2 \\ 6 \end{bmatrix} = 2 \begin{bmatrix} 1 \\ 3 \end{bmatrix}$  となり線形従属であり、実際ベクトルを一つにまとめることができ、方程式は  $(x + 2y) \begin{bmatrix} 1 \\ 3 \end{bmatrix} = \begin{bmatrix} 5 \\ 15 \end{bmatrix}$  となり確かに不定解を得ることがわかる。

この見かたでは、一般的な 2 元連立一次方程式

$$\begin{cases} ax + by = e \\ cx + dy = f \end{cases} \quad \text{は} \quad x \begin{bmatrix} a \\ c \end{bmatrix} + y \begin{bmatrix} b \\ d \end{bmatrix} = \begin{bmatrix} e \\ f \end{bmatrix} \quad (4-2-5)$$

とみることになる。ここでベクトルの講の最後で準備した「関数」  $D(\mathbf{a}, \mathbf{b})$  を登場させよう。

天下り式で恐縮だが、 $\begin{bmatrix} e \\ f \end{bmatrix} (= x \begin{bmatrix} a \\ c \end{bmatrix} + y \begin{bmatrix} b \\ d \end{bmatrix})$  と  $\begin{bmatrix} b \\ d \end{bmatrix}$  を  $\mathbf{a}, \mathbf{b}$  に代入してみると線形性と交代性より

$$D(\begin{bmatrix} e \\ f \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}) = D(x \begin{bmatrix} a \\ c \end{bmatrix} + y \begin{bmatrix} b \\ d \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}) = xD(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}) + yD(\begin{bmatrix} b \\ d \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}) = xD(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix})$$

同様に

$$D(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} e \\ f \end{bmatrix}) = D(\begin{bmatrix} a \\ c \end{bmatrix}, x \begin{bmatrix} a \\ c \end{bmatrix} + y \begin{bmatrix} b \\ d \end{bmatrix}) = xD(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} a \\ c \end{bmatrix}) + yD(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}) = yD(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix})$$

これは、 $D(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}) \neq 0$  の場合

$$x = D(\begin{bmatrix} e \\ f \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}) / D(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}), \quad y = D(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} e \\ f \end{bmatrix}) / D(\begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}) \quad (4-2-6)$$

として解が求まるということを意味している。成分で表すと  $D(\mathbf{a}, \mathbf{b}) = a_1 b_2 - a_2 b_1$  だった。

(4-2-3)式  $x \begin{bmatrix} 1 \\ 2 \end{bmatrix} + y \begin{bmatrix} 2 \\ 5 \end{bmatrix} = \begin{bmatrix} 5 \\ 12 \end{bmatrix}$  の例では、 $D(\begin{bmatrix} 1 \\ 2 \end{bmatrix}, \begin{bmatrix} 2 \\ 5 \end{bmatrix}) = 1 \times 5 - 2 \times 2 = 1$  であり、0 でない。

また  $D(\begin{bmatrix} 5 \\ 12 \end{bmatrix}, \begin{bmatrix} 2 \\ 5 \end{bmatrix}) = 5 \times 5 - 12 \times 2 = 1$ ,  $D(\begin{bmatrix} 1 \\ 2 \end{bmatrix}, \begin{bmatrix} 5 \\ 12 \end{bmatrix}) = 1 \times 12 - 2 \times 5 = 2$  なので、確かに  $x = 1, y = 2$  を得る。また(4-2-4)式の例だと列のベクトルは線形従属なので  $D(\begin{bmatrix} 1 \\ 3 \end{bmatrix}, \begin{bmatrix} 2 \\ 6 \end{bmatrix}) = 0$  となり、解が不定となる場合この方法では解を得られないことになる。

※幾何学的解釈:  $\begin{bmatrix} a \\ c \end{bmatrix} = \mathbf{a}, \begin{bmatrix} b \\ d \end{bmatrix} = \mathbf{b}, \begin{bmatrix} e \\ f \end{bmatrix} = \mathbf{e}$  により式は  $x\mathbf{a} + y\mathbf{b} = \mathbf{e}$  と

書け  $\mathbf{e}$  と  $\mathbf{b}$  が張る面積  $D(\mathbf{e}, \mathbf{b})$  は  $x\mathbf{a}$  と  $\mathbf{b}$  が張る面積  $D(x\mathbf{a}, \mathbf{b})$ 

と等しく、これは  $\mathbf{a}$  と  $\mathbf{b}$  が張る面積  $D(\mathbf{a}, \mathbf{b})$  の  $x$  倍であり、よっ

て  $D(\mathbf{e}, \mathbf{b}) = D(x\mathbf{a}, \mathbf{b}) = xD(\mathbf{a}, \mathbf{b})$  より  $D(\mathbf{a}, \mathbf{b}) \neq 0$  のとき  $x = D(\mathbf{e}, \mathbf{b})/D(\mathbf{a}, \mathbf{b})$  として求まる。

![](_page_56_Picture_59.jpeg)

同様に 3 元連立一次方程式でも各係数の列と定数項をベクトルとみなし

$$\begin{cases} ax + by + cz = j \\ dx + ey + fz = k \\ gx + hy + iz = l \end{cases} \text{ だと } x \begin{bmatrix} a \\ d \\ g \end{bmatrix} + y \begin{bmatrix} b \\ e \\ h \end{bmatrix} + z \begin{bmatrix} c \\ f \\ i \end{bmatrix} = \begin{bmatrix} j \\ k \\ l \end{bmatrix} \quad (4-2-7)$$

において  $D \left( \begin{bmatrix} j \\ k \\ l \end{bmatrix}, \begin{bmatrix} b \\ e \\ h \end{bmatrix}, \begin{bmatrix} c \\ f \\ i \end{bmatrix} \right) = x D \left( \begin{bmatrix} a \\ d \\ g \end{bmatrix}, \begin{bmatrix} b \\ e \\ h \end{bmatrix}, \begin{bmatrix} c \\ f \\ i \end{bmatrix} \right)$  等がいえて、 $D \left( \begin{bmatrix} a \\ d \\ g \end{bmatrix}, \begin{bmatrix} b \\ e \\ h \end{bmatrix}, \begin{bmatrix} c \\ f \\ i \end{bmatrix} \right) \neq 0$  の場合は

$$x = \frac{D \left( \begin{bmatrix} j \\ k \\ l \end{bmatrix}, \begin{bmatrix} b \\ e \\ h \end{bmatrix}, \begin{bmatrix} c \\ f \\ i \end{bmatrix} \right)}{D \left( \begin{bmatrix} a \\ d \\ g \end{bmatrix}, \begin{bmatrix} b \\ e \\ h \end{bmatrix}, \begin{bmatrix} c \\ f \\ i \end{bmatrix} \right)}, \quad y = \frac{D \left( \begin{bmatrix} a \\ d \\ g \end{bmatrix}, \begin{bmatrix} j \\ k \\ l \end{bmatrix}, \begin{bmatrix} c \\ f \\ i \end{bmatrix} \right)}{D \left( \begin{bmatrix} a \\ d \\ g \end{bmatrix}, \begin{bmatrix} b \\ e \\ h \end{bmatrix}, \begin{bmatrix} c \\ f \\ i \end{bmatrix} \right)}, \quad z = \frac{D \left( \begin{bmatrix} a \\ d \\ g \end{bmatrix}, \begin{bmatrix} b \\ e \\ h \end{bmatrix}, \begin{bmatrix} j \\ k \\ l \end{bmatrix} \right)}{D \left( \begin{bmatrix} a \\ d \\ g \end{bmatrix}, \begin{bmatrix} b \\ e \\ h \end{bmatrix}, \begin{bmatrix} c \\ f \\ i \end{bmatrix} \right)} \quad (4-2-8)$$

として解ける。全く同様にして、 $n$  元連立でもこの「関数」を適用して解くことができる。このような連立一次方程式の解法を**クラメルの法則** (公式) という<sup>33</sup>。本項の見かた「 $n$  元連立一次方程式の各変数を  $x_1, \dots, x_n$  係数行列の各列と右辺定数項をベクトルとみなしたものを  $a_1, \dots, a_n, b$  とすると方程式は  $x_1 a_1 + \dots + x_n a_n = b$  と書ける。」に対して、いくつか考察しよう。

○掃き出し法とは  $x_1 a_1 + \dots + x_n a_n = b$  に対し線形結合の係数の組  $x_1, \dots, x_n$  を不変に保つたまま(線形結合関係を保つという)、行基本変形により  $x_1 a'_1 + \dots + x_n a'_n = b'$  のように各ベクトルを変形していき、最終的に  $a'_1, \dots, a'_n$  を標準基底に変形することで  $x_1 e_1 + \dots + x_n e_n = x$  として解  $x$  を得る手法といえる。つまり行基本変形は線形結合関係を保つ<sup>34</sup> (だから解になる)。

○この見かたでは簡約行列の rank は線形独立な列のベクトルの最大数と同じとみなせる。実際前項の例では rank = 2 だが主成分がないため掃き出せなかった 3 列目は主成分のある 2 列のベクトルの線形結合で表され、簡約行列の構造から一般的に成り立つことがわかる (付録 2 参照)。また上記のように線形結合関係は行基本変形で保たれるので、rank を (係数) 行列の線形独立な列のベクトルの最大数と定義し直すことで簡約行列でない任意の (係数) 行列に拡張できることになる。

○前講(3-6-17)の対偶「 $D(a_1, \dots, a_n) \neq 0 \Rightarrow a_1, \dots, a_n$  は線形独立」および「 $n$  次元のベクトル( $b$ )の線形独立な  $n$  本のベクトル ( $a_1, \dots, a_n$ ) による線形結合での表し方は一意<sup>35</sup>」より、クラメルの法則により得る解は一意な解であることがいえる。また  $n$  本の列のベクトルの組が線形独立な場合、上記より rank は  $n$  となりその際の掃き出し法で定まるの解の一意性もいえる。

前項の幾何学的解釈でみた行をベクトルの組とみなしたときの線形独立性と解の一意性、および  $D(a_1, \dots, a_n) \neq 0$  との関係は次講にてまとめて示す。

 $D(a_1, \dots, a_n) \neq 0$  は連立一次方程式が一意な解を持つことを示す。次節で改めて調べよう。

<sup>33</sup> 掃き出し法に比べ計算量が多いため、数値計算には向かず理論的考察等に用いられる。次講にて再登場する。なおクラメルの法則(公式)は通常 行列式を用いて定式化されているものを指す。念のため。

<sup>34</sup> 「だから解になる」ので成立して当然なのだが、付録 3 : ●行基本変形と線形結合関係 にて示す

<sup>35</sup> 第 3 講第 2 節 (3-2-5) 参照

<span id="page-58-0"></span>**【4-3】 行列式の導入**

**【4-3-1】 あらためて「関数」  $D(a, b, c)$  とは**

【3-6】 節でみた 4 つの性質で、その値が一意に定まった。3 次の場合を以下に再掲する。

$$\begin{cases} (i) D(a_1 + a_2, b, c) = D(a_1, b, c) + D(a_2, b, c) & (3 - 6 - 5) \\ (ii) D(ka, b, c) = kD(a, b, c) & (3 - 6 - 6) \\ (iii) D(a, a, b) = 0 \quad \therefore D(b, a, c) = -D(a, b, c) & (3 - 6 - 7) \\ (iv) D(e_1, e_2, e_3) = 1 & (3 - 6 - 8) \end{cases}$$

今、相手にしているのは連立一次方程式で、その係数行列を列のベクトルの組として見ているのだった。これからこの「関数」を成分表記で調べるが、係数行列を列のベクトルの組として見ることを踏まえて  $a_j = \sum_{i=1}^n a_{ij} e_i$  として成分を定義する。成分  $a_{ij}$  の左側の添字  $i$  は各ベクトルの上から数えて何番目の成分か（つまり何行目か）を、右側の添字  $j$  は横に並んだ列のベクトルの組のうち左から数えて何番目か（つまり何列目か）を表している。行はその成分が横に並び、列はその成分が縦に並ぶことを思い出そう。また 3 行 3 列だと図のようになることに注意しよう。つまり添字は  $a_{\text{行列}}$  を指す。

$$\begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} \leftarrow 1 \text{ 行}$$

$$\begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} \leftarrow 2 \text{ 行}$$

$$\uparrow 1 \text{ 列} \uparrow 2 \text{ 列} \uparrow 3 \text{ 列}$$

感覚を掴むために、まずは 3 次からやると

$$D(a_1, a_2, a_3) = D \left( \sum_{i=1}^3 a_{i1} e_i, \sum_{j=1}^3 a_{j2} e_j, \sum_{k=1}^3 a_{k3} e_k \right) = \sum_{i,j,k=1}^3 a_{i1} a_{j2} a_{k3} D(e_i, e_j, e_k) \quad (4 - 3 - 1)$$

(4-3-1)式の右辺をじっくり観察してみよう。係数行列の成分は  $a_{i1} a_{j2} a_{k3}$  のように各ベクトルからの積として現れ、右側の添字はベクトルの番号すなわち列の番号を示し、1, 2, 3 と固定されている。左側の添字  $i, j, k$  は各ベクトルの成分の番号を表し、それぞれ独立に 1, 2, 3 をとるが  $D(e_i, e_j, e_k)$  により  $i, j, k$  の値が全て異なる場合のみ残る。つまり各列から一つずつ、他のどの行とも重ならないように成分を選ぶことになる。符号は  $D(e_i, e_j, e_k)$  により決まり、 $(i, j, k) = (1, 2, 3)$  の時+1 で、どの 2 つの添字を入れ替えても符号が変わる。という構造をしている。

3 次の場合、 $D(e_i, e_j, e_k)$  は Levi-Civita 記号  $\varepsilon_{ijk}$  と同一視できた。

この構造は n 次の場合も同様となる。

$$D(a_1, a_2, \dots, a_n) = \sum_{i_1, i_2, \dots, i_n=1}^n a_{i_1 1} a_{i_2 2} \dots a_{i_n n} D(e_{i_1}, e_{i_2}, \dots, e_{i_n}) \quad (4 - 3 - 2)$$

係数行列の成分は  $a_{i_1 1} a_{i_2 2} \dots a_{i_n n}$  のように列を表す右側の添字は 1, 2,  $\dots, n$  固定、各成分を表す左側の添字  $i_1, i_2, \dots, i_n$  は  $D(e_{i_1}, e_{i_2}, \dots, e_{i_n})$  により 添字の値が全て異なる場合のみ残る。つまり各列から一つずつ、他のどの行とも重ならないように成分を選ぶことになる。符号は  $(i_1, i_2, \dots, i_n) = (1, 2, \dots, n)$  の時+1 で、どの 2 つの添字を入れ替えても符号が変わる。n 次の場合も  $D(e_{i_1}, e_{i_2}, \dots, e_{i_n})$  は 拡張 Levi-Civita 記号  $\varepsilon_{i_1 i_2 \dots i_n}$  と同一視できた。

**[4-3-2] 行列式の定義**

前節で連立一次方程式の係数を列のベクトルの組とみたときの「関数」  $D(\mathbf{a}, \mathbf{b}, \mathbf{c}, \dots) \neq 0$  が一意な解をもつ条件であることをみた。この指標を**行列式**という<sup>36</sup>。この後 4 節で定義する行列に対しても、固有な特徴を示す重要な指標となる。ここで改めて定義しよう。表記としては(係数)行列の成分をそのまま並べ、大括弧 [] でなく、縦棒 | | で挟んだ形で表す。 $D(\mathbf{e}_i, \mathbf{e}_j, \mathbf{e}_k, \dots)$  の表記は書くのがメンドクサイので、Levi-Civita 記号  $\varepsilon_{ijk\dots}$  で代用しよう<sup>37</sup>。

2 次だと以下のように定義される

$$\begin{vmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{vmatrix} \equiv \sum_{i,j=1}^2 \varepsilon_{ij} a_{i1} a_{j2} = a_{11} a_{22} - a_{21} a_{12} \quad (4-3-3)$$

$$\varepsilon_{ij} \equiv \begin{cases} +1 & \text{if } (i,j) = (1,2) \\ -1 & \text{if } (i,j) = (2,1) \\ 0 & \text{other} \end{cases} \quad (4-3-4)$$

簡単な覚え方としてよく使われるのは図の左側で、左上から右下へ掛ける場合は + の、右上から左下へ掛ける場合は - の符号がつく。

![](_page_59_Diagram_29.jpeg)

3 次だと

$$\begin{vmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{vmatrix} \equiv \sum_{i,j,k=1}^3 \varepsilon_{ijk} a_{i1} a_{j2} a_{k3} \quad (4-3-5)$$

展開すると

$$= a_{11} a_{22} a_{33} + a_{21} a_{32} a_{13} + a_{31} a_{12} a_{23} - a_{31} a_{22} a_{13} - a_{11} a_{32} a_{23} - a_{21} a_{12} a_{33}$$

簡単な覚え方としてよく使われるのは、上図の右側で、サラスの方法とも呼ばれる。

いずれも各列から一つずつ、他のどの行とも重ならないように成分を選んでいる事に再度注意。

 $n$  次の場合以下のように定義される。

$$\begin{vmatrix} a_{11} & \dots & a_{1n} \\ \vdots & \ddots & \vdots \\ a_{n1} & \dots & a_{nn} \end{vmatrix} \equiv \sum_{i_1, \dots, i_n=1}^n \varepsilon_{i_1 \dots i_n} a_{i_1} \dots a_{i_n} \quad (4-3-6)$$

4 次以上では、サラスの方法のような簡易的な覚え方は適用できない<sup>38</sup>。また  $n$  次の行列式は展開すると  $i_1, \dots, i_n$  の順列の個数すなわち  $n!$  個の項数となり、計算量も膨大となっていく。なにかしら計算量を減らす方法が望まれる。次項にて行列式の性質をさらに深掘りしよう。

<sup>36</sup> 歴史的にはこのように連立一次方程式の可解性を判定する指標として導入された。

<sup>37</sup> 一般的な行列式の定義である、ライプニッツの明示公式と同等であり、付録 4 にて言及する

<sup>38</sup> なぜか？ 4 次を例に同じような図を書いてみて理由を考えてみよう

**[4-3-3] 行列式の性質 I**

以下にまとめて列挙するが 【3-6】 節でみた「関数」  $D(\mathbf{a}, \mathbf{b}, \dots)$  の (列の) ベクトルに関する性質はそのまま引き継ぐ。3 次の場合を具体例として示す。高次も同様となる。

- ● (i) 各列のベクトルの多重線形性 : ベクトルの和

$$\begin{vmatrix} a_1 & b_1 + c_1 & d_1 \\ a_2 & b_2 + c_2 & d_2 \\ a_3 & b_3 + c_3 & d_3 \end{vmatrix} = \begin{vmatrix} a_1 & b_1 & d_1 \\ a_2 & b_2 & d_2 \\ a_3 & b_3 & d_3 \end{vmatrix} + \begin{vmatrix} a_1 & c_1 & d_1 \\ a_2 & c_2 & d_2 \\ a_3 & c_3 & d_3 \end{vmatrix} \quad (4-3-7)$$

- ● (ii) 各列のベクトルの多重線形性 : スカラー積

$$\begin{vmatrix} a_1 & kb_1 & c_1 \\ a_2 & kb_2 & c_2 \\ a_3 & kb_3 & c_3 \end{vmatrix} = k \begin{vmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{vmatrix} \quad (4-3-8)$$

- ● (iii) 列のベクトル間の交代性

$$\begin{vmatrix} a_1 & a_1 & b_1 \\ a_2 & a_2 & b_2 \\ a_3 & a_3 & b_3 \end{vmatrix} = 0 \quad \therefore \begin{vmatrix} b_1 & a_1 & c_1 \\ b_2 & a_2 & c_2 \\ b_3 & a_3 & c_3 \end{vmatrix} = - \begin{vmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{vmatrix} \quad (4-3-9)$$

- ● (iv) 標準基底を順に列のベクトルにもつ行列式の値は 1

$$\begin{vmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{vmatrix} = 1 \quad (4-3-10)$$

- ● (v) ある列のスカラー倍を別の列に加えても行列式の値は変わらない

$$\begin{vmatrix} a_1 & b_1 + kc_1 & c_1 \\ a_2 & b_2 + kc_2 & c_2 \\ a_3 & b_3 + kc_3 & c_3 \end{vmatrix} = \begin{vmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{vmatrix} \quad (4-3-11)$$

- ● (vi) 列のベクトルの組が線形従属  $\Rightarrow$  行列式の値は 0 (4-3-12)

(対偶 : 行列式の値が 0 でない  $\Rightarrow$  列のベクトルの組は線形独立)

(vi') 列のベクトルの組は線形独立である  $\Leftrightarrow$  行列式の値は 0 でない (次講第 3 節で示す)

これ以外のとても重要な性質として、行列式は行と列が完全に対等であることを示すことができ、上記を含め列に対して成立する性質がそのまま行に対しても成立する事がわかる。付録 1 に記載する。またこれを用いると、具体的には 3 次の場合だと

$$\begin{vmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{vmatrix} \leftrightarrow \begin{vmatrix} a_{11} & a_{21} & a_{31} \\ a_{12} & a_{22} & a_{32} \\ a_{13} & a_{23} & a_{33} \end{vmatrix}$$

のように行と列を入れ替えた (つまり  $a_{ij} \leftrightarrow a_{ji}$  となる) (係数) 行列を転置行列というが、転置してもその行列式は変化しない (値は等しい) 事が示せる。証明を同様に付録 1 に記載する。

- ● (vii) 転置行列の行列式は元の行列の行列式と等しい (4-3-13)

さらに上記の性質は行に対しても成り立つため、掃き出し法での行基本変形を当てはめて考えると

- ● (viii) 行基本変形に対する性質 (4-3-14)

- A) ある行の定数倍を別の行に加えても、行列式の値は変わらない (性質(v)より)
- B) ある行を (0 以外で) 定数倍すると、行列式の値も定数倍される (性質(ii)より)
- C) ある行と別の行を入れ替えると、行列式の符号が変わる (性質(iii)より)

行基本変形を適用して、以下のように行列式の 1 列目を 1 行目以外 0 にできたとしよう。4 次を例として考えてみる。 $a_{21} = a_{31} = a_{41} = 0$  に注意し行列式の定義より添字  $i$  で展開すると

$$\begin{vmatrix} a_{11} & a_{12} & a_{13} & a_{14} \\ 0 & a_{22} & a_{23} & a_{24} \\ 0 & a_{32} & a_{33} & a_{34} \\ 0 & a_{42} & a_{43} & a_{44} \end{vmatrix} = \sum_{i,j,k,l=1}^4 \varepsilon_{ijkl} a_{i1} a_{j2} a_{k3} a_{l4} = \sum_{j,k,l=1}^4 \varepsilon_{1jkl} a_{11} a_{j2} a_{k3} a_{l4} = a_{11} \sum_{j,k,l=1}^4 \varepsilon_{1jkl} a_{j2} a_{k3} a_{l4}$$

と  $i$  が 1 以外の項は残らない。最右辺は  $\varepsilon_{1jkl}$  と最初の添字が 1 に確定し、 $j, k, l$  が 1 になる項も残らなくなり  $a_{11}$  以外の 1 列目だけでなく 1 行目も除いた成分だけが残ることになる。また置換  $(1,2,3,4) \rightarrow (1,j,k,l)$  の偶奇性は先頭の 1 が不動なので置換  $(2,3,4) \rightarrow (j,k,l)$  の偶奇性と等しく、これは各数字を -1 した（各数字の名前をつけ直した）置換  $(1,2,3) \rightarrow (j-1,k-1,l-1)$  の偶奇性とも等しい(前講付録 3 演習参照)。つまり新たな添字を  $(J,K,L) = (j-1,k-1,l-1)$  と定義すれば  $\varepsilon_{1jkl} = \varepsilon_{JKL}$  と書ける（要するに 2,3,4 と 1,2,3 の並び替え方は同じということ）。そこで 1 行目と 1 列目を除いた係数行列を

$$\begin{vmatrix} a'_{11} & a'_{12} & a'_{13} \\ a'_{21} & a'_{22} & a'_{23} \\ a'_{31} & a'_{32} & a'_{33} \end{vmatrix} = \begin{vmatrix} a_{22} & a_{23} & a_{24} \\ a_{32} & a_{33} & a_{34} \\ a_{42} & a_{43} & a_{44} \end{vmatrix} \text{ として } a_{11} \text{ 以外の最右辺は} \sum_{j,k,l=1}^4 \varepsilon_{1jkl} a_{j2} a_{k3} a_{l4} = \sum_{j,k,l=2}^4 \varepsilon_{1jkl} a_{j2} a_{k3} a_{l4} = \sum_{j,K,L=1}^3 \varepsilon_{JKL} a'_{j1} a'_{k2} a'_{L3} = \begin{vmatrix} a'_{11} & a'_{12} & a'_{13} \\ a'_{21} & a'_{22} & a'_{23} \\ a'_{31} & a'_{32} & a'_{33} \end{vmatrix}$$

と書けることになり、この  $|a'_{JK}|$  のように成分（添字）を定義し直した場合の行列式という意味で

$$\begin{vmatrix} a_{11} & a_{12} & a_{13} & a_{14} \\ 0 & a_{22} & a_{23} & a_{24} \\ 0 & a_{32} & a_{33} & a_{34} \\ 0 & a_{42} & a_{43} & a_{44} \end{vmatrix} = a_{11} \begin{vmatrix} a_{22} & a_{23} & a_{24} \\ a_{32} & a_{33} & a_{34} \\ a_{42} & a_{43} & a_{44} \end{vmatrix}$$

となる。以上の議論は、より高次にも全く同様に適用でき以下が成り立つことがわかる。

● (ix) 行列式の次数下げ

$$\begin{vmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ 0 & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ 0 & a_{n2} & \cdots & a_{nn} \end{vmatrix} = a_{11} \begin{vmatrix} a_{22} & \cdots & a_{2n} \\ \vdots & \ddots & \vdots \\ a_{n2} & \cdots & a_{nn} \end{vmatrix} \quad (4-3-15)$$

※幾何学的解釈 : 3 次を例とする。 $\begin{vmatrix} a_1 & b_1 & c_1 \\ 0 & b_2 & c_2 \\ 0 & b_3 & c_3 \end{vmatrix} = a_1 \begin{vmatrix} b_2 & c_2 \\ b_3 & c_3 \end{vmatrix}$ 

左辺は 3 本のベクトル  $a, b, c$  が張る平行六面体の体積を表し、右辺は  $b, c$  を 2-3 平面に射影した  $b', c'$  が張る平行四辺形の面積に高さ  $a_1$  を掛けたものとなる。このように  $n$  次の場合 ( $n$  次元体積) = ( $n$  次元目の高さ) × ( $n-1$  次元体積) と解釈できる。

![](_page_61_Picture_31.jpeg)

● (x) 上三角行列の行列式

成分  $a_{ij} = 0$  ( $i > j$ ) となる（係数）行列を**上三角行列**といい、次数下げを繰り返し適用できる。

$$\begin{vmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ 0 & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \cdots & a_{nn} \end{vmatrix} = a_{11} a_{22} \cdots a_{nn} \quad (4-3-16)$$

<span id="page-62-0"></span>**【4-4】 行列の導入**

**【4-3-1】 導入小話 : もしかすると行列つて · · · ·**

拡大係数行列は、連立一次方程式を以下のように表示していた（とりあえず 2 行 2 列で）。

$$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} e \\ f \end{bmatrix} \quad \begin{cases} ax + by = e \\ cx + dy = f \end{cases}$$

係数や定数項の値だけでなく、方程式そのものを表示するにはどうすればよいだろうか？

方程式なので両辺を等号で結ぶ形にしたい。連立方程式の定数項はセットにして等号の右辺に置きたい。変数も同じようにセットにして、係数行列と共に左辺に置きたい。こんな感じで。

$$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} e \\ f \end{bmatrix}$$

左辺を係数行列と変数の積とみて、積を定義しよう。方程式を再現させるには、左辺の係数のそれぞれの行と変数の列の積が、右辺定数項のそれぞれの値になるように、

$$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} \equiv \begin{bmatrix} ax + by \\ cx + dy \end{bmatrix} \quad (4-4-1)$$

という演算を定義すればよいだろう。

ついでに連立方程式が変数変換しても成り立つようにしておこう。 $(x, y) \rightarrow (u, v)$  となる

$$\begin{cases} x = \alpha u + \beta v \\ y = \gamma u + \delta v \end{cases} \quad (4-4-2)$$

という変数変換<sup>39</sup>を行うと、連立方程式の左辺は

$$\begin{cases} ax + by = a(\alpha u + \beta v) + b(\gamma u + \delta v) = (a\alpha + b\gamma)u + (a\beta + b\delta)v \\ cx + dy = c(\alpha u + \beta v) + d(\gamma u + \delta v) = (c\alpha + d\gamma)u + (c\beta + d\delta)v \end{cases} \quad (4-4-3)$$

となるが、(4-4-1) 式で定義した積を使うと、(4-4-2)式と(4-4-3)式はそれぞれ

$$\begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} \alpha & \beta \\ \gamma & \delta \end{bmatrix} \begin{bmatrix} u \\ v \end{bmatrix}, \quad \begin{bmatrix} ax + by \\ cx + dy \end{bmatrix} = \begin{bmatrix} a\alpha + b\gamma & a\beta + b\delta \\ c\alpha + d\gamma & c\beta + d\delta \end{bmatrix} \begin{bmatrix} u \\ v \end{bmatrix}$$

と書ける。これを (4-4-1) 式の両辺に代入すると

$$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} \alpha & \beta \\ \gamma & \delta \end{bmatrix} \begin{bmatrix} u \\ v \end{bmatrix} = \begin{bmatrix} a\alpha + b\gamma & a\beta + b\delta \\ c\alpha + d\gamma & c\beta + d\delta \end{bmatrix} \begin{bmatrix} u \\ v \end{bmatrix}$$

となるので、

$$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} \alpha & \beta \\ \gamma & \delta \end{bmatrix} \equiv \begin{bmatrix} a\alpha + b\gamma & a\beta + b\delta \\ c\alpha + d\gamma & c\beta + d\delta \end{bmatrix} \quad (4-4-4)$$

という積を定義すればよいだろう。ん？この積もしかして逆に掛けると

$$\begin{bmatrix} \alpha & \beta \\ \gamma & \delta \end{bmatrix} \begin{bmatrix} a & b \\ c & d \end{bmatrix} = \begin{bmatrix} a\alpha + c\beta & b\alpha + d\beta \\ a\gamma + c\delta & b\gamma + d\delta \end{bmatrix}$$

となって、非可換<sup>40</sup>だな。ま、しょうがないか。これを行列と呼ぶことにしよう。

・・・・という感じで発見されたのかも。知らないけど。

<sup>39</sup> 一次変換であることに注意

<sup>40</sup> 可換 : 交換則が成り立つ ( $ab = ba$ )、非可換 : 交換則が成り立たない ( $ab \neq ba$ ) ということ

**[4-4-2] 行列と演算の定義**

●行列 : 数や変数・定数・式などを表す文字を  $n$ 個  $\times m$ 個 の形に縦横に並べて、括弧でくくったものを行列といい数や文字をその成分という。本講座では、成分は実数のみ、行列は  $n = m$  の場合（**正方行列**という）のみを対象とする。例外は後述する  $1 \times n$  または  $n \times 1$  行列。

●行と列 例 :  $2 \times 2$  行列  $\begin{bmatrix} a & b \\ c & d \end{bmatrix}$  以降、この行列を例にとって説明する横に並んだ  $a$   $b$  や  $c$   $d$  を行、縦に並んだ  $a$  や  $b$  を列という<sup>41</sup>。行と列に関わるあらゆるものは、行が先、列が後の順番になる。例えば、 $2 \times 1$  行列は 2 行 1 列の行列を意味し  $\begin{bmatrix} a \\ c \end{bmatrix}$  のように書く。列のみの行列であり、**列ベクトル**（縦ベクトル）ともいう。同様に  $1 \times 2$  行列は 1 行 2 列の行列を意味し  $\begin{bmatrix} a & b \end{bmatrix}$  のように書く。行のみの行列であり、**行ベクトル**（横ベクトル）ともいう。

●成分 : 成分も行と列の順で表す。例えば (1,2) 成分は 1 行 2 列目のことを指し、例では  $b$  を指す。添字を使って  $a_{ij}$  のように表記することもあり、 $i$  行  $j$  列目の成分を意味する。この場合、行列として表記すると  $\begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix}$  となる。混同しやすいので注意。 $a_{行列}$  : 行、列の順。

●表記 : これまでの例のように括弧で成分をくくった表記以外に、 $A$  のように（通常）大文字のアルファベットで表すこともある。その際、列ベクトルはベクトルの表記に習い  $x$  のように太文字で表す。またこの場合、行列式<sup>42</sup>は  $\det(A)$  とも書かれる。ちなみに行列の括弧も大括弧  $[ \ ]$  と小括弧  $( \ )$  どちらもあるが、本講座では大括弧を採用する<sup>43</sup>。

●対角成分と単位行列、零行列 : 例だと  $a$  や  $d$  のように行と列が一致した対角線上に並んだ成分を**対角成分**という。対角成分のみ 1 で、他は 0 となる成分をもつ行列を**単位行列**という。

例 :  $\begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}$  単位行列は  $E$  または  $I$  と表記される。本講座では  $E$  を採用する。成分が全て 0 の行列を**零行列**という。通常アルファベット大文字の 0 と表記される。

●転置行列 :  $\begin{bmatrix} a & b \\ c & d \end{bmatrix} \rightarrow \begin{bmatrix} a & c \\ b & d \end{bmatrix}$  のように行と列の成分を入れ替えた行列を**転置行列**といい行列  $A$  の転置行列は  $A^T$  のように右肩に  $T$  を載せて表記する。成分の添字で表わすと  $(A^T)_{ij} = (A)_{ji}$  ということになる。（左肩に  $t$  を載せ  ${}^t A$  とする表記もある。）

<sup>41</sup> 日本語は本来縦書きなので混同しやすいが、西洋では行とは横に並んだ文字列を指す

<sup>42</sup> 英語では determinant といい、「決定因子」くらいの意味となる

<sup>43</sup> 使用している数式エディタの場合、小括弧だとやや見にくくなるので

●行列の和とスカラー積

ベクトルの和やスカラー積と同様に、成分同士の和、全成分に対する積と定義される。

$$\text{和} : \begin{bmatrix} a & b \\ c & d \end{bmatrix} + \begin{bmatrix} e & f \\ g & h \end{bmatrix} \equiv \begin{bmatrix} a+e & b+f \\ c+g & d+h \end{bmatrix} \quad \text{スカラー積} : k \begin{bmatrix} a & b \\ c & d \end{bmatrix} \equiv \begin{bmatrix} ka & kb \\ kc & kd \end{bmatrix} \quad (4-4-5)$$

●行列と列ベクトル、行ベクトルと行列の積

○  $n \times n$  行列と  $n \times 1$  行列である列ベクトルとの積が  $n \times 1$  行列の列ベクトルとなる。  
 $n$  が 2, 3 の場合は以下のように定義される。

$$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} \equiv \begin{bmatrix} ax+by \\ cx+dy \end{bmatrix}, \quad \begin{bmatrix} a & b & c \\ d & e & f \\ g & h & i \end{bmatrix} \begin{bmatrix} x \\ y \\ z \end{bmatrix} \equiv \begin{bmatrix} ax+by+cz \\ dx+ey+fz \\ gx+hy+iz \end{bmatrix} \quad (4-4-6)$$

理論的な話の場合、添字での表記が用いられる事が多く、規則性が分かりやすくなる。

$$\mathbf{y} = A\mathbf{x} \quad \text{に対し} \quad y_i = \sum_{j=1}^n a_{ij}x_j \quad (4-4-7)$$

 $\mathbf{y}$  の  $i$  行目の成分は、 $A$  の  $i$  行と  $\mathbf{x}$  との成分同士の積の和となっている事が分かる。

○  $1 \times n$  行列である行ベクトルと  $n \times n$  行列との積が  $1 \times n$  行列の行ベクトルとなる。  
 $n$  が 2, 3 の場合は以下のように定義される。

$$\begin{bmatrix} x & y \\ z & w \end{bmatrix} \begin{bmatrix} a & b \\ d & e \\ g & h \\ i & j \end{bmatrix} \equiv \begin{bmatrix} ax+by & bx+dy \\ ax+dy+gz & bx+ey+hz \\ cx+fy+iz & cx+fy+iz \end{bmatrix} \quad (4-4-8)$$

添字での表記では（列ベクトルの転置行列でもある行ベクトルを  $\mathbf{x}^T$  のように表記して）

$$\mathbf{y}^T = \mathbf{x}^T A \quad \text{に対し} \quad y_j = \sum_{i=1}^n x_i a_{ij} \quad (4-4-9)$$

 $\mathbf{y}^T$  の  $j$  列目の成分は、 $\mathbf{x}^T$  と  $A$  の  $j$  列との成分同士の積の和となっている事が分かる。

●行列と行列との積

 $n \times n$  行列と  $n \times n$  行列との積が  $n \times n$  行列となる。 $n$  が 2, 3 の場合は以下のように定義される。

$$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} w & x \\ y & z \end{bmatrix} \equiv \begin{bmatrix} aw+by & ax+bz \\ cw+dy & cx+dz \end{bmatrix} \\ \begin{bmatrix} a & b & c \\ d & e & f \\ g & h & i \end{bmatrix} \begin{bmatrix} r & s & t \\ u & v & w \\ x & y & z \end{bmatrix} \equiv \begin{bmatrix} ar+bu+cx & as+bv+cy & at+bw+cz \\ dr+eu+fx & ds+ev+fy & dt+ew+fz \\ gr+hu+ix & gs+hv+iy & gt+hw+iz \end{bmatrix} \quad (4-4-10)$$

添字での表記では

$$AB = C \quad \text{に対し} \quad c_{ij} = \sum_{k=1}^n a_{ik}b_{kj} \quad (4-4-11)$$

この場合、 $C$  の  $(i,j)$  成分は、 $A$  の  $i$  行と  $B$  の  $j$  列との成分同士の積の和となる。

**[4-4-3] 行列の基本性質**

任意の正方行列  $A, B, C$ 、単位行列  $E$ 、零行列  $O$ 、スカラー  $k, l$  に対して以下が成り立つ。

● 和とスカラー積 : ベクトル空間の公理を満たす

| (i) $A + B = B + A$              | (vi) $(k + l)A = kA + lA$   |
|----------------------------------|-----------------------------|
| (ii) $(A + B) + C = A + (B + C)$ | (vii) $k(lA) = (kl)A$       |
| (iii) $A + O = O + A = A$        | (viii) $1A = A, (-1)A = -A$ |
| (iv) $A + (-A) = (-A) + A = O$   | (ix) $0A = O, kO = O$       |
| (v) $k(A + B) = kA + kB$         |                             |

● 積

| (i) $(AB)C = A(BC)$       | (iii) $AE = EA = A$ |
|---------------------------|---------------------|
| (ii) $(A + B)C = AC + BC$ | (iv) $OA = AO = O$  |
| $A(B + C) = AB + AC$      |                     |

**[4-4-4] 連立一次方程式の行列による表示**

行列とその積が定義されたので、行列を使って連立一次方程式を表してみよう。

例えば 3 元連立一次方程式の場合、

$$\begin{cases} a_{11}x_1 + a_{12}x_2 + a_{13}x_3 = b_1 \\ a_{21}x_1 + a_{22}x_2 + a_{23}x_3 = b_2 \\ a_{31}x_1 + a_{32}x_2 + a_{33}x_3 = b_3 \end{cases}$$

に対して、

$$\begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \\ x_3 \end{bmatrix} = \begin{bmatrix} b_1 \\ b_2 \\ b_3 \end{bmatrix} \quad \text{or} \quad \sum_{j=1}^3 a_{ij}x_j = b_i$$

また以下のようにも書ける。

$$A = \begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix}, \quad x = \begin{bmatrix} x_1 \\ x_2 \\ x_3 \end{bmatrix}, \quad b = \begin{bmatrix} b_1 \\ b_2 \\ b_3 \end{bmatrix} \quad \text{とすれば} \quad Ax = b$$

最後の式  $Ax = b$  は、まるで一次方程式  $ax = b$  のようにもみえる。 $ax = b$  が  $a \neq 0$  の時に  $x = \frac{1}{a}b$  と解くことができたように、連立一次方程式も解けないのだろうか？この 1 次方程式の可解条件  $a \neq 0$  は、行列式  $|A| \neq 0$  に対応しているのではないか？

そもそも  $\frac{1}{a}$  とは何だろう？  $a$  の逆数である  $\frac{1}{a}$  は一次方程式  $ax' = 1$  の解とみることもでき、この  $x'$  を右辺  $b$  に掛けた  $x'b$  が元の一次方程式  $ax = b$  の解とみることもできる。

このことを行列形式で書いた連立一次方程式に拡張してみよう。 $ax' = 1$  の右辺の 1 にあたるものは積の基本性質(iii)から単位行列  $E$  としてよいだろう。左辺の  $a$  に相当するものは係数行列  $A$  なので、 $x'$  に相当するものも行列となり、 $Ax' = E$  となりそうだ。標語的に書けば :

$$ax = b: ax' = 1 \rightarrow x = x'b \quad \Rightarrow \quad Ax = b: Ax' = E \rightarrow x = X'b ?$$

実際  $x = X'b$  として左から  $A$  を掛けると  $Ax = AX'b = Eb = b$  となり式を満たすことになる。この  $AX' = E$  を満たす  $X'$  は、行列  $A$  の逆数に相当するものといえるかも知れない。

3 次を例に具体的に考えてみよう。 $AX' = E$  を成分で書くと

$$\begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} \begin{bmatrix} x'_{11} & x'_{12} & x'_{13} \\ x'_{21} & x'_{22} & x'_{23} \\ x'_{31} & x'_{32} & x'_{33} \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$$

となる。よく見ればこれは

$$x'_1 = \begin{bmatrix} x'_{11} \\ x'_{21} \\ x'_{31} \end{bmatrix}, x'_2 = \begin{bmatrix} x'_{12} \\ x'_{22} \\ x'_{32} \end{bmatrix}, x'_3 = \begin{bmatrix} x'_{13} \\ x'_{23} \\ x'_{33} \end{bmatrix} \quad e_1 = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}, e_2 = \begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix}, e_3 = \begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}$$

としたときの

$$Ax'_1 = e_1, \quad Ax'_2 = e_2, \quad Ax'_3 = e_3$$

という連立一次方程式 3 セットとみることもでき、 $x'_1, x'_2, x'_3$  をそれぞれ求めることができる。

もはや興味の対象は連立一次方程式を解くことから行列の逆数に相当するものに移っているが、 $x'_1, x'_2, x'_3$  を掃き出し法で求めてみよう。掃き出し法とは連立一次方程式  $Ax = b$  に対して行基本変形を用いて  $[A|b] \rightarrow [E|x]$  として解く手法だった。行基本変形は直接加減し合うのは同じ列の間だけであり、係数行列が同じ場合は定数項である列ベクトルを並べ  $[A|e_1 e_2 e_3] \rightarrow [E|x'_1 x'_2 x'_3]$  として 3 つの連立方程式を一度に解けることになる。この場合の拡大係数行列は

$$\begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$$

となる。実際に本講の冒頭の 2 例でみてみよう。

$$\begin{bmatrix} 1 & 1 & 2 & 1 & 0 & 0 \\ 2 & 1 & 3 & 0 & 1 & 0 \\ 1 & 2 & 4 & 0 & 0 & 1 \end{bmatrix} \quad \begin{bmatrix} 1 & -1 & 3 & 1 & 0 & 0 \\ -1 & 1 & -2 & 0 & 1 & 0 \\ 2 & -3 & 4 & 0 & 0 & 1 \end{bmatrix}$$

これにそれぞれ行基本変形を適応させる。掃き出す手順は冒頭と全く同じことに注意。

$$\begin{bmatrix} 1 & 1 & 2 & 1 & 0 & 0 \\ 0 & -1 & -1 & -2 & 1 & 0 \\ 0 & 1 & 2 & -1 & 0 & 1 \end{bmatrix} \begin{matrix} r_2 - 2r_1 \\ r_3 - r_1 \end{matrix} \quad \begin{bmatrix} 1 & -1 & 3 & 1 & 0 & 0 \\ 0 & 0 & 1 & 1 & 1 & 0 \\ 0 & -1 & -2 & -2 & 0 & 1 \end{bmatrix} \begin{matrix} r_2 + r_1 \\ r_2 - 2r_1 \end{matrix}$$

$$\begin{bmatrix} 1 & 1 & 2 & 1 & 0 & 0 \\ 0 & 1 & 1 & 2 & -1 & 0 \\ 0 & 1 & 2 & -1 & 0 & 1 \end{bmatrix} \begin{matrix} r_2 \times (-1) \\ \\ \\ \end{matrix} \quad \begin{bmatrix} 1 & -1 & 3 & 1 & 0 & 0 \\ 0 & -1 & -2 & -2 & 0 & 1 \\ 0 & 0 & 1 & 1 & 1 & 0 \end{bmatrix} \begin{matrix} r_2 \leftrightarrow r_3 \\ \\ \\ \end{matrix}$$

$$\begin{bmatrix} 1 & 1 & 2 & 1 & 0 & 0 \\ 0 & 1 & 1 & 2 & -1 & 0 \\ 0 & 0 & 1 & -3 & 1 & 1 \end{bmatrix} \begin{matrix} r_3 - r_2 \\ \\ \\ \end{matrix} \quad \begin{bmatrix} 1 & -1 & 3 & 1 & 0 & 0 \\ 0 & 1 & 2 & 2 & 0 & -1 \\ 0 & 0 & 1 & 1 & 1 & 0 \end{bmatrix} \begin{matrix} r_2 \times (-1) \\ \\ \\ \end{matrix}$$

$$\begin{bmatrix} 1 & 1 & 0 & 7 & -2 & -2 \\ 0 & 1 & 0 & 5 & -2 & -1 \\ 0 & 0 & 1 & -3 & 1 & 1 \end{bmatrix} \begin{matrix} r_1 - 2r_3 \\ r_2 - r_3 \\ \\ \end{matrix} \quad \begin{bmatrix} 1 & -1 & 0 & -2 & -3 & 0 \\ 0 & 1 & 0 & 0 & -2 & -1 \\ 0 & 0 & 1 & 1 & 1 & 0 \end{bmatrix} \begin{matrix} r_1 - 3r_3 \\ \\ \\ \end{matrix}$$

$$\begin{bmatrix} 1 & 0 & 0 & 2 & 0 & -1 \\ 0 & 1 & 0 & 5 & -2 & -1 \\ 0 & 0 & 1 & -3 & 1 & 1 \end{bmatrix} \begin{matrix} r_1 - r_2 \\ \\ \\ \end{matrix} \quad \begin{bmatrix} 1 & 0 & 0 & -2 & -5 & -1 \\ 0 & 1 & 0 & 0 & -2 & -1 \\ 0 & 0 & 1 & 1 & 1 & 0 \end{bmatrix} \begin{matrix} r_1 + r_2 \\ \\ \\ \end{matrix}$$

元の連立方程式 (  $Ax = b$  )

$$\begin{bmatrix} 1 & 1 & 2 \\ 2 & 1 & 3 \\ 1 & 2 & 4 \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \\ x_3 \end{bmatrix} = \begin{bmatrix} 9 \\ 13 \\ 17 \end{bmatrix} \quad \begin{bmatrix} 1 & -1 & 3 \\ -1 & 1 & -2 \\ 2 & -3 & 4 \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \\ x_3 \end{bmatrix} = \begin{bmatrix} 8 \\ -5 \\ 8 \end{bmatrix}$$

に対して得られた行列 (  $AX' = E$  となるはずの  $X'$  ) はそれぞれ

$$\begin{bmatrix} 2 & 0 & -1 \\ 5 & -2 & -1 \\ -3 & 1 & 1 \end{bmatrix} \quad \begin{bmatrix} -2 & -5 & -1 \\ 0 & -2 & -1 \\ 1 & 1 & 0 \end{bmatrix}$$

であり、実際に積 (  $AX'$  ) をとってみると ( 確かめよう)

$$\begin{bmatrix} 1 & 1 & 2 \\ 2 & 1 & 3 \\ 1 & 2 & 4 \end{bmatrix} \begin{bmatrix} 2 & 0 & -1 \\ 5 & -2 & -1 \\ -3 & 1 & 1 \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix} \quad \begin{bmatrix} 1 & -1 & 3 \\ -1 & 1 & -2 \\ 2 & -3 & 4 \end{bmatrix} \begin{bmatrix} -2 & -5 & -1 \\ 0 & -2 & -1 \\ 1 & 1 & 0 \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$$

確かに積は単位行列となった。さらに元の連立方程式の右辺定数項との積 (  $X'b$  ) は

$$\begin{bmatrix} 2 & 0 & -1 \\ 5 & -2 & -1 \\ -3 & 1 & 1 \end{bmatrix} \begin{bmatrix} 9 \\ 13 \\ 17 \end{bmatrix} = \begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix} \quad \begin{bmatrix} -2 & -5 & -1 \\ 0 & -2 & -1 \\ 1 & 1 & 0 \end{bmatrix} \begin{bmatrix} 8 \\ -5 \\ 8 \end{bmatrix} = \begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix}$$

となり、確かに冒頭で解いた解と一致するではないか ( 確かめよう)。

行列の逆数にあたるものを掃き出し法で求められそうなことがわかった。もしこの  $AX' = E$  となる  $X'$  が  $X'A = E$  でもあれば、 $Ax = b$  の左から  $X'$  を掛けて  $x = X'b$  が直接いえ、まさに逆数に相当するといえそうだ。実は上記の例の  $X'$  は  $X'A = E$  でもある ( 確かめよう)。このことは偶然なのだろうか？次講でこの行列の逆数にあたるものを含め、さらに深く探っていこう。

<span id="page-67-0"></span>**【4-5】 付録 1 : 行列式の重要な性質**

● 行列式の重要な性質

3 次を例として以下を考える。行列式は列をベクトルとしてみなし  $a_j = \sum_{i=1}^3 a_{ij} e_i$  としたとき

$$|A| = \begin{vmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{vmatrix} = D(a_1, a_2, a_3) = \sum_{i,j,k=1}^3 \varepsilon_{ijk} a_{i1} a_{j2} a_{k3}$$

として定義された。ここで  $D(a_l, a_m, a_n)$  ( $1 \leq l, m, n \leq 3$ ) を考えてみよう。まず  $D(a_l, a_m, a_n)$  のベクトルの入れ替えに対する交代性により  $(l, m, n)$  の値が全て異なる場合のみ 0 以外の値を持ちえる。 $(l, m, n) = (1, 2, 3)$  の時は定義より行列式  $|A|$  となり、それ以外は同様にベクトルの入れ替えにより符号が変わるだけで  $(l, m, n)$  が  $(1, 2, 3)$  の偶/奇置換のとき  $\pm |A|$  となる。以上をまとめると

$$D(a_l, a_m, a_n) = \begin{cases} +|A| & \text{if } (l, m, n) \text{ が} (1, 2, 3) \text{ の偶置換} : (1, 2, 3), (2, 3, 1), (3, 1, 2) \\ -|A| & \text{if } (l, m, n) \text{ が} (1, 2, 3) \text{ の奇置換} : (1, 3, 2), (2, 1, 3), (3, 2, 1) \\ 0 & \text{other} \end{cases}$$

となり、これは  $|A|$  を掛けた  $\varepsilon_{lmn}$  そのものである。よって 以下のように書けることになる。

$$D(a_l, a_m, a_n) = |A| \varepsilon_{lmn}$$

一方左辺は  $a_l = \sum_{i=1}^3 a_{il} e_i$  等により  $\sum_{i,j,k=1}^3 a_{il} a_{jm} a_{kn} D(e_i, e_j, e_k) = \sum_{i,j,k=1}^3 \varepsilon_{ijk} a_{il} a_{jm} a_{kn}$ 

とも書けるため、結果として以下が成り立つ。

$$\sum_{i,j,k=1}^3 \varepsilon_{ijk} a_{il} a_{jm} a_{kn} = |A| \varepsilon_{lmn} \quad (4-5-1)$$

この両辺に  $\varepsilon_{lmn}$  を掛けて添字  $l, m, n$  の総和をとると (  $\sum_{l,m,n=1}^3 \varepsilon_{lmn} \varepsilon_{lmn} = \sum_{l \neq m \neq n} 1 = 3!$  より)

$$\sum_{i,j,k=1}^3 \sum_{l,m,n=1}^3 \varepsilon_{ijk} \varepsilon_{lmn} a_{il} a_{jm} a_{kn} = |A| \sum_{l,m,n=1}^3 \varepsilon_{lmn} \varepsilon_{lmn} = 3! |A|$$

$$\therefore |A| = \frac{1}{3!} \sum_{i,j,k=1}^3 \sum_{l,m,n=1}^3 \varepsilon_{ijk} \varepsilon_{lmn} a_{il} a_{jm} a_{kn} \quad (4-5-2)$$

が成り立つ。全く同様の議論により、 $n$  次の行列式に対して以下が成り立つ。

$$\sum_{i_1, \dots, i_n=1}^n \varepsilon_{i_1 \dots i_n} a_{i_1 j_1} \dots a_{i_n j_n} = |A| \varepsilon_{j_1 \dots j_n} \quad (4-5-3)$$

$$|A| = \frac{1}{n!} \sum_{i_1, \dots, i_n=1}^n \sum_{j_1, \dots, j_n=1}^n \varepsilon_{i_1 \dots i_n} \varepsilon_{j_1 \dots j_n} a_{i_1 j_1} \dots a_{i_n j_n} \quad (4-5-4)$$

これにより、行列式の行と列は完全に対等である (従って同等の性質を持つ) ことがわかる。

3次を例に説明すると、(4-5-2)式を添字  $l, m, n$  について展開し  $\varepsilon_{ijk}$  の交代性に着目し整理すると元の行列式の定義  $|A| = \sum_{i,j,k=1}^3 \varepsilon_{ijk} a_{i1} a_{j2} a_{k3}$  に帰着するが、逆に添字  $i, j, k$  について展開して整理することで  $|A| = \sum_{l,m,n=1}^3 \varepsilon_{lmn} a_{1l} a_{2m} a_{3n}$  を得る。前者が行列を列ベクトルの組として捉えているのに対し、後者は行ベクトルの組とした場合に相当し、行列式として両者は代数的に全く同じようにふるまい、列ベクトルとみなした場合に持つ (列に対する) 性質は行ベクトルとみなした場合も (行に対しても) 同様に成り立つ。(4-5-2)式、(4-5-4)式はそう主張している。

●転置行列の行列式 :  $|A^T| = |A|$  (総和記号に不慣れな場合は 第 2 講 付録 2 参照)

【証明】 3次の場合でみてみると (4-5-2) 式および  $a_{ij}^T = a_{ji}$  より

$$|A^T| = \frac{1}{3!} \sum_{i,j,k=1}^3 \sum_{l,m,n=1}^3 \varepsilon_{ijk} \varepsilon_{lmn} a_{il}^T a_{jm}^T a_{kn}^T$$

$$= \frac{1}{3!} \sum_{i,j,k=1}^3 \sum_{l,m,n=1}^3 \varepsilon_{ijk} \varepsilon_{lmn} a_{il} a_{mj} a_{nk} = \frac{1}{3!} \sum_{l,m,n=1}^3 \sum_{i,j,k=1}^3 \varepsilon_{lmn} \varepsilon_{ijk} a_{il} a_{mj} a_{nk} = |A|$$

 $n$  次の場合も同様となる。 ■

●行列の積の行列式 :  $|AB| = |A||B|$  (ついでに示す 本編での登場は第 5 講 第 3 節にて)

【証明】  $C = AB$  として 3次の場合でみてみると  $c_{ij} = \sum_{k=1}^3 a_{ik} b_{kj}$  と (4-5-1) 式より

$$|AB| = |C| = \sum_{i,j,k=1}^3 \varepsilon_{ijk} c_{i1} c_{j2} c_{k3} = \sum_{i,j,k=1}^3 \sum_{l,m,n=1}^3 \varepsilon_{ijk} a_{il} b_{l1} a_{jm} b_{m2} a_{kn} b_{n3}$$

$$= \sum_{l,m,n=1}^3 \sum_{i,j,k=1}^3 \varepsilon_{ijk} a_{il} a_{jm} a_{kn} b_{l1} b_{m2} b_{n3} = \sum_{l,m,n=1}^3 |A| \varepsilon_{lmn} b_{l1} b_{m2} b_{n3} = |A||B|$$

<span id="page-69-0"></span>**【4-6】 付録 2 : 簡約行列の構造**

簡約行列は定義に従うと rank に応じてとり得るパターンは限られ、例として行列の次数 2,3,4 に対して列挙すると以下のようになり、より高次も同様となる。

\*の成分は任意の値 小括弧内の数字は (rank, 解の自由度) を表す

○ 2 次

$$(2,0): \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}, \quad (1,1): \begin{bmatrix} 1 & * \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix}, \quad (0,2): \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix}$$

○ 3 次

$$(3,0): \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}, \quad (2,1): \begin{bmatrix} 1 & 0 & * \\ 0 & 1 & * \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 1 & * & 0 \\ 0 & 0 & 1 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 & 0 \\ 0 & 0 & 1 \\ 0 & 0 & 0 \end{bmatrix}$$

$$(1,2): \begin{bmatrix} 1 & * & * \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 & * \\ 0 & 0 & * \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 1 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{bmatrix}, \quad (0,3): \begin{bmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{bmatrix}$$

○ 4 次

$$(4,0): \begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{bmatrix}, \quad (3,1): \begin{bmatrix} 1 & 0 & 0 & * \\ 0 & 1 & 0 & * \\ 0 & 0 & 1 & * \\ 0 & 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 1 & 0 & * & 0 \\ 0 & 1 & * & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 1 & * & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix}$$

$$(2,2): \begin{bmatrix} 1 & 0 & * & * \\ 0 & 1 & * & * \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 1 & * & 0 & * \\ 0 & 0 & 1 & * \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 1 & * & * & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 & * & 0 \\ 0 & 0 & 1 & * \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 & * & * \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}, (0,4): \begin{bmatrix} 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}$$

○ 主成分がない行 : 連立させる方程式が全て独立でない場合は行基本変形により掃き出され、その式に対応する行は全て 0 となり、行の入れ替えにより下の方に集められていく。連立方程式の解が不定となる場合、この全成分が 0 の行の数は、解の自由度を意味することになる。

○ 主成分がある行 : 残った主成分のある行の数が独立な式の数を意味する rank となる。(主成分の定義より) この行の 1 である主成分の左側は全て 0 となり、右側は任意の値(\*)をとり得る。各主成分は行列の上から行を降りるごとに右側にすなわち階段状に配置され、配置される列の選び方 : (次数) n 列の中から (rank) r 列を選ぶ組み合わせの数  $_nC_r$  だけパターンがあることになる。

○ 主成分がある列 : この列の主成分の下側はもちろん、上側の各成分の各行の左側に別の主成分があって任意の値をとり得る成分(\*)も掃き出されて 0 となる。

○ 主成分がない列 : この列の左側の列に主成分があれば、任意の値を持ちうるその行の成分(\*)は掃き出すことができずに残る。左側のどの列にも主成分がなければ、主成分の左側は 0 なので、この主成分がない列は全て 0 となることになる。行基本変形は同じ列の間だけで直接加減しあうので、この列は最初から全て 0 すなわち該当する変数の係数が最初から全て 0 である特殊な場合となる。

<span id="page-70-0"></span>**【4-7】 付録 3 : 補足説明**

● 3 次元空間における平面の方程式

3 次元空間における平面をベクトルで表そう。平面の法線ベクトルを  $\mathbf{n} = (a, b, c)$ 、平面の代表点の位置ベクトルを  $\mathbf{r}_0 = (x_0, y_0, z_0)$ 、平面上の任意の点の位置ベクトルを  $\mathbf{r} = (x, y, z)$  とすると、ベクトル  $\mathbf{r} - \mathbf{r}_0$  は法線ベクトル  $\mathbf{n}$  と直交するので平面の方程式は  $\mathbf{n} \cdot (\mathbf{r} - \mathbf{r}_0) = 0$  と書ける。

![](_page_70_Picture_24.jpeg)

これは  $ax + by + cz = ax_0 + by_0 + cz_0$  となり右辺を  $d$  とすれば 3 元一次方程式  $ax + by + cz = d$  と解釈できる。今、 $\mathbf{r}_0$  を動かすことを考えよう。 $\mathbf{r}_0 \rightarrow \mathbf{r}'_0 = \mathbf{r}_0 + \Delta_\perp + \Delta_{//}$  とし、変位量を平面に垂直な方向  $\Delta_\perp$  と平行な方向  $\Delta_{//}$  に分解して考えると、 $\mathbf{n}$  と  $\Delta_{//}$  は直交するので、一次方程式の右辺  $d \rightarrow d' = \mathbf{n} \cdot \mathbf{r}'_0 = \mathbf{n} \cdot (\mathbf{r}_0 + \Delta_\perp + \Delta_{//}) = \mathbf{n} \cdot \mathbf{r}_0 + \mathbf{n} \cdot \Delta_\perp = d + \mathbf{n} \cdot \Delta_\perp$  となり、平面に平行な変位は  $d$  の変化に寄与しない。つまり同じ平面上の代表点  $\mathbf{r}_0$  のとり方には依らないことを意味する。逆に右辺  $d$  が変化すると、平面全体は法線ベクトルの方向（逆向きを含む）に平行移動することになる。

● 行基本変形と線形結合関係

行基本変形が線形結合関係を保つことを、2 次を例として示す。高次も同様となる。

2 元連立一次方程式  $x \begin{bmatrix} a_1 \\ a_2 \end{bmatrix} + y \begin{bmatrix} b_1 \\ b_2 \end{bmatrix} = \begin{bmatrix} c_1 \\ c_2 \end{bmatrix}$  が成り立つとき、行基本変形  $\begin{bmatrix} a_1 & b_1 \\ a_2 & b_2 \end{bmatrix} \begin{bmatrix} c_1 \\ c_2 \end{bmatrix} \rightarrow \begin{bmatrix} a'_1 & b'_1 \\ a'_2 & b'_2 \end{bmatrix} \begin{bmatrix} c'_1 \\ c'_2 \end{bmatrix}$ 

を行っても、 $x \begin{bmatrix} a'_1 \\ a'_2 \end{bmatrix} + y \begin{bmatrix} b'_1 \\ b'_2 \end{bmatrix} = \begin{bmatrix} c'_1 \\ c'_2 \end{bmatrix}$  が成り立つことを示すことになる。

(A)  $r_1 \leftrightarrow r_2 : \begin{bmatrix} a_1 & b_1 \\ a_2 & b_2 \end{bmatrix} \begin{bmatrix} c_1 \\ c_2 \end{bmatrix} \rightarrow \begin{bmatrix} a_2 & b_2 \\ a_1 & b_1 \end{bmatrix} \begin{bmatrix} c_2 \\ c_1 \end{bmatrix}$ 

$$x \begin{bmatrix} a'_1 \\ a'_2 \end{bmatrix} + y \begin{bmatrix} b'_1 \\ b'_2 \end{bmatrix} = x \begin{bmatrix} a_2 \\ a_1 \end{bmatrix} + y \begin{bmatrix} b_2 \\ b_1 \end{bmatrix} = \begin{bmatrix} xa_2 + yb_2 \\ xa_1 + yb_1 \end{bmatrix} = \begin{bmatrix} c_2 \\ c_1 \end{bmatrix} = \begin{bmatrix} c'_1 \\ c'_2 \end{bmatrix}$$

(B)  $r_2 \times k : \begin{bmatrix} a_1 & b_1 \\ a_2 & b_2 \end{bmatrix} \begin{bmatrix} c_1 \\ c_2 \end{bmatrix} \rightarrow \begin{bmatrix} a_1 & b_1 \\ ka_2 & kb_2 \end{bmatrix} \begin{bmatrix} c_1 \\ kc_2 \end{bmatrix}$  (他も同様)

$$x \begin{bmatrix} a'_1 \\ a'_2 \end{bmatrix} + y \begin{bmatrix} b'_1 \\ b'_2 \end{bmatrix} = x \begin{bmatrix} a_1 \\ ka_2 \end{bmatrix} + y \begin{bmatrix} b_1 \\ kb_2 \end{bmatrix} = \begin{bmatrix} xa_1 + yb_1 \\ k(xa_2 + yb_2) \end{bmatrix} = \begin{bmatrix} c_1 \\ kc_2 \end{bmatrix} = \begin{bmatrix} c'_1 \\ c'_2 \end{bmatrix}$$

(C)  $r_2 + kr_1 : \begin{bmatrix} a_1 & b_1 \\ a_2 & b_2 \end{bmatrix} \begin{bmatrix} c_1 \\ c_2 \end{bmatrix} \rightarrow \begin{bmatrix} a_1 & b_1 \\ a_2 + ka_1 & b_2 + kb_1 \end{bmatrix} \begin{bmatrix} c_1 \\ kc_1 \end{bmatrix}$  (他も同様)

$$x \begin{bmatrix} a'_1 \\ a'_2 \end{bmatrix} + y \begin{bmatrix} b'_1 \\ b'_2 \end{bmatrix} = x \begin{bmatrix} a_1 \\ a_2 + ka_1 \end{bmatrix} + y \begin{bmatrix} b_1 \\ b_2 + kb_1 \end{bmatrix} = \begin{bmatrix} xa_1 + yb_1 \\ xa_2 + yb_2 + k(xa_1 + yb_1) \end{bmatrix} = \begin{bmatrix} c_1 \\ c_2 + kc_1 \end{bmatrix} = \begin{bmatrix} c'_1 \\ c'_2 \end{bmatrix}$$

以上により題意は示された。 ■

<span id="page-71-0"></span>**【4-8】 付録 4 : 行列式の定義について**

本講での行列式の定義が、線形代数の教科書によく載っているいわゆる行列式に対するライプニッツの明示公式

$$\begin{vmatrix} a_{11} & \dots & a_{1n} \\ \vdots & \ddots & \vdots \\ a_{n1} & \dots & a_{nn} \end{vmatrix} \equiv \sum_{\sigma \in S_n} \text{sgn}(\sigma) a_{1,\sigma(1)} \cdots a_{n,\sigma(n)}$$

( $S_n$  は  $n$  次対称群、 $\text{sgn}(\sigma)$  は置換  $\sigma$  の符号を表す)

と同等であることを、3次を例として解説する。まず置換  $\sigma$  とは何かをごく簡単に説明する。

前講の[3-7-2] 拡張 Levi-Civita 記号の説明で、「 $(1,2,3)$ の数字の並びの順列は、 $3!=6$  通りあり、 $(1,2,3)$ から2つの数字の入れ替えである互換の組み合わせで変換するとき、偶数回の互換で到達できる場合を偶置換、奇数回の互換で到達できる場合を奇置換といい、この偶奇性は互換のやり方によらない。」という話をした。この「置換」は本来以下のよう定式化される。

 $(1,2,3)$  を  $(3,2,1)$  に変換する置換  $\sigma$  を  $\sigma = \begin{pmatrix} 1 & 2 & 3 \\ 3 & 2 & 1 \end{pmatrix}$  と書く。この場合、1 と 3 の互換 1 回で変換ができるのでこの置換  $\sigma$  は奇置換となる。またこの置換  $\sigma$  を各要素に注目して 1 が 3 に、2 が 2 に、3 が 1 に変換されることを  $\sigma(1) = 3$ ,  $\sigma(2) = 2$ ,  $\sigma(3) = 1$  と表記する。

この $(1,2,3)$ の置換の集合は3次の対称群  $S_3$  とよばれ、その要素は3の順列の数と等しく6つある。 $S_3$  の元である6通りの置換を全て書き下すと、

$$\text{偶置換} : \begin{pmatrix} 1 & 2 & 3 \\ 1 & 2 & 3 \end{pmatrix}, \begin{pmatrix} 1 & 2 & 3 \\ 2 & 3 & 1 \end{pmatrix}, \begin{pmatrix} 1 & 2 & 3 \\ 3 & 1 & 2 \end{pmatrix} \quad \text{奇置換} : \begin{pmatrix} 1 & 2 & 3 \\ 1 & 3 & 2 \end{pmatrix}, \begin{pmatrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{pmatrix}, \begin{pmatrix} 1 & 2 & 3 \\ 3 & 2 & 1 \end{pmatrix}$$

となり、符号を表す  $\text{sgn}(\sigma)$  は 置換  $\sigma$  が偶置換の場合は +1、奇置換の場合は -1 を表す。

以上を用いて3次の行列式のライプニッツの明示公式は「3次の全ての置換に対してその置換の符号付きで、行列の各行から置換に対応した列の要素を選んで積を作ったものの総和を取る」という手続きにより行列式を求める事となる。具体的には、

$$\begin{aligned} & \sum_{\sigma \in S_3} \text{sgn}(\sigma) a_{1,\sigma(1)} a_{2,\sigma(2)} a_{3,\sigma(3)} \\ &= \text{sgn} \begin{pmatrix} 1 & 2 & 3 \\ 1 & 2 & 3 \end{pmatrix} a_{1,\sigma(1)} a_{2,\sigma(2)} a_{3,\sigma(3)} + \text{sgn} \begin{pmatrix} 1 & 2 & 3 \\ 2 & 3 & 1 \end{pmatrix} a_{1,\sigma(1)} a_{2,\sigma(2)} a_{3,\sigma(3)} \\ &+ \text{sgn} \begin{pmatrix} 1 & 2 & 3 \\ 3 & 1 & 2 \end{pmatrix} a_{1,\sigma(1)} a_{2,\sigma(2)} a_{3,\sigma(3)} + \text{sgn} \begin{pmatrix} 1 & 2 & 3 \\ 1 & 3 & 2 \end{pmatrix} a_{1,\sigma(1)} a_{2,\sigma(2)} a_{3,\sigma(3)} \\ &+ \text{sgn} \begin{pmatrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{pmatrix} a_{1,\sigma(1)} a_{2,\sigma(2)} a_{3,\sigma(3)} + \text{sgn} \begin{pmatrix} 1 & 2 & 3 \\ 3 & 2 & 1 \end{pmatrix} a_{1,\sigma(1)} a_{2,\sigma(2)} a_{3,\sigma(3)} \\ &= a_{11} a_{22} a_{33} + a_{12} a_{23} a_{31} + a_{13} a_{21} a_{32} - a_{11} a_{23} a_{32} - a_{12} a_{21} a_{33} - a_{13} a_{22} a_{31} \end{aligned}$$

本講での定義では行列の要素は列番号を1からnに固定し、行番号を動かして総和を取る形式だった。付録1で示したように、行列式は行と列の性質が同等であるため両者は一致する。

## 【第 5 講】 行列 II : 線形変換

<span id="page-72-1"></span><span id="page-72-0"></span>

### 【5-1】 はじめに

前講では連立一次方程式をテーマとしてきた。一次方程式  $ax = b$  の見かたを変えて  $y = ax$  として 1 次関数と見ることができたように、行列形式で書かれた連立一次方程式  $Ax = b$  を  $y = Ax$  として みてみると、これはベクトル  $x$  で表された点が行列  $A$  で別のベクトル  $y$  で示される点に写されるものだと考えることができる。本講ではこの視点で行列や行列式、ベクトルがもつ性質を掘り下げていこう。最後に線形写像という一段高い位置から俯瞰することで理解を深め、次講に繋げていく。

<span id="page-72-2"></span>

### 【5-2】 線形変換（一次変換）

#### 【5-2-1】 線形変換の例

式  $y = Ax$  のようにベクトル  $x$  を行列  $A$  によってベクトル  $y$  に写す（対応させる）ことを線形変換（一次変換）という。例として下記の 2 次の行列  $A$  で考えてみる。

$$A = \begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix}$$

この行列による変換は、

$$\begin{bmatrix} y_1 \\ y_2 \end{bmatrix} = \begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \end{bmatrix} \quad \text{あるいは} \begin{cases} y_1 = a_{11}x_1 + a_{12}x_2 \\ y_2 = a_{21}x_1 + a_{22}x_2 \end{cases} \quad (5-2-1)$$

という変換（まさに一次変換）となる。この式は、座標値  $(x_1, x_2)$  の点が  $(a_{11}x_1 + a_{12}x_2, a_{21}x_1 + a_{22}x_2)$  に写されることを意味しているが、これを以下のようにとらえることもできる。

変換前の任意の点を表す位置ベクトル  $x = x_1e_1 + x_2e_2$  は

$$y = Ax = A(x_1e_1 + x_2e_2) = x_1Ae_1 + x_2Ae_2 = x_1e'_1 + x_2e'_2 \quad (5-2-2)$$

と写されるとみることができる。これは標準基底  $e_1 = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, e_2 = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$  が別の基底  $e'_1, e'_2$  に

$$e'_1 = Ae_1 : \begin{bmatrix} a_{11} \\ a_{21} \end{bmatrix} = \begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix} \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \quad e'_2 = Ae_2 : \begin{bmatrix} a_{12} \\ a_{22} \end{bmatrix} = \begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix} \begin{bmatrix} 0 \\ 1 \end{bmatrix} \quad (5-2-3)$$

として写され（対応させられ）、このとき写された基底を元の標準基底で表すと

$$\begin{bmatrix} a_{11} \\ a_{21} \end{bmatrix} = a_{11} \begin{bmatrix} 1 \\ 0 \end{bmatrix} + a_{21} \begin{bmatrix} 0 \\ 1 \end{bmatrix}, \begin{bmatrix} a_{12} \\ a_{22} \end{bmatrix} = a_{12} \begin{bmatrix} 1 \\ 0 \end{bmatrix} + a_{22} \begin{bmatrix} 0 \\ 1 \end{bmatrix} \quad \text{or} \quad \begin{cases} e'_1 = a_{11}e_1 + a_{21}e_2 \\ e'_2 = a_{12}e_1 + a_{22}e_2 \end{cases} \quad (5-2-4)$$

となり、座標値の変換（5-2-1）式と異なる変換をしていると解釈できる。

この意味は後ほど述べる<sup>44</sup>こととして、(5-2-2) 式で変換された点は

$$\begin{bmatrix} y_1 \\ y_2 \end{bmatrix} = y = x_1e'_1 + x_2e'_2 = x_1 \begin{bmatrix} a_{11} \\ a_{21} \end{bmatrix} + x_2 \begin{bmatrix} a_{12} \\ a_{22} \end{bmatrix} = \begin{bmatrix} a_{11}x_1 + a_{12}x_2 \\ a_{21}x_1 + a_{22}x_2 \end{bmatrix}$$

となり、当然（5-2-1）式と一致する。

以上の話を具体的に 2 次の行列で可視化してみよう。例として以下の行列で考えてみる。

<sup>44</sup> 本講第 5 節にて。

$$A = \begin{bmatrix} 3/2 & 1/2 \\ 1/4 & 1 \end{bmatrix}$$

図は変換前の（灰色の）点線で描かれた直交座標系を張る標準基底  $e_1, e_2$  が（ピンク色の）鎖線で描かれた斜交座標系を張る基底  $e'_1, e'_2$  に

$$e'_1 = Ae_1 : \begin{bmatrix} 3/2 \\ 1/4 \end{bmatrix} = \begin{bmatrix} 3/2 & 1/2 \\ 1/4 & 1 \end{bmatrix} \begin{bmatrix} 1 \\ 0 \end{bmatrix}$$

$$e'_2 = Ae_2 : \begin{bmatrix} 1/2 \\ 1 \end{bmatrix} = \begin{bmatrix} 3/2 & 1/2 \\ 1/4 & 1 \end{bmatrix} \begin{bmatrix} 0 \\ 1 \end{bmatrix}$$

として写されたものを重ねて描いたものであり

変換前の任意の点  $x = x_1e_1 + x_2e_2$  は (5-2-2)式

$$y = Ax = A(x_1e_1 + x_2e_2) = x_1Ae_1 + x_2Ae_2 = x_1e'_1 + x_2e'_2$$

より直交座標のある座標値の点が、斜交座標での同じ座標値の点に写されることがわかる。このようすは、図で変換前の直交座標での正方形の各頂点(0,3),(1,3),(1,2),(0,2)が変換後の斜交座標での該当する各頂点に写されていることからもわかる。また原点を中心とした半径 1 の円が対応する斜交座標で原点から  $\pm 1$  の範囲内に写されていることもわかる。

![](_page_73_Figure_27.jpeg)

図 5-2-1

線形変換の特徴として、まず写された後の基底  $e'_1, e'_2$  を列ベクトルとして並べたものが、線形変換の行列となっている事があげられる。高次でも同様となり、これの意味は第 5 節で詳しく述べる。

次に変換による面積の変化は、基底により張られる面積の変化によりわかるが、これはまさに我らが  $D(a, b, c, \dots)$  「関数」の出発点で行列式の値となり、高次でも成り立つ。この例では、 $|A| = \frac{3}{2} \times 1 - \frac{1}{4} \times \frac{1}{2} = \frac{11}{8} = 1.375$  となり、変換前の標準基底が張る面積 1 に対して、1.375 倍となり、四角形や円の面積も 1.375 倍となる。

![](_page_73_Figure_31.jpeg)

図 5-2-2

図 5-2-2 は行列が  $\begin{bmatrix} 1.2 & 0 \\ 0 & 0.8 \end{bmatrix}$  の例で、行列式の値は 0.96 となる。縦 0.8 倍、横 1.2 倍のスケール変換となっていることがわかる。

図 5-2-3 は行列が  $\begin{bmatrix} 1 & 0.8 \\ 0 & 1 \end{bmatrix}$  の例で、行列式の値は 1 となる。 $\begin{bmatrix} 1 & k \\ 0 & 1 \end{bmatrix}$  の形の変換は剪断（せんだん : shear）と呼ばれ面積を保つ変形を表すものとして知られる。

![](_page_73_Figure_35.jpeg)

図 5-2-3

図 5-2-4 は行列が  $\begin{bmatrix} \cos(\pi/3) & -\sin(\pi/3) \\ \sin(\pi/3) & \cos(\pi/3) \end{bmatrix}$  の例で、原点を中心とした角度  $\pi/3$  の回転を表し、行列式の値は 1 となる。4 節で詳しくみることになる。

図 5-2-5, 図 5-2-6 は行列が

$$\begin{bmatrix} 1 & 0.8 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} \cos(\pi/3) & -\sin(\pi/3) \\ \sin(\pi/3) & \cos(\pi/3) \end{bmatrix} \begin{bmatrix} \cos(\pi/3) & -\sin(\pi/3) \\ \sin(\pi/3) & \cos(\pi/3) \end{bmatrix} \begin{bmatrix} 1 & 0.8 \\ 0 & 1 \end{bmatrix}$$

の例で、「回転」「せん断」の合成変換を表している。このように線形変換を連続して行う場合、対応する行列の積が合成した変換を表すことになるが行列の積は非可換なのでその結果も一般的には異なる。この違いも 5 節で詳しく述べる。

図 5-2-7 は行列式が 0 となる例で、行列が

 $\begin{bmatrix} 1 & -1 \\ -1 & 1 \end{bmatrix}$  のときを示している。写された基底は  $\begin{bmatrix} 1 \\ -1 \end{bmatrix}, \begin{bmatrix} -1 \\ 1 \end{bmatrix}$  となり真逆を向いて線形従属となり、平面上の点は全て直線上に写されていること（つまり面積は 0）が見て取れる。変換は

$$\begin{bmatrix} y_1 \\ y_2 \end{bmatrix} = \begin{bmatrix} 1 & -1 \\ -1 & 1 \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \end{bmatrix} = \begin{bmatrix} x_1 - x_2 \\ -x_1 + x_2 \end{bmatrix}$$

となり、直線  $x_2 = x_1 + a$  上の点は全て点  $(-a, a)$  上に、特に直線  $x_1 = x_2$  上の点は全て原点に写されることになる。

![](_page_74_Figure_28.jpeg)

図 5-2-4

![](_page_74_Figure_30.jpeg)

図 5-2-5

![](_page_74_Figure_32.jpeg)

図 5-2-6

前講の最後に行列の逆数に相当する行列を掃き出し法で求めた。これは線形変換では逆変換に当たるのではないか？また上記の行列式が 0 で、ある直線上の点が全て同じ点に写されるような場合には逆変換は存在しなさそうだが、それと行列式が 0 とは繋がっているのではないか？

ここらで課題となっていた行列の逆数にあたる行列について調べてみよう。

![](_page_74_Figure_36.jpeg)

図 5-2-7

<span id="page-75-0"></span>**【5-3】 逆行列**

**[5-3-1] 行列式の性質 II : 余因子展開と積の行列式**

行列の逆数にあたる逆行列を求める上でまず必要となる行列式の性質をみてみよう。

3 次を例として行列式に対し以下のことを考えてみる。 $D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3)$  は  $\mathbf{a}_1 = \sum_{i=1}^3 a_{i1} e_i$  より

$$D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3) = a_{11}D(\mathbf{e}_1, \mathbf{a}_2, \mathbf{a}_3) + a_{21}D(\mathbf{e}_2, \mathbf{a}_2, \mathbf{a}_3) + a_{31}D(\mathbf{e}_3, \mathbf{a}_2, \mathbf{a}_3)$$

として 1 列目で展開できる。行列式の表記では

$$\begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} = a_{11} \begin{bmatrix} 1 & a_{12} & a_{13} \\ 0 & a_{22} & a_{23} \\ 0 & a_{32} & a_{33} \end{bmatrix} + a_{21} \begin{bmatrix} 0 & a_{12} & a_{13} \\ 1 & a_{22} & a_{23} \\ 0 & a_{32} & a_{33} \end{bmatrix} + a_{31} \begin{bmatrix} 0 & a_{12} & a_{13} \\ 0 & a_{22} & a_{23} \\ 1 & a_{32} & a_{33} \end{bmatrix}$$

となるが、右辺第 1 項は行列式の次数下げ(4-3-15)式を 3 次に適用すると以下のようになる。

$$a_{11} \begin{bmatrix} 1 & a_{12} & a_{13} \\ 0 & a_{22} & a_{23} \\ 0 & a_{32} & a_{33} \end{bmatrix} = a_{11} \begin{bmatrix} a_{22} & a_{23} \\ a_{32} & a_{33} \end{bmatrix}$$

ここで第 2 項は 1 度、第 3 項は 2 度、行を入れ換えて 1 行目に持っていけば

$$\begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} = a_{11} \begin{bmatrix} 1 & a_{12} & a_{13} \\ 0 & a_{22} & a_{23} \\ 0 & a_{32} & a_{33} \end{bmatrix} - a_{21} \begin{bmatrix} 1 & a_{22} & a_{23} \\ 0 & a_{12} & a_{13} \\ 0 & a_{32} & a_{33} \end{bmatrix} + a_{31} \begin{bmatrix} 1 & a_{32} & a_{33} \\ 0 & a_{12} & a_{13} \\ 0 & a_{22} & a_{23} \end{bmatrix}$$

と書ける（入れ換え時の符号の反転に注意）ので、行列式の次数下げを同様に適用すると

$$= a_{11} \begin{bmatrix} a_{22} & a_{23} \\ a_{32} & a_{33} \end{bmatrix} - a_{21} \begin{bmatrix} a_{12} & a_{13} \\ a_{32} & a_{33} \end{bmatrix} + a_{31} \begin{bmatrix} a_{12} & a_{13} \\ a_{22} & a_{23} \end{bmatrix}$$

と書けることになる。

この 2 次の行列式の部分は、それぞれ以下のように

$$\begin{bmatrix} (a_{11}) & \dots & \dots \\ \vdots & a_{22} & a_{23} \\ \vdots & a_{32} & a_{33} \end{bmatrix}, \quad \begin{bmatrix} \vdots & a_{12} & a_{13} \\ (a_{21}) & \dots & \dots \\ \vdots & a_{32} & a_{33} \end{bmatrix}, \quad \begin{bmatrix} \vdots & a_{12} & a_{13} \\ \vdots & a_{22} & a_{23} \\ (a_{31}) & \dots & \dots \end{bmatrix}$$

 $a_{11}, a_{21}, a_{31}$  のそれぞれの行と列の成分を除いた残りを詰めた形になっていることがわかる。

このような成分  $a_{ij}$  の行と列の成分を除いて詰めた行列を小行列、その行列式を**小行列式**といい

 $M_{ij}$  と表す事が多い。上記の例ではそれぞれ  $M_{11}, M_{21}, M_{31}$  となる。

同様に 2 列目でも展開できる。 $\mathbf{a}_2 = \sum_{i=1}^3 a_{i2} e_i$  より展開し行列式で表すと

$$D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3) = a_{12}D(\mathbf{a}_1, \mathbf{e}_1, \mathbf{a}_3) + a_{22}D(\mathbf{a}_1, \mathbf{e}_2, \mathbf{a}_3) + a_{32}D(\mathbf{a}_1, \mathbf{e}_3, \mathbf{a}_3)$$

$$\begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} = a_{12} \begin{bmatrix} a_{11} & 1 & a_{13} \\ a_{21} & 0 & a_{23} \\ a_{31} & 0 & a_{33} \end{bmatrix} + a_{22} \begin{bmatrix} a_{11} & 0 & a_{13} \\ a_{21} & 1 & a_{23} \\ a_{31} & 0 & a_{33} \end{bmatrix} + a_{32} \begin{bmatrix} a_{11} & 0 & a_{13} \\ a_{21} & 0 & a_{23} \\ a_{31} & 1 & a_{33} \end{bmatrix}$$

となり、それぞれ 1 列目と入れ換えて

$$= -a_{12} \begin{bmatrix} 1 & a_{11} & a_{13} \\ 0 & a_{21} & a_{23} \\ 0 & a_{31} & a_{33} \end{bmatrix} - a_{22} \begin{bmatrix} 0 & a_{11} & a_{13} \\ 1 & a_{21} & a_{23} \\ 0 & a_{31} & a_{33} \end{bmatrix} - a_{32} \begin{bmatrix} 0 & a_{11} & a_{13} \\ 0 & a_{21} & a_{23} \\ 1 & a_{31} & a_{33} \end{bmatrix}$$

さらに 1 列目のときと同様に第 2 項は 1 度の、第 3 項は 2 度の入れ換えで 1 行目に移して

$$= -a_{12} \begin{bmatrix} 1 & a_{11} & a_{13} \\ 0 & a_{21} & a_{23} \\ 0 & a_{31} & a_{33} \end{bmatrix} + a_{22} \begin{bmatrix} 1 & a_{21} & a_{23} \\ 0 & a_{11} & a_{13} \\ 0 & a_{31} & a_{33} \end{bmatrix} - a_{32} \begin{bmatrix} 1 & a_{31} & a_{33} \\ 0 & a_{11} & a_{13} \\ 0 & a_{21} & a_{23} \end{bmatrix}$$

$$= -a_{12} \begin{bmatrix} a_{21} & a_{23} \\ a_{31} & a_{33} \end{bmatrix} + a_{22} \begin{bmatrix} a_{11} & a_{13} \\ a_{31} & a_{33} \end{bmatrix} - a_{32} \begin{bmatrix} a_{11} & a_{13} \\ a_{21} & a_{23} \end{bmatrix}$$

$$M_{12} : \begin{vmatrix} \cdots & (a_{12}) & \cdots \\ a_{21} & \vdots & a_{23} \\ a_{31} & \vdots & a_{33} \end{vmatrix}, \quad M_{22} : \begin{vmatrix} a_{11} & \vdots & a_{13} \\ \cdots & (a_{22}) & \cdots \\ a_{31} & \vdots & a_{33} \end{vmatrix}, \quad M_{32} : \begin{vmatrix} a_{11} & \vdots & a_{13} \\ a_{21} & \vdots & a_{23} \\ \cdots & (a_{32}) & \cdots \end{vmatrix}$$

また展開の際につく符号は、入れ換えの回数より  $(-1)^{i+j}$  と書けることがわかる (確認しよう)。

この入れ換えによる符号  $(-1)^{i+j}$  を小行列の行列式  $M_{ij}$  に付けた  $(-1)^{i+j}M_{ij}$  を成分  $a_{ij}$  の**余因子**といい、 $\tilde{a}_{ij}$  (あるいは  $C_{ij}$ ) と書かれることが多い。

同様に 3 列目の展開は

$$\begin{aligned} D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3) &= a_{13}D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{e}_1) + a_{23}D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{e}_2) + a_{33}D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{e}_3) \\ \begin{vmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{vmatrix} &= a_{13} \begin{vmatrix} a_{11} & a_{12} & 1 \\ a_{21} & a_{22} & 0 \\ a_{31} & a_{32} & 0 \end{vmatrix} + a_{23} \begin{vmatrix} a_{11} & a_{12} & 0 \\ a_{21} & a_{22} & 1 \\ a_{31} & a_{32} & 0 \end{vmatrix} + a_{33} \begin{vmatrix} a_{11} & a_{12} & 0 \\ a_{21} & a_{22} & 0 \\ a_{31} & a_{32} & 1 \end{vmatrix} \\ &= (-1)^{1+3} a_{13} \begin{vmatrix} a_{21} & a_{22} \\ a_{31} & a_{32} \end{vmatrix} + (-1)^{2+3} a_{23} \begin{vmatrix} a_{11} & a_{12} \\ a_{31} & a_{32} \end{vmatrix} + (-1)^{3+3} a_{33} \begin{vmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{vmatrix} \end{aligned}$$

となり、小行列式・余因子で表すと以下のように書ける。

$$\begin{aligned} &= (-1)^{1+3} a_{13} M_{13} + (-1)^{2+3} a_{23} M_{23} + (-1)^{3+3} a_{33} M_{33} \\ &= a_{13} \tilde{a}_{13} + a_{23} \tilde{a}_{23} + a_{33} \tilde{a}_{33} \end{aligned}$$

元の展開式と比較すれば、余因子  $\tilde{a}_{ij}$  とは  $j$  列目が標準基底の  $i$  番目  $\mathbf{e}_i$  となる  $D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3)$  の ことでもあり、同じことだが  $j$  列目が標準基底の  $i$  番目となる行列式のことでもある。

これまでの話はそのまま  $n$  次へ拡張されることもわかる。このような展開を**余因子展開**という。

● (xi) 列に対する余因子展開 ( $j$  列目による展開)

$$\begin{vmatrix} a_{11} & \cdots & a_{1n} \\ \vdots & \ddots & \vdots \\ a_{n1} & \cdots & a_{nn} \end{vmatrix} = \sum_{i=1}^n (-1)^{i+j} a_{ij} M_{ij} = \sum_{i=1}^n a_{ij} \tilde{a}_{ij} \quad (5-3-1)$$

行列式は列に対して成り立つ性質は行に対しても成り立つ。余因子展開は以下のようになる。

● (xii) 行に対する余因子展開 ( $i$  行目による展開)

$$\begin{vmatrix} a_{11} & \cdots & a_{1n} \\ \vdots & \ddots & \vdots \\ a_{n1} & \cdots & a_{nn} \end{vmatrix} = \sum_{j=1}^n (-1)^{i+j} a_{ij} M_{ij} = \sum_{j=1}^n a_{ij} \tilde{a}_{ij} \quad (5-3-2)$$

同様に余因子  $\tilde{a}_{ij}$  は  $i$  行目が標準基底の  $j$  番目となる行列式でもあることになる (次項も参照)。

● (xiii) 正方行列  $A, B$  の積の行列式は、それぞれの行列式の積

$$|AB| = |A| |B| \quad (5-3-3)$$

証明は前講 付録 1 参照。なお証明をたどれば  $|A| = 0$  or  $|B| = 0$  のときも成り立つことに注意。

### [5-3-2] 逆行列の定義と余因子行列による表示

前講の最後に考えた行列  $A$  の逆数にあたる行列は  $AX' = E$  を満たすもので、もしこれが  $X'A = E$  でもあれば  $Ax = b$  の両辺に左から  $X'$  を掛けることで  $x = X'b$  を得て実際に解を得た結果に結びつくのだった。また線形変換  $\mathbf{y} = Ax$  も同様に左から  $X'$  を掛けることで  $x = X'\mathbf{y}$  と書けることになり逆変換となりそうだ。これらを踏まえ、逆行列を以下のように定義しよう。

●逆行列と正則行列の定義

正方行列  $A$  に対して行列  $X$  が  $AX = XA = E$  を満たすとき、  
 $X$  を  $A$  の逆行列であるといい  $A^{-1}$  と表記する。逆行列を持つ行列を**正則行列**という。  
 (定義から  $A$  は  $A^{-1}$  の逆行列でもあることに注意)

3次を例として、それぞれ  $AX = E, YA = E$  を満たす  $X, Y$  を考えてみよう。  
 まず以下の式を満たす行列  $X$  を求める。

$$AX = E, \quad \begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} \begin{bmatrix} x_{11} & x_{12} & x_{13} \\ x_{21} & x_{22} & x_{23} \\ x_{31} & x_{32} & x_{33} \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$$

前講の最後にやったように、行列  $A, X, E$  を列ベクトルが並んだものとみなし

$$\mathbf{a}_1 = \begin{bmatrix} a_{11} \\ a_{21} \\ a_{31} \end{bmatrix}, \mathbf{a}_2 = \begin{bmatrix} a_{12} \\ a_{22} \\ a_{32} \end{bmatrix}, \mathbf{a}_3 = \begin{bmatrix} a_{13} \\ a_{23} \\ a_{33} \end{bmatrix}, \mathbf{x}_1 = \begin{bmatrix} x_{11} \\ x_{21} \\ x_{31} \end{bmatrix}, \mathbf{x}_2 = \begin{bmatrix} x_{12} \\ x_{22} \\ x_{32} \end{bmatrix}, \mathbf{x}_3 = \begin{bmatrix} x_{13} \\ x_{23} \\ x_{33} \end{bmatrix}, \mathbf{e}_1 = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}, \mathbf{e}_2 = \begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix}, \mathbf{e}_3 = \begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}$$

を導入すれば、以下の3つの連立一次方程式となり

$$A\mathbf{x}_1 = \mathbf{e}_1, \quad A\mathbf{x}_2 = \mathbf{e}_2, \quad A\mathbf{x}_3 = \mathbf{e}_3$$

さらにそれぞれを前講[4-2-4]でやったように列ベクトル  $\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3$  の線形結合の形に書き直すと

$$\begin{aligned} x_{11}\mathbf{a}_1 + x_{21}\mathbf{a}_2 + x_{31}\mathbf{a}_3 &= \mathbf{e}_1 \\ x_{12}\mathbf{a}_1 + x_{22}\mathbf{a}_2 + x_{32}\mathbf{a}_3 &= \mathbf{e}_2 \\ x_{13}\mathbf{a}_1 + x_{23}\mathbf{a}_2 + x_{33}\mathbf{a}_3 &= \mathbf{e}_3 \end{aligned}$$

と書けて、これを一つにまとめると以下の式になる。

$$x_{1j}\mathbf{a}_1 + x_{2j}\mathbf{a}_2 + x_{3j}\mathbf{a}_3 = \mathbf{e}_j$$

クラメルの法則でみたように、これを  $D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3)$  の  $\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3$  にそれぞれ代入すれば

$$\begin{aligned} D(\mathbf{e}_j, \mathbf{a}_2, \mathbf{a}_3) &= x_{1j}D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3) = x_{1j}|A| \\ D(\mathbf{a}_1, \mathbf{e}_j, \mathbf{a}_3) &= x_{2j}D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3) = x_{2j}|A| \\ D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{e}_j) &= x_{3j}D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3) = x_{3j}|A| \end{aligned}$$

とそれぞれ  $x_{1j}, x_{2j}, x_{3j}$  の項が残る。一方左辺は前項でみたように

$$D(\mathbf{e}_j, \mathbf{a}_2, \mathbf{a}_3) = \tilde{a}_{j1}, \quad D(\mathbf{a}_1, \mathbf{e}_j, \mathbf{a}_3) = \tilde{a}_{j2}, \quad D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{e}_j) = \tilde{a}_{j3}$$

として余因子となり結果  $\tilde{a}_{ji} = x_{ij}|A|$  と書ける。添字の順番が両辺で逆になっていることに注意。

ここで余因子を成分とする行列の転置行列として以下のように**余因子行列**を定義する。

$$\tilde{A} \equiv \begin{bmatrix} \tilde{a}_{11} & \tilde{a}_{21} & \tilde{a}_{31} \\ \tilde{a}_{12} & \tilde{a}_{22} & \tilde{a}_{32} \\ \tilde{a}_{13} & \tilde{a}_{23} & \tilde{a}_{33} \end{bmatrix} \quad (\text{転置しないものを余因子行列と定義する場合もあるので注意})$$

余因子行列  $\tilde{A}$  を用いて、行列  $A$  の行列式  $|A| \neq 0$  のとき  $X = \frac{1}{|A|}\tilde{A}$  と求まる。

次に以下の式を満たす行列  $Y$  を求める ( $AX = E$  のときとほぼ同様となる)。

$$YA = E, \quad \begin{bmatrix} y_{11} & y_{12} & y_{13} \\ y_{21} & y_{22} & y_{23} \\ y_{31} & y_{32} & y_{33} \end{bmatrix} \begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$$

行列  $Y, A, E$  を行ベクトルが並んだものとみなし、

$$\begin{aligned} \mathbf{y}_1^\top &= [y_{11} \ y_{12} \ y_{13}], & \mathbf{y}_2^\top &= [y_{21} \ y_{22} \ y_{23}], & \mathbf{y}_3^\top &= [y_{31} \ y_{32} \ y_{33}] \\ \mathbf{a}_1^\top &= [a_{11} \ a_{12} \ a_{13}], & \mathbf{a}_2^\top &= [a_{21} \ a_{22} \ a_{23}], & \mathbf{a}_3^\top &= [a_{31} \ a_{32} \ a_{33}] \\ \mathbf{e}_1^\top &= [1 \ 0 \ 0], & \mathbf{e}_2^\top &= [0 \ 1 \ 0], & \mathbf{e}_3^\top &= [0 \ 0 \ 1] \end{aligned}$$

を導入すれば、以下の 3 つの連立一次方程式となり、

$$\mathbf{y}_1^\top A = \mathbf{e}_1^\top, \quad \mathbf{y}_2^\top A = \mathbf{e}_2^\top, \quad \mathbf{y}_3^\top A = \mathbf{e}_3^\top$$

それぞれを行ベクトル  $\mathbf{a}_1^\top, \mathbf{a}_2^\top, \mathbf{a}_3^\top$  の線形結合の形に書き直すと

$$\begin{aligned} y_{11}[a_{11} \quad a_{12} \quad a_{13}] + y_{12}[a_{21} \quad a_{22} \quad a_{23}] + y_{13}[a_{31} \quad a_{32} \quad a_{33}] &= [1 \quad 0 \quad 0], & y_{11}\mathbf{a}_1^\top + y_{12}\mathbf{a}_2^\top + y_{13}\mathbf{a}_3^\top &= \mathbf{e}_1^\top \\ y_{21}[a_{11} \quad a_{12} \quad a_{13}] + y_{22}[a_{21} \quad a_{22} \quad a_{23}] + y_{23}[a_{31} \quad a_{32} \quad a_{33}] &= [0 \quad 1 \quad 0], & y_{21}\mathbf{a}_1^\top + y_{22}\mathbf{a}_2^\top + y_{23}\mathbf{a}_3^\top &= \mathbf{e}_2^\top \\ y_{31}[a_{11} \quad a_{12} \quad a_{13}] + y_{32}[a_{21} \quad a_{22} \quad a_{23}] + y_{33}[a_{31} \quad a_{32} \quad a_{33}] &= [0 \quad 0 \quad 1], & y_{31}\mathbf{a}_1^\top + y_{32}\mathbf{a}_2^\top + y_{33}\mathbf{a}_3^\top &= \mathbf{e}_3^\top \end{aligned}$$
と書けて、これを一つにまとめると以下の式になる。

$$y_{i1}\mathbf{a}_1^\top + y_{i2}\mathbf{a}_2^\top + y_{i3}\mathbf{a}_3^\top = \mathbf{e}_i^\top$$

これを  $D(\mathbf{a}_1^\top, \mathbf{a}_2^\top, \mathbf{a}_3^\top)$  の  $\mathbf{a}_1^\top, \mathbf{a}_2^\top, \mathbf{a}_3^\top$  にそれぞれ代入すれば<sup>45</sup>、それぞれ  $y_{i1}, y_{i2}, y_{i3}$  の項が残り

$$D(\mathbf{e}_i^\top, \mathbf{a}_2^\top, \mathbf{a}_3^\top) = y_{i1}D(\mathbf{a}_1^\top, \mathbf{a}_2^\top, \mathbf{a}_3^\top) = y_{i1}|A|$$

$$D(\mathbf{a}_1^\top, \mathbf{e}_i^\top, \mathbf{a}_3^\top) = y_{i2}D(\mathbf{a}_1^\top, \mathbf{a}_2^\top, \mathbf{a}_3^\top) = y_{i2}|A|$$

$$D(\mathbf{a}_1^\top, \mathbf{a}_2^\top, \mathbf{e}_i^\top) = y_{i3}D(\mathbf{a}_1^\top, \mathbf{a}_2^\top, \mathbf{a}_3^\top) = y_{i3}|A|$$

となる。また左辺を行列式で表せば、例として以下のようになり余因子となることがわかる。

$$D(\mathbf{e}_3^\top, \mathbf{a}_2^\top, \mathbf{a}_3^\top) = \begin{vmatrix} 0 & 0 & 1 \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{vmatrix} = \tilde{a}_{13}, \quad D(\mathbf{e}_i^\top, \mathbf{a}_2^\top, \mathbf{a}_3^\top) = \tilde{a}_{1i}$$

$$D(\mathbf{a}_1^\top, \mathbf{e}_1^\top, \mathbf{a}_3^\top) = \begin{vmatrix} a_{11} & a_{12} & a_{13} \\ 1 & 0 & 0 \\ a_{31} & a_{32} & a_{33} \end{vmatrix} = \tilde{a}_{21}, \quad D(\mathbf{a}_1^\top, \mathbf{e}_i^\top, \mathbf{a}_3^\top) = \tilde{a}_{2i}$$

$$D(\mathbf{a}_1^\top, \mathbf{a}_2^\top, \mathbf{e}_2^\top) = \begin{vmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ 0 & 1 & 0 \end{vmatrix} = \tilde{a}_{32}, \quad D(\mathbf{a}_1^\top, \mathbf{a}_2^\top, \mathbf{e}_i^\top) = \tilde{a}_{3i}$$

左辺を余因子として結果  $\tilde{a}_{ji} = y_{ij}|A|$  と書ける。添字の順番が両辺で逆になっていることに注意。

余因子行列を用いて、行列  $A$  の行列式  $|A| \neq 0$  のとき  $Y = \frac{1}{|A|}\tilde{A}$  と求まる。

3 次を例とした以上の議論は、より高次にも全く同様に適用され  $n$  次の正方行列  $A$  に対し

 $AX = E, YA = E$  を満たす  $X, Y$  は、 $|A| \neq 0$  のとき  $X = Y = \frac{1}{|A|}\tilde{A}$  となり逆行列の定義を満たす。

$$A^{-1} = \frac{1}{|A|}\tilde{A} \quad (|A| \neq 0) \quad (5-3-4)$$

これは逆行列の余因子行列による表示となる。次項でこの逆行列の性質を調べよう。

### [5-3-3] 正則行列/逆行列の性質

(i) 逆行列は一意 : 正則な行列がもつ逆行列は一意に定まる (5-3-5)

 $AX = XA = E, AY = YA = E$  を満たす任意の  $X, Y$  に対し  $AY = E$  の両辺に左から  $X$  を掛けると  $XAY = X$  となるが  $XA = E$  より  $EY = X$  したがって  $Y = X$  がいえて、題意は示された。 ■

(ii)  $|A^{-1}| = 1/|A|$  : (正則行列の) 逆行列の行列式は行列式の逆数となる (5-3-6)

 $A^{-1}A = E$  の両辺の行列式は  $1 = |E| = |A^{-1}A| = |A^{-1}||A|$  となり  $\therefore |A^{-1}| = 1/|A|$  ■

<sup>45</sup>  $D(\mathbf{a}, \mathbf{b}, \mathbf{c})$  のベクトルは列ベクトルと限られているわけではなく、行ベクトルとみなしても良い。そもそも  $D(\mathbf{a}, \mathbf{b}, \mathbf{c})$  自体には行や列の概念はなく、列をベクトルとみなして定義した場合の行も、列と同じ性質を持つ (逆もしかり) という関係にあること (第 4 講 付録 1 参照) に注意。

(iii)  $(AB)^{-1} = B^{-1}A^{-1}$  : 正則行列の積も正則で、積の逆行列は逆行列の逆順の積 (5-3-7)

 $AB$  に  $B^{-1}A^{-1}$  を掛ける。左側から :  $(B^{-1}A^{-1})(AB) = B^{-1}(A^{-1}A)B = B^{-1}B = E$ 

右側から :  $(AB)(B^{-1}A^{-1}) = A(BB^{-1})A^{-1} = AA^{-1} = E$  となり、題意を満たす。 ■

(iv) 正方行列  $A$  に対し  $AX = E$  または  $XA = E \Rightarrow X = A^{-1}$  (5-3-8)

 $AX = E$  の両辺の行列式を求めると、 $1 = |E| = |AX| = |A||X|$  となり  $|A| \neq 0$  がいえて、

 $A^{-1}A = AA^{-1} = E$  となる  $A^{-1} = \frac{1}{|A|}\tilde{A}$  が求まる。 $AX = E$  の両辺に左側から  $A^{-1}$  を掛けると、

 $A^{-1}AX = A^{-1} \Rightarrow X = A^{-1}$  となる。 $XA = E$  の場合も同様。よって題意は示された。 ■

• 性質(i)により、 $Ax = b$  に対し  $|A| \neq 0$  のとき  $x = A^{-1}b$  として得る解の一意性がいえる。

• 性質(iv)により、前講の最後に掃き出し法で求めた方法でも逆行列が求まることがわかった。

●  $n$  次正方行列  $A$  に対して以下の条件は全て同値となる (5-3-9)

(i)  $A$  は正則行列である

(ii) 行列式  $|A| \neq 0$ 

(iii)  $Ax = 0$  が自明な解のみをもつ

(iv)  $A$  を列ベクトルの組とみなしたとき、その組は線形独立である

(iv')  $A$  を行ベクトルの組とみなしたとき、その組は線形独立である

(v)  $\text{rank}(A) = n$ 

【証明】

• (i)  $\Rightarrow$  (ii) :

 $A^{-1}A = E$  の両辺の行列式  $1 = |E| = |A^{-1}A| = |A^{-1}||A|$  より  $|A| \neq 0$  がいえる。

• (ii)  $\Rightarrow$  (iii) :

 $|A| \neq 0$  より  $A^{-1}$  となる  $\frac{1}{|A|}\tilde{A}$  が求まり  $Ax = 0$  の両辺に左から掛け一意な解  $x = 0$  を得る。

• (iii)  $\Rightarrow$  (iv) :

 $A$  を列ベクトルの組  $[a_1 \cdots a_n]$  とみなすと  $Ax = 0$  は  $x_1a_1 + \cdots + x_na_n = 0$  と書けるが、自明な解のみなので  $x_1 = \cdots = x_n = 0$  のみとなり、列ベクトルの組  $a_1, \dots, a_n$  は線形独立となる。

• (iv)  $\Rightarrow$  (v) :

前講[4-2-4]の考察でみたように行基本変形は線形結合関係を保ち、簡約行列となっても列は線形独立なままとなる。このとき行 0 ベクトルが生じると、掃き出せない列が生じてその列は主成分をもつ他の列ベクトルの組の線形結合で表されることになり線形従属となって矛盾する。よって行 0 ベクトルは生じず、結果主成分は  $n$  個存在することになり  $\text{rank}(A)$  は  $n$  となる。

• (v)  $\Rightarrow$  (i) :

 $\text{rank}$  が  $n$  なので 行列  $A$  に対して掃き出し法で  $AX = E$  を満たす  $X$  が求まり、(5-3-8)より  $X$  は逆行列  $A^{-1}$  であることがいえ  $A$  は正則行列といえる。

以上により (i), (ii), (iii), (iv), (v) は全て同値であることが示された<sup>46</sup>。

最後に (ii)  $\Leftrightarrow$  (iv') を示す。(ii)  $\Leftrightarrow$  (iii) と  $|A^T| = |A|$  より「(iii')  $A^T \mathbf{x} = \mathbf{0}$  or  $\mathbf{x}^T A = \mathbf{0}$  が自明解のみをもつ」に対し (ii)  $\Leftrightarrow$  (iii') となり、また (iii)  $\Rightarrow$  (iv) と同様に (iii')  $\Rightarrow$  (iv') がいえ、逆にたどれば (iv')  $\Rightarrow$  (iii') もいえるので (iii')  $\Leftrightarrow$  (iv') がいえる。よって (ii)  $\Leftrightarrow$  (iv') が成り立つ。

以上により題意は示された。 ■

- • 上記において (iv)  $\Leftrightarrow$  (ii) より前講 (4-3-12) の行列式の性質(vi')が示された。
- • (iv), (iv')  $\Leftrightarrow$  (ii), (v) より[4-2-4]項で考察した係数行列の行・列ベクトルが線形独立であることと行列式が非零であることとの同値性、また求まる解の一意性も示された。

蛇足ながらクラメルの法則で解いた解と逆行列を用いて解いた解との関係を確認しておこう。

3次を例として連立一次方程式  $\sum_{j=1}^3 a_{ij} x_j = b_i$  or  $x_1 \mathbf{a}_1 + x_2 \mathbf{a}_2 + x_3 \mathbf{a}_3 = \mathbf{b}$  において、  
 $D(\mathbf{b}, \mathbf{a}_2, \mathbf{a}_3) = x_1 |A|$ ,  $D(\mathbf{a}_1, \mathbf{b}, \mathbf{a}_3) = x_2 |A|$ ,  $D(\mathbf{a}_1, \mathbf{a}_2, \mathbf{b}) = x_3 |A|$  の各左辺を  $D(\sum_{j=1}^3 b_j \mathbf{e}_j, \mathbf{a}_2, \mathbf{a}_3) = \sum_{j=1}^3 b_j D(\mathbf{e}_j, \mathbf{a}_2, \mathbf{a}_3) = \sum_{j=1}^3 b_j \tilde{a}_{j1}$  のように余因子で表すことでまとめて  $\sum_{j=1}^3 b_j \tilde{a}_{ji} = x_i |A|$  と書け、これは  $|A| \neq 0$  のとき  $x_i = \frac{1}{|A|} \sum_{j=1}^3 \tilde{a}_{ij}^T b_j$  あるいは  $\mathbf{x} = A^{-1} \mathbf{b}$  と逆行列を用いた解となる。

線形変換  $\mathbf{y} = A\mathbf{x}$  において、行列  $A$  が正則である場合すなわち  $|A| \neq 0$  のときは逆行列  $A^{-1}$  を両辺の左側から掛けることにより  $\mathbf{x} = A^{-1} \mathbf{y}$  なる逆変換が求まることがわかった。さらに詳しいことは第 5 節で述べるとして、次節では重要な線形変換である回転を表す行列を調べよう。

<span id="page-80-0"></span>

## 【5-4】 直交行列

### 【5-4-1】 転置行列の性質

直交行列を議論する前に関係の深い転置行列の性質を簡単にみておこう。

#### ● 転置行列の性質

(i)  $(AB)^T = B^T A^T$  : 積の転置行列は順序を逆にした転置行列の積 (5 - 4 - 1)

$$\{(AB)^T\}_{ij} = (AB)_{ji} = \sum_k a_{jk} b_{ki} = \sum_k b_{ik}^T a_{kj}^T = (B^T A^T)_{ij} \quad \therefore (AB)^T = B^T A^T \quad \blacksquare$$

(ii)  $(A^T)^{-1} = (A^{-1})^T$  : 正則行列の転置行列の逆行列は逆行列の転置行列 (5 - 4 - 2)

$$A^{-1} A = A A^{-1} = E \text{ の両辺の転置をとると } E = E^T = (A^{-1} A)^T = A^T (A^{-1})^T \text{ また } E = E^T =$$

$$(A A^{-1})^T = (A^{-1})^T A^T \text{ となり、これは } (A^{-1})^T \text{ が } A^T \text{ の逆行列となることを示している。} \quad \blacksquare$$

---

<sup>46</sup> (ii)  $\Rightarrow$  (iii)  $\Rightarrow$  (iv)  $\Rightarrow$  (v) より (ii)  $\Rightarrow$  (i) がいえて (i)  $\Rightarrow$  (ii) でもあるので (i) と(ii)は同値。同様に (iii)  $\Rightarrow$  (ii) がいえて (ii)  $\Rightarrow$  (iii) でもあるので (ii) と(iii) も同値となり、さらに同様にして (iii) と(iv)、(iv) と(v) の同値もいえるので (i), (ii), (iii), (iv), (v) は全て同値となる。

●内積の表示

列ベクトル  $x = \begin{bmatrix} x_1 \\ \vdots \\ x_n \end{bmatrix}, y = \begin{bmatrix} y_1 \\ \vdots \\ y_n \end{bmatrix}$  の標準内積を  $x \cdot y \equiv x^T y = [x_1 \quad \cdots \quad x_n] \begin{bmatrix} y_1 \\ \vdots \\ y_n \end{bmatrix} = x_1 y_1 + \cdots + x_n y_n$  として定義する。

**[5-4-2] 直交行列の定義と性質**

●直交行列の定義

 $R^T R = R R^T = E$  を満たす正方行列  $R$  を直交行列という。

●直交行列の性質

(i) 直交行列は正則行列であり、 $R$  の逆行列は  $R^T$  (定義より明らか) (5 - 4 - 3)

(ii) 行列式は  $|R| = \pm 1$  (5 - 4 - 4)

 $R^T R = E$  の両辺の行列式を求めると、 $|R^T| = |R|, |E| = 1$  より  $|R|^2 = 1 \quad \therefore |R| = \pm 1$  ■

(iii)  $R_1, R_2$  が直交行列のとき、その積もまた直交行列 (5 - 4 - 5)

 $(R_1 R_2)^T (R_1 R_2) = R_2^T R_1^T R_1 R_2 = R_2^T R_2 = E, (R_1 R_2)(R_1 R_2)^T = R_1 R_2 R_2^T R_1^T = R_1 R_1^T = E$  ■

(iv) 正方行列  $R$  において  $R^T R = E$  または  $R R^T = E \Rightarrow R$  は直行列である (5 - 4 - 6)

(5-3-8)から  $R^T R = E$  のとき  $R^T = R^{-1}$  がいえ  $R R^T = E$  も成り立つので  $R$  は直交行列といえる。 $R R^T = E$  のときも同様。よって題意は示された ■

●  $n$  次正方行列  $R$  に対して以下の条件は全て同値となる (5 - 4 - 7)

(i)  $R$  は直交行列である

(ii)  $R$  による線形変換が内積を不変に保つ ( $\forall x, y \in \mathbb{R}^n, (Rx) \cdot (Ry) = x \cdot y$ )

(iii)  $R$  による線形変換がノルムを不変に保つ ( $\forall x \in \mathbb{R}^n, \|Rx\| = \|x\|$ )

(iv)  $R$  を列ベクトルの組とみなしたとき、その組は正規直交基底をなす

(iv')  $R$  を行ベクトルの組とみなしたとき、その組は正規直交基底をなす

【証明】

• (i)  $\Rightarrow$  (ii) :

 $(Rx) \cdot (Ry) = (Rx)^T (Ry) = (x^T R^T) (Ry) = x^T (R^T R) y = x^T y = x \cdot y$  よって内積は不変となる。

• (ii)  $\Rightarrow$  (iii) :

• (iii)  $\Rightarrow$  (iv) :

 $R = [r_1 \cdots r_n]$  のとき標準基底  $e_i$  に対して  $Re_i = r_i$  より  $\|r_i\| = \|Re_i\| = \|e_i\| = 1$  がいえ、また  $R(e_i + e_j) = r_i + r_j$  より  $i \neq j$  のとき  $\|r_i + r_j\| = \|R(e_i + e_j)\| = \|e_i + e_j\| = \sqrt{2}$  となり両辺を 2 乗して  $\|r_i\|^2 + \|r_j\|^2 + 2r_i \cdot r_j = 2$  より  $r_i \cdot r_j = 0$  がいえて、 $r_i \cdot r_j = \delta_{ij}$  を得る。

• (iv)  $\Rightarrow$  (i) :

$$R^T R = \begin{bmatrix} r_1^T \\ \vdots \\ r_n^T \end{bmatrix} [r_1 \cdots r_n] = \begin{bmatrix} r_1^T r_1 & \cdots & r_1^T r_n \\ \vdots & \ddots & \vdots \\ r_n^T r_1 & \cdots & r_n^T r_n \end{bmatrix} = \begin{bmatrix} r_1 \cdot r_1 & \cdots & r_1 \cdot r_n \\ \vdots & \ddots & \vdots \\ r_n \cdot r_1 & \cdots & r_n \cdot r_n \end{bmatrix} = E \text{ がいえて、}$$

性質(iv) : (5-4-6) より  $R$  は直交行列となる。

• (i)  $\Leftrightarrow$  (iv') : ( $R$  の  $i$  行目の行ベクトルをここでは  $\tilde{r}_i$  と書くとする)

$$RR^T = \begin{bmatrix} \tilde{r}_1 \\ \vdots \\ \tilde{r}_n \end{bmatrix} [\tilde{r}_1^T \cdots \tilde{r}_n^T] = \begin{bmatrix} \tilde{r}_1 \tilde{r}_1^T & \cdots & \tilde{r}_1 \tilde{r}_n^T \\ \vdots & \ddots & \vdots \\ \tilde{r}_n \tilde{r}_1^T & \cdots & \tilde{r}_n \tilde{r}_n^T \end{bmatrix} = \begin{bmatrix} \tilde{r}_1 \cdot \tilde{r}_1 & \cdots & \tilde{r}_1 \cdot \tilde{r}_n \\ \vdots & \ddots & \vdots \\ \tilde{r}_n \cdot \tilde{r}_1 & \cdots & \tilde{r}_n \cdot \tilde{r}_n \end{bmatrix} \text{ よって ((5-4-6) より)}$$

 $R$  は直交行列であることと行ベクトルの組が正規直交基底とは同値となる。

以上により (i), (ii), (iii), (iv), (iv') は同値であることが示された。 ■

直交行列による変換 (直交変換) は (5-4-7)よりベクトルのノルム・内積が不変な (大きさ・角度を保つ) 変換となる。このような変換を**等長変換**という (厳密には原点を原点に写す等長変換)。

例として 2 次の直交行列で見てみよう (3 次は第 7 講 回転の表現 I にて詳しくみる)。任意の正規直交基底を  $e'_1, e'_2$  とし、これを列ベクトルとする行列  $[e'_1 \quad e'_2]$  は上記条件(iv)より直交行列となる。標準基底を  $e_1, e_2$  とし、図のように  $e_1, e'_1$  のなす角を  $\theta$  とすると、 $e'_1 = \begin{bmatrix} \cos \theta \\ \sin \theta \end{bmatrix}$  となる。 $e'_2$  は  $e'_1$  と直交するが向き付けにより 2 通りとることができる。

![](_page_82_Figure_31.jpeg)

図の  $e'_2(R) = \begin{bmatrix} -\sin \theta \\ \cos \theta \end{bmatrix}$  は  $e'_1$  とともに右手系の座標系を張り、直交行列は  $\begin{bmatrix} \cos \theta & -\sin \theta \\ \sin \theta & \cos \theta \end{bmatrix}$  となり 2 次元の**回転**を表し、行列式は+1 となる。 $e'_2(L) = \begin{bmatrix} \sin \theta \\ -\cos \theta \end{bmatrix}$  は  $e'_1$  とともに左手系の座標系を張り、直交行列は  $\begin{bmatrix} \cos \theta & \sin \theta \\ \sin \theta & -\cos \theta \end{bmatrix}$  となる。これは  $e_1$  を軸とした反射を表す直交行列  $\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$  と回転を表す直交行列との積 :  $\begin{bmatrix} \cos \theta & -\sin \theta \\ \sin \theta & \cos \theta \end{bmatrix} \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$  と解釈でき、2 次元の**鏡映** : 座標軸反射と回転の合成を表すこととなり、行列式は -1 となる。

なお  $\theta = \pi/2$  の回転に相当する  $\begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}$  に関する面白い話があるので付録 2 で紹介する。

より高次でも行列式が+1 のとき直交行列は向き付けを変えない等長変換すなわち回転を表し、これを**回転行列**という。 $n$  次の直交行列の条件式  $R^T R = E$  の独立な式は  $n + (n^2 - n)/2$  個であり、直交行列の独立な成分の個数、すなわち回転の自由度は  $n^2$  からこれを引いて  $\frac{1}{2}n(n-1)$  となる。(反射等の変換は連続したパラメータを持たず、これを除いても変換の自由度は変わらない。)

<span id="page-83-0"></span>**【5-5】 線形変換の行列による表示**

**[5-5-1] この節のねらい**

本来のベクトルが基底の取り方に依らない概念だったのに対し  $n \times 1$  行列である列ベクトルはある基底（通常は標準基底）に対する成分としての表示であり、それ自体は基底に依存する表示であることに注意を要する。実は行列も同様であり、ここで改めて任意の基底に対する表示として定式化する。最初は「抽象的だ」「回りくどい」と思うかもしれないが、基底の変換や合成変換など、基底が絡む混乱しがちな話を理解しやすくなり、話が進むにつれその意義がわかってくると思う。

**[5-5-2] 必要な諸定義**

● 写像（関数の概念の一般化）

![](_page_83_Diagram_25.jpeg)

ある集合の全ての元それぞれをある集合の一意な元に対応させる規則のことを**写像**(mapping)という。集合  $U$  の元を集合  $V$  の元に写す写像を  $f$  とする（上図左）。これを  $f: U \rightarrow V$  と書き、また特に元  $x \in U$  が  $f(x) \in V$  に写されることを  $f: x \mapsto f(x)$  とも書く。関数と同様に  $f(x)$  は一意に定まり（つまり 1 対多の対応はダメ）任意の  $x \in U$  に対して  $f(x) \in V$  となること（つまり「定義域」は  $U$  全体、「値域」は  $V$  の一部でも可）に注意。写像が 1 対 1 で「値域」が  $V$  全体の場合（上図右）逆向きの写像が定まる。これを**逆写像**といい  $f^{-1}$  で表す。

![](_page_83_Diagram_27.jpeg)

● 合成写像

写像  $f: U \ni x \mapsto y = f(x) \in V, g: V \ni y \mapsto z = g(y) \in W$  に対し（上図）、 $U$  から  $W$  への写像  $h: U \ni x \mapsto z \in W$  を  $z = g(f(x))$  と定義し、これを  $h = g \circ f$  と書いて  $f, g$  の**合成写像**という。合成写像  $h = g \circ f$  の  $f, g$  がそれぞれ逆写像をもつとき（右図）その合成は  $h^{-1} = (g \circ f)^{-1} = f^{-1} \circ g^{-1}$  となることに注意。

![](_page_83_Diagram_30.jpeg)

● 線形写像

ベクトル空間  $U \rightarrow V$  への写像  $f$  (ベクトルをベクトルに写す写像) が  $\forall x, y \in U, \forall k \in \mathbb{R}$  に対し  $f(x + y) = f(x) + f(y), f(kx) = kf(x)$  (5 - 5 - 1) を満たすとき、この写像を**線形写像**という。定義より  $f(x)$  もベクトルである。特にベクトル空間  $U, V$  が同じベクトル空間である場合、この線形写像のことを**線形変換**ともいう。この線形写像（および線形変換）自体は、ベクトルと同様に基底の取り方に依らない概念であることに注意。

**[5-5-2] ベクトルの列ベクトルによる表示**

任意のベクトルは ある基底の線形結合として表すことができ、列ベクトルはこの係数の組を各成分として縦に並べて表したものであり、逆に列ベクトルの各成分による基底の線形結合の結果が元の（基底に依らない）ベクトルとなると考えることができる。このことを定式化してみよう。

 $n$  次元ベクトル空間  $U$  の任意の元であるベクトル  $x$  が、 $U$  の任意の基底  $B = \{b_i\}$  ( $b_i$  の集合)

の線形結合として  $x = \sum_{i=1}^n b_i x_i^B$  と表されているとき<sup>47</sup>、この係数  $x_i^B$  を用いて

ベクトル  $x$  の基底  $\{b_i\}$  に対する列ベクトル表示  $x_B = \begin{bmatrix} x_1^B \\ \vdots \\ x_n^B \end{bmatrix} \in \mathbb{R}^n$  を得る。

逆に基底  $\{b_i\}$  の各ベクトルを各成分にもつ「行ベクトル」( $b_1 \cdots b_n$ ) と列ベクトル  $x_B$  との積として以下のように基底の線形結合としてのベクトル  $x$  を得る。

$$x = (b_1 \cdots b_n) x_B = (b_1 \cdots b_n) \begin{bmatrix} x_1^B \\ \vdots \\ x_n^B \end{bmatrix} = \sum_{i=1}^n b_i x_i^B \in U \quad (5-5-2)$$

![](_page_84_Picture_27.jpeg)

(ここで  $x_i^B$  の右肩および  $x_B$  の右下の  $B$  は基底  $B$  に対する表示を示し、また「 $U$  上のベクトルを成分に持つ行ベクトル」として小括弧を用いている<sup>48</sup>。)

以上により列ベクトル  $x_B$  は  $U$  上のベクトル  $x$  の基底  $B = \{b_i\}$  に対する  $\mathbb{R}^n$  上での表示となる。

### [5-5-3] ベクトルの組の行列による表示

 $n$  次元ベクトル空間  $U$  の任意の  $n$  本のベクトル  $a_j$  ( $j = 1, 2, \dots, n$ ) の組の表示を考える。各  $a_j$  が  $U$  の任意の基底  $B = \{b_i\}$  の線形結合として  $a_j = \sum_{i=1}^n b_i a_{ij}^B$  と表されているとき、この係数  $a_{ij}^B$  を用いてベクトル  $a_j$ 

の基底  $\{b_i\}$  に対する列ベクトル表示  $a_j = (b_1 \cdots b_n) \begin{bmatrix} a_{1j}^B \\ \vdots \\ a_{nj}^B \end{bmatrix} = (b_1 \cdots b_n) a_{jB}$ 

を得る。この列ベクトル表示を横に並べることでベクトルの組  $\{a_j\}$  を各成分にもつ「行ベクトル」( $a_1 \cdots a_n$ ) (基底という意味ではない) として

$$(a_1 \cdots a_n) = (b_1 \cdots b_n) \begin{bmatrix} a_{11}^B & \cdots & a_{1n}^B \\ \vdots & \ddots & \vdots \\ a_{n1}^B & \cdots & a_{nn}^B \end{bmatrix} = (b_1 \cdots b_n) A_B \quad (5-5-3)$$

![](_page_84_Picture_35.jpeg)

と書けることになり、これはベクトルの組  $\{a_j\}$  の基底  $\{b_i\}$  に対する行列  $A_B$  による表示と解釈できる。このベクトルの組  $\{a_j\}$  の線形独立性と表示行列  $A_B$  の正則性には以下の関係がある。

- ● ベクトルの組  $\{a_j\}$  が線形独立  $\Leftrightarrow$  その表示行列  $A_B$  が正則  $(5-5-4)$
- $\{a_j\}$  の線形結合  $\sum_{j=1}^n c_j a_j = 0$  は  $a_j = \sum_{i=1}^n b_i a_{ij}^B$  より  $\sum_{i,j=1}^n b_i a_{ij}^B = 0$  と書け  $\{b_j\}$  は線形独立なので  $\sum_{j=1}^n a_{ij}^B c_j = 0$  すなわち  $A_B c = 0$  となり (5-3-9):(i)  $\Leftrightarrow$  (iii)((iv)ではない)より示された。■

なお本項の話で  $\{a_j\}$  を基底  $\{b_i\}$  自身とした場合を考えると基底  $\{b_i\}$  の基底  $\{b_i\}$  に対する表示行列は単位行列となり、表示された列ベクトルの組は常に  $\mathbb{R}^n$  の「標準基底」となることがわかる。

<sup>47</sup> 線形結合の係数である成分を基底であるベクトルの右に書くのには理由があり、すぐあとでわかる

<sup>48</sup> これらの表記法は特に一般的なものではない。また本節以外で特に必要でない場合は省略される。

**[5-5-4] 線形変換の行列による表示**

 $n$  次元ベクトル空間  $U$  の任意の元  $x$  がある線形変換  $f: U \rightarrow U$  で

$$\mathbf{y} = f(x) \quad (5-5-5)$$

に写されるとする。ベクトル  $x, \mathbf{y}$  を  $U$  の任意の基底  $B = \{\mathbf{b}_i\}$  に対する列ベクトルで表示すると

$$\mathbf{x} = (\mathbf{b}_1 \cdots \mathbf{b}_n) \mathbf{x}_B, \quad \mathbf{y} = (\mathbf{b}_1 \cdots \mathbf{b}_n) \mathbf{y}_B \quad (5-5-6)$$

となり、(5-5-6)式を (5-5-5)式に代入して以下のようになる。

$$(\mathbf{b}_1 \cdots \mathbf{b}_n) \mathbf{y}_B = f(\sum_{i=1}^n \mathbf{b}_i x_i^B) = \sum_{i=1}^n f(\mathbf{b}_i) x_i^B = (f(\mathbf{b}_1) \cdots f(\mathbf{b}_n)) \mathbf{x}_B \quad (5-5-7)$$

 $n$  本のベクトルの組である  $f(\mathbf{b}_j)$  は基底  $\{\mathbf{b}_i\}$  に対する行列で表示でき

$$f(\mathbf{b}_j) = \sum_{i=1}^n \mathbf{b}_i a_{ij}^B \quad \text{or} \quad (f(\mathbf{b}_1) \cdots f(\mathbf{b}_n)) = (\mathbf{b}_1 \cdots \mathbf{b}_n) A_B \quad (5-5-8)$$

これを (5-5-7)式に代入して  $(\mathbf{b}_1 \cdots \mathbf{b}_n) \mathbf{y}_B = (\mathbf{b}_1 \cdots \mathbf{b}_n) A_B \mathbf{x}_B$  となり、

基底  $\{\mathbf{b}_i\}$  は線形独立なので以下を得る。

$$\mathbf{y}_B = A_B \mathbf{x}_B \quad \text{or} \quad y_i^B = \sum_{j=1}^n a_{ij}^B x_j^B \quad (5-5-9)$$

以上により行列  $A_B$  は  $U$  上の線形変換  $f$  の基底  $B = \{\mathbf{b}_i\}$  に対する

 $\mathbb{R}^{n \times n}$  上での表示と解釈できる。またこのことはベクトル空間の公理を

満たすベクトル空間の元が線形変換 (写像) されるとき、どんなもの

でも行列 (および列ベクトル) で表示できることを意味する。

![](_page_85_Diagram_42.jpeg)

例として本講第 2 節での線形変換  $\mathbf{y} = Ax$  について考察しよう。この  $\mathbf{y} = Ax$  は、あるベクトル空間  $U$  の標準基底  $E = \{\mathbf{e}_i\}$  に対し表示された  $\mathbf{y}_E = A_E \mathbf{x}_E$  のことだと解釈でき、 $\mathbf{x}_E, \mathbf{y}_E$  として表示された  $U$  のベクトル  $x, \mathbf{y}$  は  $x = (\mathbf{e}_1 \cdots \mathbf{e}_n) \mathbf{x}_E, \mathbf{y} = (\mathbf{e}_1 \cdots \mathbf{e}_n) \mathbf{y}_E$  のことであり、また行列  $A_E$  として表示された線形変換  $f$  は

$$f(\mathbf{e}_j) = \sum_{i=1}^n \mathbf{e}_i a_{ij}^E = (\mathbf{e}_1 \cdots \mathbf{e}_n) \mathbf{a}_{jE} \quad \text{or} \quad (f(\mathbf{e}_1) \cdots f(\mathbf{e}_n)) = (\mathbf{e}_1 \cdots \mathbf{e}_n) A_E$$

を満たすものであると考えることができる。

実際、基底  $\mathbf{e}_j$  が写る先を  $\mathbf{e}'_j = f(\mathbf{e}_j)$  として  $\mathbf{e}'_j = \sum_{i=1}^n \mathbf{e}_i a_{ij}^E$  と書くと (5-5-9)式との違いが、基底を写す(5-2-4)式と座標値の変換 (5-2-1)式との違いに相当する。また(5-5-7)式に相当する

 $\mathbf{y} = (f(\mathbf{e}_1) \cdots f(\mathbf{e}_n)) \mathbf{x}_E = (\mathbf{e}'_1 \cdots \mathbf{e}'_n) \mathbf{x}_E$  は、変換先の点を表す  $\mathbf{y}$  は変換元の座標系での座標値 ( $\mathbf{x}_E$ ) を座標値とした  $\mathbf{e}'_j$  が張る座標系により示される点であることを示している。さらに行列の各列ベクトルが  $\mathbf{e}'_j$  の基底  $\{\mathbf{e}_j\}$  に対する表示になるということに相当している。

注意すべきは、基底が写る先  $\mathbf{e}'_j = f(\mathbf{e}_j)$  の組は必ずしも線形独立になるとは限らないという点であり、(5-5-4)より  $f(\mathbf{e}_j)$  の組の線形独立性と表示行列  $A_E$  の正則性が同値となる。基底が写る先が線形独立であれば、逆変換として元の基底をその線形結合で表すことができ、その表示が逆行列となる。式で書くと  $(\mathbf{e}'_1 \cdots \mathbf{e}'_n) = (\mathbf{e}_1 \cdots \mathbf{e}_n) A_E$  に対して逆に  $(\mathbf{e}_1 \cdots \mathbf{e}_n) = (\mathbf{e}'_1 \cdots \mathbf{e}'_n) C$  と表せて、これに先の式を代入すると  $(\mathbf{e}_1 \cdots \mathbf{e}_n) = (\mathbf{e}_1 \cdots \mathbf{e}_n) A_E C$  より  $A_E C = E$  つまり  $C = A_E^{-1}$  となる。

**[5-5-5] 基底の変換と座標変換**

に対する列ベクトル  $x_B, x_C$  として、それぞれ

$$x = (b_1 \cdots b_n)x_B = (c_1 \cdots c_n)x_C \quad (5-5-10)$$

と表されているとする。 $\{c_i\}$  は  $n$  本のベクトルの組なので (5-5-3) 式の

ように基底  $\{b_i\}$  に対する行列で表示することができ、

$$(c_1 \cdots c_n) = (b_1 \cdots b_n)P_{B \rightarrow C} \quad \text{or} \quad c_j = \sum_{i=1}^n b_i p_{ij}^{B \rightarrow C} \quad (5-5-11)$$

と書ける。この  $P_{B \rightarrow C}$  を**基底の変換行列**という。

これを (5-5-10)に代入して  $x_B = P_{B \rightarrow C}x_C$  となる。変換の向きが異なるこ

とに注意。基底はそれぞれ線形独立なので (5-5-4)より  $P_{B \rightarrow C}$  は正則

行列となり逆行列を用いて

$$x_C = P_{B \rightarrow C}^{-1}x_B \quad \text{or} \quad x_i^C = \sum_{j=1}^n p_{ij}^{-1}x_j^B \quad (5-5-12)$$

を得る。この式を基底の変換に伴う座標変換という。

例)  $(c_1 \ c_2) = (b_1 \ b_2) \begin{bmatrix} 2 & 1 \\ 1 & 1 \end{bmatrix}, \quad x = 3b_1 + 2b_2 : x_B = \begin{bmatrix} 3 \\ 2 \end{bmatrix}$ 

$$\rightarrow x_C = \begin{bmatrix} 2 & 1 \\ 1 & 1 \end{bmatrix}^{-1} \begin{bmatrix} 3 \\ 2 \end{bmatrix} = \begin{bmatrix} 1 & -1 \\ -1 & 2 \end{bmatrix} \begin{bmatrix} 3 \\ 2 \end{bmatrix} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$$

この座標変換を線形変換のときの座標値の変換(5-5-9)式と混同しない

よう注意。線形変換の方は  $U$  上のベクトル自体の変換を同じ基底に対

して表示した結果であるのに対し、座標変換は  $U$  上のある同じベクトルの異なる基底に対する

(異なる  $\mathbb{R}^n$  上での) 表示間の変換（つまり異なる座標系で同じモノを見た結果間の変換）という

根本的な違いがある。基底の変換により、ある同じベクトルの表示である列ベクトルが変換を受け

たように、ある同じ線形変換の表示行列も基底を変換すると変換される。詳しくみてみよう。

**[5-5-6] 線形変換に対する基底の変換と表示行列の変換**

 $n$  次元ベクトル空間  $U$  上のベクトルの線形変換  $f: x \mapsto y = f(x)$ 

の 2 組の基底  $B = \{b_i\}, C = \{c_i\}$  に対する表示行列を  $F_B, F_C$ 

基底の変換行列を  $(c_1 \cdots c_n) = (b_1 \cdots b_n)P_{B \rightarrow C}$  としたとき変換後の

ベクトル  $f(x)$  をそれぞれ表示する。基底と座標の変換を用いて

$$f(x) = (b_1 \cdots b_n)F_B x_B = (c_1 \cdots c_n)F_C x_C = (b_1 \cdots b_n)P_{B \rightarrow C} F_C x_C \\ = (b_1 \cdots b_n)P_{B \rightarrow C} F_C P_{B \rightarrow C}^{-1} x_B$$

と書けて、**表示行列の変換**  $F_B = P_{B \rightarrow C} F_C P_{B \rightarrow C}^{-1}$  あるいは

$$F_C = P_{B \rightarrow C}^{-1} F_B P_{B \rightarrow C} \quad (5-5-13)$$

を得る。この関係は図からも読み取れる。

![](_page_86_Diagram_63.jpeg)

![](_page_86_Diagram_64.jpeg)

![](_page_86_Diagram_65.jpeg)

基底すなわち座標系は対象の系に対し最も都合が良いものを選ぶことができ、この表示行列の変換式により行列が単純になる基底があれば応用上重要となる。これは次講のテーマの一つとなる。

また (5-5-13) 式で両辺の行列式を求めると、 $|F_C| = |P_{B \rightarrow C}^{-1} F_B P_{B \rightarrow C}| = |P_{B \rightarrow C}^{-1}| |F_B| |P_{B \rightarrow C}|$  となるが (5-3-6) より  $|P_{B \rightarrow C}^{-1}| = 1/|P_{B \rightarrow C}|$  がいえて、 $|F_C| = |F_B|$  となる。つまり行列式の値は基底の取り方に依らず、表示元である線形変換  $f$  に固有な量を表す重要な量であることがわかる。

**[5-5-7] 線形変換と座標変換 (Active と Passive)**

線形変換による座標値の変換と、基底の変換による座標変換の形式的な類似を利用して、線形変換の結果に相当する座標変換を考えよう。 [5-5-5] 項より座標変換の変換行列は基底の変換行列の逆行列となるので、変換先の基底は実現したい線形変換  $f$  の逆変換による変換先の組  $\{\mathbf{b}'_i = f^{-1}(\mathbf{b}_i)\}$  とする。そうすれば基底の変換行列は  $f$  の基底  $B$  に対する表示行列  $F_B$  の逆行列  $F_B^{-1}$  となり

$$(\mathbf{b}'_1 \cdots \mathbf{b}'_n) = (\mathbf{b}_1 \cdots \mathbf{b}_n) F_B^{-1} \quad (5-5-14)$$

と書け、このときの座標変換は

$$\mathbf{x}_{B'} = F_B \mathbf{x}_B \quad (5-5-15)$$

と書けることになる。線形変換が実際にベクトルを変換するため **Active** な変換、基底の変換に伴う座標変換ではベクトル自体は実際には変換されないため

**Passive** な変換と区別することがある。混同しないよ

![](_page_87_Diagram_41.jpeg)

![](_page_87_Figure_42.jpeg)

う改めて注意。例として左図の 2 次元の回転を考えよう。ベクトル  $\mathbf{x}$  の線形変換  $f$  による  $\mathbf{x}'$  への  $\frac{\pi}{2}$  回転を基底  $\{\mathbf{b}_1, \mathbf{b}_2\}$  で表示すれば

$$\mathbf{x}'_B = F_B \mathbf{x}_B: \begin{bmatrix} 1 \\ 1 \end{bmatrix} = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 1 \\ -1 \end{bmatrix} \text{ (Active) となる。これを線形変換 } f \text{ の逆変換}$$

$$f^{-1} \text{ による基底変換} (\mathbf{b}'_1 \ \mathbf{b}'_2) = (\mathbf{b}_1 \ \mathbf{b}_2) F_B^{-1} = (\mathbf{b}_1 \ \mathbf{b}_2) \begin{bmatrix} 0 & 1 \\ -1 & 0 \end{bmatrix} = (-\mathbf{b}_2 \ \mathbf{b}_1)$$

(この座標変換で表せば  $\mathbf{x}_{B'} = F_B \mathbf{x}_B: \begin{bmatrix} 1 \\ 1 \end{bmatrix} = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 1 \\ -1 \end{bmatrix}$  (Passive) となる。混同しないこと！

**[5-5-8] 合成変換の行列による表示**

 $n$  次元ベクトル空間  $U$  上のベクトルの線形変換  $f: \mathbf{x} \mapsto \mathbf{y} = f(\mathbf{x})$ ,  $g: \mathbf{y} \mapsto \mathbf{z} = g(\mathbf{y})$  の基底  $B = \{\mathbf{b}_i\}$  に対する行列表示が  $F_B, G_B$  のとき、合成変換  $h = g \circ f$  の表示行列  $H_B$  を  $F_B, G_B$  で表さう。 $g \circ f: \mathbf{x} \mapsto \mathbf{z} = g(f(\mathbf{x}))$  において  $(\mathbf{b}_1 \cdots \mathbf{b}_n) \mathbf{y}_B = (\mathbf{b}_1 \cdots \mathbf{b}_n) F_B \mathbf{x}_B$  より  $\mathbf{y}_B = F_B \mathbf{x}_B$  が言えて、これを  $(\mathbf{b}_1 \cdots \mathbf{b}_n) \mathbf{z}_B = (\mathbf{b}_1 \cdots \mathbf{b}_n) G_B \mathbf{y}_B$  に代入して  $(\mathbf{b}_1 \cdots \mathbf{b}_n) \mathbf{z}_B = (g \circ f)(\mathbf{x}) = (\mathbf{b}_1 \cdots \mathbf{b}_n) G_B F_B \mathbf{x}_B$  となり以下を得る。

$$\mathbf{z}_B = H_B \mathbf{x}_B, \quad H_B = G_B F_B \quad (5-5-16)$$

このように合成変換の同じ基底に対する表示行列は、各変換の表示行列の変換順での積となる。

![](_page_87_Diagram_51.jpeg)

このとき、合成される 2 回目以降の変換について注意が必要で、本講第 2 節の図 5-2-5 のように「回転」と続く「せん断」の合成変換の場合、せん断変換で平行にずらされる方向は回転しても変わらず横 ( $x_1$  軸) 方向のままになっている (実際に図を見て欲しい)。一方で「せん断」が先でその後「回転」の場合 (図 5-2-6) は、せん断で横方向にずらされた状態で全体が回転される。この後者の合成変換 (変換順が逆) の結果は、前者の合成変換でせん断のずらされる方向が回転後の軸とした場合とも解釈できるがこのことは偶然だろうか？ 2 回目以降の変換において、変換固有の向き (例えば 3 次元回転の回転軸なども考えられる) を 1 回目の変換に伴い変えさせたい場合はどう

すればよいのだろうか？ 実現したい変換は図のように 2 回目の変換  $g$  を 1 回目の変換  $f$  の逆変換後の基底として見た変換と考えることができるので、Passive 変換

![](_page_88_Diagram_28.jpeg)

により行うのが自然ともいえる。1 回目・2 回目の基底変換と伴う座標変換は

$$(\mathbf{b}'_1 \cdots \mathbf{b}'_n) = (\mathbf{b}_1 \cdots \mathbf{b}_n) F_B^{-1}, \mathbf{x}_{B'} = F_B \mathbf{x}_B \text{ と } (\mathbf{b}''_1 \cdots \mathbf{b}''_n) = (\mathbf{b}'_1 \cdots \mathbf{b}'_n) G_{B'}^{-1}, \mathbf{x}_{B''} = G_{B'} \mathbf{x}_{B'}$$

と書け、このときの  $G_{B'}$  は基底  $B'$  による表示すなわち 1 回目の基底変換に伴う行

列の変換であり (5-5-13)式で  $P_{B \rightarrow C} = F_B^{-1}$  にあたる  $G_{B'} = F_B G_B F_B^{-1}$  となる。これにより以下の合成変換を得る。

$$\mathbf{x}_{B''} = H_B \mathbf{x}_B, H_B = G_{B'} F_B \quad (G_{B'} = F_B G_B F_B^{-1}) \quad (5-5-17)$$

このとき基底の変換は実現したい座標変換の逆変換なので、その合成変換としては基底の逆変換の

合成  $h^{-1} = g^{-1} \circ f^{-1} = (f \circ g)^{-1}$  なる変換となり、相当する

線形変換(Active)は  $h = f \circ g$  と変換の順序が逆なので、その

表示行列は  $F_B G_B$  となることに注意を要する。このことは

(5-5-13)式にあたる行列の変換式  $G_{B'} = F_B G_B F_B^{-1}$  より

 $G_{B'} F_B = F_B G_B$  が言えることからもわかる。先に考察した線形

変換での回転とせん断の合成変換での変換順を逆にした結果と

解釈できた「からくり」が理解できただろうか。もっと具体例

等を知りたい人は 第 7 講 回転の表現 I 第 2・3 節で 3 次元の

回転にこの方法を応用するのでそちらも参照して頂きたい。

![](_page_88_Diagram_44.jpeg)

<span id="page-88-0"></span>**【5-6】 [▼C]付録 1 : Levi-Civita 記号の積の性質**

宿題となっていた第 3 講 (3-7-5) 式である  $\sum_{i=1}^3 \varepsilon_{ijk} \varepsilon_{imn} = \delta_{jm} \delta_{kn} - \delta_{jn} \delta_{km}$  の導出を行う。

3 次元の列ベクトルの組  $\mathbf{a}, \mathbf{b}, \mathbf{c}$  および  $\mathbf{x}, \mathbf{y}, \mathbf{z}$  が成す 3 次正方行列の行列式において、転置行列の行列式は元の行列式と等しいこと、行列の積の行列式は行列式の積に等しいことにより

$$\begin{bmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{bmatrix} \begin{bmatrix} x_1 & y_1 & z_1 \\ x_2 & y_2 & z_2 \\ x_3 & y_3 & z_3 \end{bmatrix} = \begin{bmatrix} a_1 & a_2 & a_3 \\ b_1 & b_2 & b_3 \\ c_1 & c_2 & c_3 \end{bmatrix} \begin{bmatrix} x_1 & y_1 & z_1 \\ x_2 & y_2 & z_2 \\ x_3 & y_3 & z_3 \end{bmatrix} = \begin{bmatrix} \mathbf{a} \cdot \mathbf{x} & \mathbf{a} \cdot \mathbf{y} & \mathbf{a} \cdot \mathbf{z} \\ \mathbf{b} \cdot \mathbf{x} & \mathbf{b} \cdot \mathbf{y} & \mathbf{b} \cdot \mathbf{z} \\ \mathbf{c} \cdot \mathbf{x} & \mathbf{c} \cdot \mathbf{y} & \mathbf{c} \cdot \mathbf{z} \end{bmatrix} \quad (5-6-1)$$

が成り立つ。ここで標準基底  $\{\mathbf{e}_i\}$  において  $D(\mathbf{e}_i, \mathbf{e}_j, \mathbf{e}_k) = \varepsilon_{ijk}$  と上式より、以下が成り立つ。

$$\varepsilon_{ijk} \varepsilon_{lmn} = D(\mathbf{e}_i, \mathbf{e}_j, \mathbf{e}_k) D(\mathbf{e}_l, \mathbf{e}_m, \mathbf{e}_n) = \begin{bmatrix} \mathbf{e}_i \cdot \mathbf{e}_l & \mathbf{e}_i \cdot \mathbf{e}_m & \mathbf{e}_i \cdot \mathbf{e}_n \\ \mathbf{e}_j \cdot \mathbf{e}_l & \mathbf{e}_j \cdot \mathbf{e}_m & \mathbf{e}_j \cdot \mathbf{e}_n \\ \mathbf{e}_k \cdot \mathbf{e}_l & \mathbf{e}_k \cdot \mathbf{e}_m & \mathbf{e}_k \cdot \mathbf{e}_n \end{bmatrix} = \begin{bmatrix} \delta_{il} & \delta_{im} & \delta_{in} \\ \delta_{jl} & \delta_{jm} & \delta_{jn} \\ \delta_{kl} & \delta_{km} & \delta_{kn} \end{bmatrix} \quad (5-6-2)$$

$$= \delta_{il} \delta_{jm} \delta_{kn} + \delta_{im} \delta_{jn} \delta_{kl} + \delta_{in} \delta_{jl} \delta_{km} - \delta_{il} \delta_{jn} \delta_{km} - \delta_{im} \delta_{jl} \delta_{kn} - \delta_{in} \delta_{jm} \delta_{kl} \quad (5-6-3)$$

(5-6-3)式において  $l = i$  として和をとると、以下のように求める式を得る。

$$\begin{aligned} \sum_{i=1}^3 \varepsilon_{ijk} \varepsilon_{imn} &= \sum_{i=1}^3 (\delta_{ii} \delta_{jm} \delta_{kn} + \delta_{im} \delta_{jn} \delta_{ki} + \delta_{in} \delta_{ji} \delta_{km} - \delta_{ii} \delta_{jn} \delta_{km} - \delta_{im} \delta_{ji} \delta_{kn} - \delta_{in} \delta_{jm} \delta_{ki}) \\ &= 3 \delta_{jm} \delta_{kn} + \delta_{jn} \delta_{km} + \delta_{jn} \delta_{km} - 3 \delta_{jn} \delta_{km} - \delta_{jm} \delta_{kn} - \delta_{jm} \delta_{kn} = \delta_{jm} \delta_{kn} - \delta_{jn} \delta_{km} \blacksquare \end{aligned}$$

なお、(5-6-2)式はその導き方により n 次においても同様に成り立つことがわかる。

$$\varepsilon_{i_1 \cdots i_n} \varepsilon_{j_1 \cdots j_n} = \begin{bmatrix} \delta_{i_1 j_1} & \cdots & \delta_{i_1 j_n} \\ \vdots & \ddots & \vdots \\ \delta_{i_n j_1} & \cdots & \delta_{i_n j_n} \end{bmatrix} \quad (5-6-4)$$

<span id="page-89-0"></span>**【5-7】 付録 2 : 複素数の行列による表現**

2次の回転行列  $\begin{bmatrix} \cos \theta & -\sin \theta \\ \sin \theta & \cos \theta \end{bmatrix}$  において  $\theta = \pi/2$  とした行列  $I = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}$  に対して、単位行列  $E$  との線形結合である行列  $Z = xE + yI$  ( $x, y \in \mathbb{R}$ ) を考えよう (以下登場人物は全員が実数)。

 $Z = \begin{bmatrix} x & -y \\ y & x \end{bmatrix}$  であり、 $Z = 0$  となるのは  $x = y = 0$  のときのみで  $E$  と  $I$  は線形独立となる。

$$Z_1 = x_1 E + y_1 I, \quad Z_2 = x_2 E + y_2 I$$

とすると、和は

$$Z_1 + Z_2 = (x_1 + x_2)E + (y_1 + y_2)I$$

となり、積は  $E^2 = E$ ,  $IE = I$ ,  $EI = I$ ,  $I^2 = \begin{bmatrix} -1 & 0 \\ 0 & -1 \end{bmatrix} = -E$  より

$$Z_1 Z_2 = (x_1 E + y_1 I)(x_2 E + y_2 I) = (x_1 x_2 - y_1 y_2)E + (x_1 y_2 + y_1 x_2)I = Z_2 Z_1$$

となる。また

$$E^T = E, I^T = -I \quad \text{および} \quad Z^T = \begin{bmatrix} x & y \\ -y & x \end{bmatrix} = xE^T + yI^T = xE - yI$$

となり、 $ZZ^T = (x^2 + y^2)E = Z^T Z$  となるので

$$\|Z\|^2 E = ZZ^T \quad (\|Z\| = \sqrt{x^2 + y^2})$$

として自然なノルム  $\|Z\|$  ( $\|Z\| = 0 \Leftrightarrow Z = 0$ ) が定義できる。よって  $Z \neq 0$  のとき

$$Z \left( \frac{1}{\|Z\|^2} Z^T \right) = \left( \frac{1}{\|Z\|^2} Z^T \right) Z = E$$

となり 逆元

$$Z^{-1} = \frac{1}{\|Z\|^2} Z^T$$

が定まる (実際、行列式  $|Z| = x^2 + y^2 = \|Z\|^2$ 、余因子行列  $\tilde{Z} = Z^T$  より確かに逆行列となる)。

また  $\cos \theta = \frac{x}{\sqrt{x^2 + y^2}}$ ,  $\sin \theta = \frac{y}{\sqrt{x^2 + y^2}}$  と書け、ノルムの定義から  $Z = \|Z\|(\cos \theta E + \sin \theta I) = \|Z\| \begin{bmatrix} \cos \theta & -\sin \theta \\ \sin \theta & \cos \theta \end{bmatrix}$  となり、大きさ 1 の  $Z$  を掛けることは  $\theta$  回転させることに相当する。  
(つまり  $Z$  はノルムで正規化すると回転行列となる)。

というわけで、対比表としてまとめると

|     | 基底/元                   | 共役                                   | 和                                         | 積                                               | ノルム                                                                                     | 逆元                                                 | 極形式                                        |
|-----|------------------------|--------------------------------------|-------------------------------------------|-------------------------------------------------|-----------------------------------------------------------------------------------------|----------------------------------------------------|--------------------------------------------|
| 複素数 | $1, i$<br>$z = x + iy$ | $\bar{i} = -i$<br>$\bar{z} = x - iy$ | $z_1 + z_2 = (x_1 + x_2) + i(y_1 + y_2)$  | $1^2 = 1$<br>$1i = i$<br>$i1 = i$<br>$i^2 = -1$ | $ z ^2 = z\bar{z}$<br>$ z  = \sqrt{x^2 + y^2}$<br>$( z  = 0 \Leftrightarrow z = 0)$     | $z^{-1} = \frac{1}{ z ^2} \bar{z}$<br>$(z \neq 0)$ | $z =  z (\cos \theta + i \sin \theta)$     |
| 行列  | $E, I$                 | $I^T = -I$                           | $Z_1 + Z_2 = (x_1 + x_2)E + (y_1 + y_2)I$ | $E^2 = E$<br>$EI = I$<br>$IE = I$<br>$I^2 = -E$ | $\ Z\ ^2 E = ZZ^T$<br>$\ Z\  = \sqrt{x^2 + y^2}$<br>$(\ Z\  = 0 \Leftrightarrow Z = 0)$ | $Z^{-1} = \frac{1}{\ Z\ ^2} Z^T$<br>$(Z \neq 0)$   | $Z = \ Z\ (\cos \theta E + \sin \theta I)$ |

表 5-6-1

つまり、 $Z = xE + yI$  は  $E, I$  を実数/虚数単位、転置を共役とみなすことで、複素数  $z = x + iy$  と同一視できることになる。おもしろいよね。(次講の付録で、もう一列追加されます・・・)
