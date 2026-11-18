(app-b)=
# B. Derivations and Approximations

<!-- Source PDF page 283; printed label 274. -->

(sec-B-1)=
## B.1 Derivation of Elliptical Orbits

Starting from the energy equation for a central force ([Chapter 10](#ch-10)), we have

$$
E = \frac{1}{2} m\dot{r}^{2}+ U_{eff}
$$

where $U_{eff}$ is the effective potential. Re-arranging the equation gives:

```{math}
:label: eq-b-1
:enumerator: B.1

\dot{r}^{2}= \frac{2}{m} (E - U_{eff})
```

where $\dot{r} = \frac{\mathrm{d}r}{\mathrm{d}t}$. We want to get $r(\theta)$ to describe the orbit. To do this, we will use the ratio of $\dot{r}$ and $\dot{\theta}$,

```{math}
:label: eq-b-2
:enumerator: B.2

\frac{\dot{r}}{\dot{\theta}} = \frac{\mathrm{d}r/\mathrm{d}t}{\mathrm{d}\theta /\mathrm{d}t} = \frac{\mathrm{d}r}{\mathrm{d}\theta}
```

So we need to get an equation for $\dot{\theta}$.

For $\dot{\theta}$, we can use the conservation of angular momentum. Recall that central forces conserve angular momentum by definition (see [Chapter 10](#ch-10)). The magnitude of angular momentum is:

```{math}
:label: eq-b-3
:enumerator: B.3

L = mr^{2}\dot{\theta} \quad\Rightarrow  \dot{\theta} = \frac{L}{mr^{2}}
```

with $L$ = constant.

We can then combine the $\dot{r}$ and $\dot{\theta}$ equations as follows:

$$
\Bigg(\frac{\mathrm{d}r}{\mathrm{d}\theta} \Bigg)^{2}= \frac{\dot{r}^{2}}{\dot{\theta}^{2}} \quad\Rightarrow  \text{from Equation B.2}
$$

$$
\Bigg(\frac{\mathrm{d}r}{\mathrm{d}\theta} \Bigg)^{2}= \frac{\frac{2}{m} (E - U_{eff})}{\Big(\frac{L}{mr^{2}} \Big)^{2}} \quad\Rightarrow  \text{sub in Equations B}.1 \text{and B}.3
$$

$$
\Bigg(\frac{\mathrm{d}r}{\mathrm{d}\theta} \Bigg)^{2}= \frac{2}{m} \frac{(E - U_{eff})}{L^{2}} (m^{2}r^{4})
$$

$$
\frac{1}{r^{4}} \Bigg(\frac{\mathrm{d}r}{\mathrm{d}\theta} \Bigg)^{2}= \frac{2m(E - U_{eff})}{L^{2}} \quad\Rightarrow  \text{bring all }r \text{terms to the other side}$$

<!-- Source PDF page 284; printed label 275. -->

```{math}
:label: eq-b-4
:enumerator: B.4

\Bigg(\frac{1}{r^{2}} \frac{\mathrm{d}r}{\mathrm{d}\theta} \Bigg)^{2}= \frac{2m(E - U_{eff})}{L^{2}} \quad\Rightarrow  \text{simplify the LHS of the equation}
```

Equation B.4 applies to any effective potential. Since we’re talking about orbits, the central force is gravity. That makes the effective potential:

```{math}
:label: eq-b-5
:enumerator: B.5

U_{eff}= \frac{L^{2}}{2mr^{2}} - \frac{\gamma}{r}
```

where $\gamma = GMm$ for simplicity. Substituting Equation B.5 into Equation B.4 gives,

$$
\Bigg(\frac{1}{r^{2}} \frac{\mathrm{d}r}{\mathrm{d}\theta} \Bigg)^{2}= \frac{2mE}{L^{2}} - \bigg(\frac{2m}{L^{2}} \bigg)\Bigg(\frac{L^{2}}{2mr^{2}} \Bigg) + \bigg(\frac{2m}{L^{2}} \bigg)\bigg(\frac{\gamma}{r} \bigg)
$$

```{math}
:label: eq-b-6
:enumerator: B.6

\Bigg(\frac{1}{r^{2}} \frac{\mathrm{d}r}{\mathrm{d}\theta} \Bigg)^{2}= \frac{2mE}{L^{2}} - \frac{1}{r^{2}} + \frac{2m\gamma}{rL^{2}} \quad\Rightarrow  \text{simplify}
```

To solve Equation B.6, there is a substitution trick we can use to help simplify the problem. Instead of solving for $r$, we’re going to solve for $y = \frac{1}{r}$. The reason for this substitution is that

$$
\frac{\mathrm{d}y}{\mathrm{d}\theta} = - \frac{1}{r^{2}} \frac{\mathrm{d}r}{\mathrm{d}\theta} \quad\Rightarrow  \text{remember that }y = \frac{1}{r}
$$

Thus, we can write Equation B.6 in terms of $y = \frac{1}{r}$ instead of $r$.

```{math}
:label: eq-b-7
:enumerator: B.7

\Bigg(\frac{\mathrm{d}y}{\mathrm{d}\theta} \Bigg)^{2}= \frac{2mE}{L^{2}} - y^{2}+ \frac{2m\gamma}{L^{2}} y \quad\Rightarrow  \text{sub} y = \frac{1}{r} \text{into Equations B}.6
```

Already this looks simpler. We can simplify more, however, by “completing the square”,

```{math}
:label: eq-b-8
:enumerator: B.8

-\bigg(y - \frac{m\gamma}{L^{2}} \bigg)^{2}= -y^{2}+ \frac{2m\gamma}{L^{2}} y - \bigg(\frac{m\gamma}{L^{2}} \bigg)^{2}
```

Note that the first two terms on the right-hand side of Equation B.8 are present on the right-hand side of Equation B.7. From Equation B.8, we can say that

```{math}
:label: eq-b-9
:enumerator: B.9

-y^{2}+ \frac{2m\gamma}{L^{2}} y = -\bigg(y - \frac{m\gamma}{L^{2}} \bigg)^{2}+ \bigg(\frac{m\gamma}{L^{2}} \bigg)^{2}
```

And we can substitute Equation B.9 into Equation B.7 to give:

```{math}
:label: eq-b-10
:enumerator: B.10

\Bigg(\frac{\mathrm{d}y}{\mathrm{d}\theta} \Bigg)^{2}= \frac{2mE}{L^{2}} - \bigg(y - \frac{m\gamma}{L^{2}} \bigg)^{2}+ \bigg(\frac{m\gamma}{L^{2}} \bigg)^{2}
```

With Equation B.10, we have an equation with one $y$ term and two constant terms. To make the equation a bit simpler, we will introduce a couple more substitutions for the constants.

<!-- Source PDF page 285; printed label 276. -->

First, we will use $z = y - \dfrac{m\gamma}{L^{2}}$. Note that $\dfrac{\mathrm{d}z}{\mathrm{d}\theta} = \dfrac{\mathrm{d}y}{\mathrm{d}\theta}$ because $\dfrac{m\gamma}{L^{2}}$ is a constant.

```{math}
:label: eq-b-11
:enumerator: B.11

\Bigg(\frac{\mathrm{d}z}{\mathrm{d}\theta} \Bigg)^{2}= -z^{2}+ \frac{2mE}{L^{2}} + \bigg(\frac{m\gamma}{L^{2}} \bigg)^{2}
```

Second, we will substitute for the sum of the remaining constants as $B^{2}$,

```{math}
:label: eq-b-12
:enumerator: B.12

\begin{aligned}
B^{2}&= \frac{2mE}{L^{2}} + \bigg(\frac{m\gamma}{L^{2}} \bigg)^{2} \\
B^{2}&= \bigg(\frac{m\gamma}{L^{2}} \bigg)^{2}\Bigg(\frac{2EL^{2}}{m\gamma ^{2}} + 1\Bigg)
\end{aligned}
```

```{math}
:label: eq-b-13
:enumerator: B.13

B = \frac{m\gamma}{L^{2}}\sqrt{1 + \frac{2EL^{2}}{m\gamma^{2}}}
```

Substituting Equation B.12 into Equation B.11, we get:

$$
\Bigg(\frac{\mathrm{d}z}{\mathrm{d}\theta} \Bigg)^{2}= -z^{2}+ B^{2}
$$

The sign of $\mathrm{d}z/\mathrm{d}\theta$ changes at the radial turning points, so the squared equation cannot be solved by choosing a single square-root branch throughout the orbit. Instead, use the radial equation of motion with $L\ne 0$ and $y=1/r$:

$$
\begin{aligned}
m(\ddot{r}-r\dot{\theta}^{2}) &= -\frac{\gamma}{r^{2}}, \\
\frac{\mathrm{d}y}{\mathrm{d}\theta} &= -\frac{m}{L}\dot{r}, \\
\frac{\mathrm{d}^{2}y}{\mathrm{d}\theta^{2}} &= -\frac{m^{2}r^{2}}{L^{2}}\ddot{r}=\frac{m\gamma}{L^{2}}-y.
\end{aligned}
$$

Since $z=y-m\gamma/L^{2}$, this gives $\mathrm{d}^{2}z/\mathrm{d}\theta^{2}+z=0$. The squared first-order equation above fixes the amplitude to $B$. For $B>0$, take $\theta=0$ at periapsis, where $y$ and $z$ are largest. The result also includes the circular case $B=0$:

```{math}
:label: eq-b-14
:enumerator: B.14

z = B\cos\theta
```

Now we need to put back all of those substitutions that we made!

$$
1. z = y - \frac{m\gamma}{L^{2}} \quad\Rightarrow  y - \frac{m\gamma}{L^{2}} = B\cos \theta
$$

$$
2. y = \frac{1}{r} \quad\Rightarrow  \frac{1}{r} - \frac{m\gamma}{L^{2}} = B\cos \theta
$$

<!-- Source PDF page 286; printed label 277. -->

3. From Equation B.13: $B = \dfrac{m\gamma}{L^{2}}\sqrt{1 + \dfrac{2EL^{2}}{m\gamma^{2}}}$

```{math}
:label: eq-b-15
:enumerator: B.15

\begin{aligned}
\frac{1}{r} - \frac{m\gamma}{L^{2}}
&= \frac{m\gamma}{L^{2}}\sqrt{1 + \frac{2EL^{2}}{m\gamma^{2}}}\,\cos\theta \\
\frac{1}{r}
&= \frac{m\gamma}{L^{2}} + \frac{m\gamma}{L^{2}}\sqrt{1 + \frac{2EL^{2}}{m\gamma^{2}}}\,\cos\theta \\
\frac{1}{r}
&= \frac{m\gamma}{L^{2}}\left(1 + \sqrt{1 + \frac{2EL^{2}}{m\gamma^{2}}}\,\cos\theta\right)
\end{aligned}
```

We now define the eccentricity of the orbit, $\varepsilon$ as:

```{math}
:label: eq-b-16
:enumerator: B.16

\varepsilon = \sqrt{1 + \frac{2EL^{2}}{m\gamma^{2}}}
```

Substitute Equation B.16 into Equation B.15:

```{math}
:label: eq-b-17
:enumerator: B.17

\frac{1}{r} = \frac{m\gamma}{L^{2}} (1 + \varepsilon \cos \theta)
```

Finally, let’s solve for $r$.

```{math}
:label: eq-b-18
:enumerator: B.18

r = \Bigg(\frac{L^{2}}{m\gamma} \Bigg) \frac{1}{1 + \varepsilon \cos \theta}
```

We now have an equation of $r(\theta)$ that defines our orbit. You will note that Equation B.18 has a similar structure to the equation for a generic ellipse (Equation 11.2), but with different constants out front.

If $\varepsilon$ = 0, then we have a circular orbit with a radius of

```{math}
:label: eq-b-19
:enumerator: B.19

r_{c}= \frac{L^{2}}{m\gamma}
```

We define $r_{c}$ as the radius of a circular orbit for a given angular momentum, $L$. See also [Chapter 11.2](#sec-11-2) for the derivation of $r_{c}$ using Newton’s laws.

So substituting in $r_{c}$, we recover Equation 11.7.

```{math}
:label: eq-b-20
:enumerator: B.20

r = \frac{r_{c}}{1 + \varepsilon \cos \theta}
```

(sec-B-2)=
## B.2 Approximations

Many times, mathematical functions can be simplified by using limits and making reasonable approximations. There are many ways to simplify a function. Here, we will look at a few of them.

<!-- Source PDF page 287; printed label 278. -->

(sec-B-2-1)=
### B.2.1 Binomial Approximation

For simple power functions, such as $f(x)$ = (1 + $x)^{a}$, you can apply the binomial or linear expansion to approximate their value. The approximation works as follows:

$$
f(x) \approx f(x_{0}) + \frac{\mathrm{d}f(x_{0})}{\mathrm{d}x} (x - x_{0})
$$

where $x_{0}$ is the point about which you are measuring $x$. That is, you are expanding the series about the point where $x = x_{0}$.

At first glance, this approximation seems reasonable. The approximation states that the value of a function at position $x$ near position $x_{0}$ can be approximated by the value at position $x_{0}$ with a modification given by the slope at $x_{0}$ and the distance between $x_{0}$ and $x$. For values of $x \approx x_{0}$, this approximation should be reasonable.

For the function, $f(x)$ = (1 + $x)^{a}$ with $x_{0}$ = 0, the binomial approximation would be,

$$
\begin{aligned}
f(x) &\approx f(0) + \frac{\mathrm{d}f(0)}{\mathrm{d}x} (x) \\
f(x) &\approx 1 + ax
\end{aligned}
$$

In this case, the value of $x$ must be close to zero for the approximation to be valid. If $x$ is not close to zero, then we need to shift $x_{0}$.

(sec-B-2-2)=
### B.2.2 Taylor Series

If $f$ has $n+1$ continuous derivatives near $x_0$, its Taylor polynomial gives a local approximation with a remainder of order $(x-x_0)^{n+1}$:

$$
\begin{aligned}
f(x) &= f(x_{0}) + \frac{\mathrm{d}f(x_{0})}{\mathrm{d}x} (x - x_{0}) + \frac{1}{2} \frac{\mathrm{d}^{2}f(x_{0})}{\mathrm{d}x^{2}} (x - x_{0})^{2} \\
&\quad{}+\frac{1}{3!} \frac{\mathrm{d}^{3}f(x_{0})}{\mathrm{d}x^{3}} (x - x_{0})^{3}+ \cdots + \frac{1}{n!} \frac{\mathrm{d}^{n}f(x_{0})}{\mathrm{d}x^{n}} (x - x_{0})^{n}+R_n(x).
\end{aligned}
$$

For a function analytic near $x_0$, the corresponding infinite Taylor series equals $f(x)$ in a neighborhood of $x_0$.

For example, the Taylor series expansion of $\sqrt{1 + x}$ (where $x_{0}$ = 0) is equal to:

$$
\begin{aligned}
\sqrt{1 + x}
&= 1 + \frac{1}{2}x + \frac{1}{2!}\left(-\frac{1}{4}\right)x^{2} + \frac{1}{3!}\left(\frac{3}{8}\right)x^{3} + \cdots \\
\sqrt{1 + x}
&= 1 + \frac{1}{2}x - \frac{1}{8}x^{2} + \frac{1}{16}x^{3} - \cdots
\end{aligned}
$$

If $x$ is small $(x$ is close to zero), then $x^{2}$ and $x^{3}$ are very small and don’t change the result much. For example, if $x = 0.1$, then $x^{3}= 0.001$ and $\frac{1}{16} x^{3}= 6.25\times 10^{-5}$. That term is much smaller than 1 and all subsequent terms will be even smaller, so they are negligible. That means, for small values of $x$, we can approximate $\sqrt{1 + x}$ as:

$$
\sqrt{1 + x} \approx 1 + \frac{1}{2}x
$$

<!-- Source PDF page 288; printed label 279. -->

It is key that $x$ is small (for $x_{0}$ = 0). If $x$ is larger, then the higher order terms are more significant and cannot be considered negligible.

The Taylor series for $\sin x$ and $\cos x$ (with $x_{0}$ = 0) are:

$$
\begin{aligned}
\sin x &= x - \frac{x^{3}}{3!} + \frac{x^{5}}{5!} - \frac{x^{7}}{7!} + \frac{x^{9}}{9!} - \cdots \\
\cos x &= 1 - \frac{x^{2}}{2!} + \frac{x^{4}}{4!} - \frac{x^{6}}{6!} + \frac{x^{8}}{8!} - \cdots
\end{aligned}
$$

Note that $x$ must be in radians for the Taylor series approximation to hold. You cannot use $x$ in degrees. If $x$ (in radians) is small, then the higher order terms again become negligible and $\sin x \approx x$ and $\cos x \approx 1 - \frac{x^{2}}{2}$. There are several functions with well established Taylor series approximations based on the above definition. [Appendix A.3](#sec-A-3) lists the expansions for many common equations.

::::{admonition} Small Angle Approximation

The small angle approximation is an application of the Taylor Series expansion. It states that the separation $s$ between two points subtended by an angle is $s = D\tan \theta \approx D\theta$, where $D$ is the distance between you and the points (see figure below for definitions).

:::{image} ../images/figures/figure-p288-1.png
:alt: Cartoon showing the angle created by a building a distance D from an observer.
:width: 279px
:align: center
:::

You will use the small angle assumption many times in this course and in other courses. As an astronomer, I use the small angle approximation in my research all the time. For example, large objects in space

(e.g., diameter of a crater on the moon, radius of a planet-forming disk around another star, distance between two interacting galaxies) subtend very tiny angles because they are so far away $(\theta$ is small because $D$ is large). We also use this approximation in optics with interference and diffraction patterns, where the distance to the first fringes corresponds to small angle differences from the normal.

::::

::::{tip} Quick Questions

1. Use a calculator to verify that $\sin x \approx x$ and $\cos x \approx 1 - \frac{x^{2}}{2}$ for small angles.

2. Try plotting both functions and see at which angles the approximations break down. Practice using a programming language like Python if you can.

3. You have a telescope and lens that can resolve (separate) objects that subtend angles of at least $0.0003^{\circ}$. Could you resolve a crater that is 1 km in diameter on the Moon with this telescope? Assume the Moon is 300,000 km away.

::::
