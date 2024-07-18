---
title: Sample Solutions 3 July 17
draft: 
tags:
---
## Parallelogram identity
1. && Compute $\mathbf{u} - \mathbf{v}$ and $\mathbf{u} + \mathbf{v}$ using the rules of vector addition  %% fold %% 
    - Componentwise addition, subtraction: $$\begin{align*}\mathbf{u} - \mathbf{v} &= \left(\begin{smallmatrix}4 \\ 0 \\ 3\end{smallmatrix}\right) - \left(\begin{smallmatrix}-2 \\ 1 \\ 5\end{smallmatrix}\right) = \left(\begin{smallmatrix}6 \\ -1 \\ -2\end{smallmatrix}\right)\\\\ \mathbf{u} + \mathbf{v} &= \left(\begin{smallmatrix}4 \\ 0 \\ 3\end{smallmatrix}\right) + \left(\begin{smallmatrix}-2 \\ 1 \\ 5\end{smallmatrix}\right) = \left(\begin{smallmatrix}2 \\ 1 \\ 8\end{smallmatrix}\right)\end{align*}$$
2. && Compute norms using $|\mathbf{v}| = \sqrt{\mathbf{v} \cdot \mathbf{v}}$ %% fold %% 
    - Plug in data: $$\begin{align*}|\mathbf{u}| &= \sqrt{4^2 + 0^2 + 3^2} = 5\\ |\mathbf{v}| &= \sqrt{(-2)^2 + 1^2 + 5^2} = \sqrt{30}\\ |\mathbf{u} - \mathbf{v}| &= \sqrt{6^2 + (-1)^2 + (-2)^2} = \sqrt{41}\\ |\mathbf{u} + \mathbf{v}| &= \sqrt{2^2 + 1^2 + 8^2} = \sqrt{69}\end{align*}$$
3. && Verify $|\mathbf{u} + \mathbf{v}|^2 + |\mathbf{u} - \mathbf{v}|^2 = 2|\mathbf{u}|^2 + 2|\mathbf{v}|^2$ %% fold %% 
    - Plug in data: $$\begin{align*}|\mathbf{u} + \mathbf{v}|^2 + |\mathbf{u} - \mathbf{v}|^2 &= (\sqrt{69})^2 + (\sqrt{41})^2 = 110\\\\ 2|\mathbf{u}|^2 + 2|\mathbf{v}|^2 &= 2(5^2) + 2(\sqrt{30})^2 = 2(25) + 2(30) = 110\end{align*}$$
    - Substitute on both sides to verify equality.

## Angle between some vectors
1. && Obtain formula $\theta = \cos^{-1}\left(\frac{\mathbf{u} \cdot \mathbf{v}}{|\mathbf{u}| |\mathbf{v}|}\right)$ %% fold %% 
    - !! Cosine Angle Rule: $\mathbf{x} \cdot \mathbf{y} = |\mathbf{x}| |\mathbf{y}| \cos(\theta)$
    - Rearrange cosine angle rule: $$\mathbf{u} \cdot \mathbf{v} = |\mathbf{u}| |\mathbf{v}| \cos(\theta) \qquad ⨠⨠ \qquad \cos(\theta) = \frac{\mathbf{u} \cdot \mathbf{v}}{|\mathbf{u}| |\mathbf{v}|} \qquad ⨠⨠ \qquad \theta = \cos^{-1}\left(\frac{\mathbf{u} \cdot \mathbf{v}}{|\mathbf{u}| |\mathbf{v}|}\right)$$
3. && Compute $\theta\approx 0.705\text{ rad}$ %% fold %% 
    - Plug in data: $$\begin{align*}\cos(\theta) &= \frac{(3, 6, 2) \cdot (4, 2, 4)}{|(3, 6, 2)| |(4, 2, 4)|}\\\\ \theta &= \cos^{-1}\left(\frac{32}{42}\right) \approx 0.705\text{ rad}\end{align*}$$

## Acute, orthogonal, or obtuse?
1. &&& Sign of the dot product determines quality of the angle %% fold %% 
    - !! Cosine Angle Rule: $\mathbf{x} \cdot \mathbf{y} = |\mathbf{x}| |\mathbf{y}| \cos(\theta)$ %% fold %%
    - && Dot product signs ↔ Angle quality
        1. $\mathbf{x} \cdot \mathbf{y}>0$, angle between $\mathbf{u}$ and $\mathbf{v}$ is obtuse
        1. $\mathbf{x} \cdot \mathbf{y}<0$, angle between $\mathbf{u}$ and $\mathbf{w}$ is acute
        1. $\mathbf{x} \cdot \mathbf{y}=0$, $\mathbf{v}$ and $\mathbf{w}$ are perpendicular
2. && Compute the dot products %% fold %% 
    - Plug in data: $$\begin{align*}\mathbf{u} \cdot \mathbf{v} &= \left(\frac{1}{2}\right)(3) + \left(\frac{1}{2}\right)(1) + (5)(-2)=-8\\\\ \mathbf{u} \cdot \mathbf{w} &= \left(\frac{1}{2}\right)(4) + \left(\frac{1}{2}\right)(-3) + (5)(0) = \frac{1}{2}\\\\ \mathbf{v} \cdot \mathbf{w} &= (3)(4) + (1)(-3) + (-2)(0) = 9\end{align*}$$
3. && Evaluate signs of the dot products %% fold %% 
    - Angle between $\mathbf{u}$ and $\mathbf{v}$ is obtuse because $\mathbf{u} \cdot \mathbf{v}<0$
    - Angle between $\mathbf{u}$ and $\mathbf{w}$ is acute because $\mathbf{u} \cdot \mathbf{w}>0$
    - Angle between $\mathbf{v}$ and $\mathbf{w}$ is acute because $\mathbf{v} \cdot \mathbf{w}>0$


## Distance between parallel planes
1. & Name the planes.
    - Let $\mathbf{P}_1$ be the plane satisfying $15x+3y-3z-10=0$.
    - Let $\mathbf{P}_2$ be the plane satisfying $5x+y-z-3=0$.
2. &&& Find a vector $\mathbf{b}$ with head in $\mathbf{P}_2$ when tail is in $\mathbf{P}_1$.
    - & Choose $\mathbf{v}_1\in\mathbf{P}_1$ and $\mathbf{v}_2\in\mathbf{P}_2$. %% fold %% 
        - Choose any convenient vectors: $$\mathbf{v}_1 = \begin{pmatrix} 2/3 \\ 0 \\ 0 \end{pmatrix},\quad \mathbf{v}_2 = \begin{pmatrix} 3/5 \\ 0 \\ 0 \end{pmatrix}$$
    - & Define new vector $\mathbf{b}=\mathbf{v}_2-\mathbf{v}_1$.
        - Calculate components of $\mathbf{b}$: $$\mathbf{b} = \mathbf{v}_2 - \mathbf{v}_1 = \begin{pmatrix} \frac{3}{5} \\ 0 \\ 0 \end{pmatrix} - \begin{pmatrix} \frac{2}{3} \\ 0 \\ 0 \end{pmatrix} = \begin{pmatrix} -\frac{1}{15} \\ 0 \\ 0 \end{pmatrix}$$
3. && Find the normal vectors, $\mathbf{n}_1$ to $\mathbf{P}_1$ and $\mathbf{n}_2$ to $\mathbf{P}_2$. %% fold %% 
    - Read off the coefficients in the scalar equations of $\mathbf{P}_1$ and $\mathbf{P}_2$: $$\begin{align*}\mathbf{P}_1 &:\;\, 15x+3y-3z-10=0 \qquad &⨠⨠ \qquad \mathbf{n}_1 = \begin{pmatrix} 15 \\ 3 \\ -3 \end{pmatrix}\\ \mathbf{P}_2 &:\;\, 5x+y-z-3=0 \qquad &⨠⨠ \qquad \mathbf{n}_2 = \begin{pmatrix} 5 \\ 1 \\ -1 \end{pmatrix}\end{align*}$$
    - (Notice: $\mathbf{n}_1$ is parallel to $\mathbf{n}_2$. Because the planes are parallel.)
4. !! The distance from $\mathbf{P}_1$ to $\mathbf{P}_2$ equals the scalar projection of $\mathbf{b}$ onto either plane’s normal vector. %% fold %%
5. && Choose $\mathbf{n}_1$ and compute the scalar projection of $\mathbf{b}$ onto $\mathbf{n}_1$. %% fold %% 
    - Computing for $\mathbf{n}_1$: $$\frac{\mathbf{b} \cdot \mathbf{n}_1}{|\mathbf{n}_1|} = \frac{(\frac{-1}{15} , 0, 0) \cdot (15,3,-3)}{|(15,3,-3)|} = \frac{-1}{\sqrt{243}} = -\frac{1}{9\sqrt{3}}$$
    - (Same result for $\mathbf{n}_2$ but harder arithmetic.)
6. & Answer $=$ $\frac{1}{9\sqrt{3}}$. %% fold %% 
    - $$\text{Distance between planes} = \left| -\frac{1}{9\sqrt{3}}\right| = \frac{1}{9\sqrt{3}}$$


## Line of intersection between planes
1. & Points $(x,y,z)$ in *both* planes must satisfy *both* equations simultaneously.
    - System of equations: $$\left\{\begin{align*}6x - 3y + z - 5 &= 0 \\-x + y + 5z - 5 &= 0\end{align*}\right.$$
2. && Eliminate $z$ variable. %% fold %% 
    - Solve the first for $z$: $$z = 1 + \frac{x}{5} + \frac{ - y}{5}$$
    - Solve the second for $z$: $$z = 5-6x+3y$$
    - Equate formulas for $z$ and rearrange: $$1 + \frac{x}{5} + \frac{ - y}{5} = 5-6x+3  y \qquad ⨠⨠ \qquad y = \frac{31}{16}x-\frac{5}{4}$$
    - Now $z$ and $y$ are determined by formulas in terms of $x$.
3. !! Consider $x$ an independent parameter; change its name to $t$.
4. && Combine all formulas into the parametric vector function $(x,y,z)=(16t,\;31t-20,\;-3t+20)$. %% fold %% 
    - $$\left\{\begin{align*}x &= t \\y &= \frac{31}{16}t - \frac{5}{4} \\z &= -\frac{3}{16}t + \frac{5}{4}\end{align*}\right. \qquad ⨠⨠ \qquad (x,y,z)=\left(t,\;\frac{31}{16}t - \frac{5}{4},\;-\frac{3}{16}t + \frac{5}{4}\right)$$
    - *If desired*, change parameter from $t$ to $16t$: $$(x,y,z)=(16t,\;31t-20,\;-3t+20)$$
    - This answers the first question.
5. !!! The angle between two planes equals the angle between their normal vectors. %% fold %% 
    - View the planes so that the line of intersection passes directly into the page.
    - The angle between the planes can be rotated to align with the angle between their normal vectors. \[Insert diagram here.]
6. && Find the normal vectors, $\mathbf{n}_1$ to $\mathbf{P}_1$ and $\mathbf{n}_2$ to $\mathbf{P}_2$. %% fold %% 
    - Read off the coefficients: $$\begin{align*}\mathbf{P}_1 &:\;\, 6x - 3y + z - 5 = 0 \qquad &⨠⨠ \qquad \mathbf{n}_1 = \begin{pmatrix} 6 \\ -3 \\ 1 \end{pmatrix}\\ \mathbf{P}_2 &:\;\, -x + y + 5z - 5 = 0 \qquad &⨠⨠ \qquad \mathbf{n}_2 = \begin{pmatrix} -1 \\ 1 \\ 5 \end{pmatrix}\end{align*}$$
7. !! Cosine Angle Rule: $\mathbf{n}_1 \cdot \mathbf{n}_2 = |\mathbf{n}_1| |\mathbf{n}_2| \cos(\theta)$. %% fold %% 
    - Rearrange: $$\cos(\theta) = \frac{\mathbf{n}_1 \cdot \mathbf{n}_2}{|\mathbf{n}_1| |\mathbf{n}_2|}$$
8. && Compute that $\theta\approx 96.52^\circ$. %% fold %% 
    - Compute the dot product: $$\mathbf{n}_1 \cdot \mathbf{n}_2 = (6)(-1) + (-3 )(1) + (1)(5) = -6 - 3 + 5 = -4$$
    - Compute the norms: $$\begin{align*}|\mathbf{n}_1| &= \sqrt{6^2 + (-3)^2 + 1^2} = \sqrt{46}\\ |\mathbf{n}_2| &= \sqrt{(-1)^2 + 1^2 + 5^2} = \sqrt{27}\end{align*}$$
    - Compute the cosine using (7): $$\cos(\theta) = \frac{-4}{\sqrt{(46)(27)}} = -\frac{4}{\sqrt{1242}}$$
    - Compute the angle, the answer: $$\theta = \cos^{-1}\left(\frac{-4}{\sqrt{1242}}\right) \approx 96.52^\circ$$
    - This angle is obtuse, which is consistent with a negative dot product $-4<0$.


## Span
What we have here is an equation for a plane and two vectors that span the plane. To find a normal vector, we can take the cross product between the two vectors. This will yield a third vector perpendicular to the other two.

$$

\mathbf{n} = \begin{pmatrix} 2 \\ 0 \\ 1 \end{pmatrix} \times \begin{pmatrix} -1 \\ 1 \\ 3 \end{pmatrix}

$$

Solving, we get:

$$

\mathbf{n} = \begin{pmatrix} -1 \\ -7 \\ 2 \end{pmatrix}

$$

You can check that $\mathbf{n}$ is orthogonal to the generating vectors using the dot product.

This vector $\mathbf{n} = \begin{pmatrix} 0 \\ 5 \\ 2 \end{pmatrix}$ is normal to the plane. The scalar equation of the plane can be expressed as:

$$-1x + -7y + 2z = 0$$
## Independence
Let’s name the vectors $\mathbf{v}_1$, $\mathbf{v}_2$, and $\mathbf{v}_3$

There are many ways to solve this problem. Here is one using a system of equations:

$$x_1\mathbf{v}_1 + x_2\mathbf{v}_2=\mathbf{v}_3$$

Converting this vector addition to a system, we get:

$$

\begin{cases}

x_1 + 4x_2 &= 3 \\

-2x_1 &= -2 \\

3x_1 + 2x_2 &= 4

\end{cases}

$$

Solving this system for $x_1$ and $x_2$ yields:

$$x_1 = 1$$

$$x_2 = \frac{1}{2}$$

These are the coefficients for a linear combination of the first two vectors that yields the third. The vectors are dependent.
## Distance point to line
This question is all about projections and finding the vector between two vectors with subtraction.

Start by finding a vector $(\mathbf{p} - \mathbf{r}_0)$. This vector goes from a known point on the line to $\mathbf{p}$. For the given line, $\mathbf{r}_0 = \begin{pmatrix} -2 \\ 3 \\ 1 \end{pmatrix}$. So,

$$(\mathbf{p} - \mathbf{r}_0) = \begin{pmatrix} 1 \\ 5 \\ -2 \end{pmatrix} - \begin{pmatrix} -2 \\ 3 \\ 1 \end{pmatrix} = \begin{pmatrix} 3 \\ 2 \\ -3 \end{pmatrix}$$

Next, we project the vector $(\mathbf{p} - \mathbf{r}_0)$ onto the line. Recall that the projection of a vector $\mathbf{v}$ onto a direction vector $\mathbf{l}$ (direction of the line) is given by:

$$\mathrm{proj}_{\mathbf{l}}(\mathbf{v}) = \frac{\mathbf{v} \cdot \mathbf{l}}{\mathbf{l} \cdot \mathbf{l}} \mathbf{l}$$

Since $(\mathbf{p} - \mathbf{r}_0) = \begin{pmatrix} 3 \\ 2 \\ -3 \end{pmatrix}$ and $\mathbf{l} = \begin{pmatrix} 4 \\ 0 \\ -1 \end{pmatrix}$, we can find the projection.

$$(\mathbf{p} - \mathbf{r}_0) \cdot \mathbf{l} = \begin{pmatrix} 3 \\ 2 \\ -3 \end{pmatrix} \cdot \begin{pmatrix} 4 \\ 0 \\ -1 \end{pmatrix} = 12 - 0 + 3 = 15$$

$$\mathbf{l} \cdot \mathbf{l} = 4^2 + 0^2 + (-1)^2 = 17$$

$$\mathrm{proj}_{\mathbf{l}}(\mathbf{p} - \mathbf{r}_0) = \frac{15}{17} \mathbf{l} = \begin{pmatrix}60/17\\0\\-15/17 \end{pmatrix}$$

The final step is to find the distance between $\mathbf{p}$ and $\mathrm{proj}_{\mathbf{l}}(\mathbf{p} - \mathbf{r}_{0})+ \mathbf{r_0}$ 
Add the projection vector to $\mathbf{r}_0$ to find the point on the line closest to $\mathbf{p}$: $$\mathrm{proj}_{\mathbf{l}}(\mathbf{p} - \mathbf{r}_0) + \mathbf{r}_0 = \begin{pmatrix} \frac{60}{17} \\ 0 \\ -\frac{15}{17} \end{pmatrix} + \begin{pmatrix} -2 \\ 3 \\ 1 \end{pmatrix} = \begin{pmatrix} \frac{26}{17} \\ 3 \\ \frac{2}{17} \end{pmatrix}$$ Now, find the vector from $\mathbf{p}$ to this point: $$\mathbf{p} - \left(\mathrm{proj}_{\mathbf{l}}(\mathbf{p} - \mathbf{r}_0) + \mathbf{r}_0\right) = \begin{pmatrix} 1 \\ 5 \\ -2 \end{pmatrix} - \begin{pmatrix} \frac{26}{17} \\ 3 \\ \frac{2}{17} \end{pmatrix} = \begin{pmatrix} \frac{-9}{17} \\ 2 \\ -\frac{36}{17} \end{pmatrix}$$ Finally, find the magnitude of this vector to get the distance: $$|\mathbf{p} - \left(\mathrm{proj}_{\mathbf{l}}(\mathbf{p} - \mathbf{r}_0) + \mathbf{r}_0\right)| = \sqrt{\left( \frac{-9}{17} \right)^2 + 2^2 + \left( -\frac{36}{17} \right)^2} = \sqrt{\frac{149}{17}}$$
