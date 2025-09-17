
# 📘 10 Exercises on Monotonicity and Extrema (with Solutions)

---

### **Exercise 1. (Definition Check)**

State the definitions of **monotonically increasing** and **monotonically decreasing** functions. Give an example of each.

**Solution:**

* *Increasing:* On interval $I$, if for all $x_1 < x_2$, $f(x_1) < f(x_2)$, then $f$ is monotonically increasing.
  Example: $f(x) = e^x$.
* *Decreasing:* On interval $I$, if for all $x_1 < x_2$, $f(x_1) > f(x_2)$, then $f$ is monotonically decreasing.
  Example: $f(x) = -x$.

---

### **Exercise 2. (Monotonicity via Derivative)**

Find the monotonic intervals of

$$
f(x) = x^3 - 3x^2 + 2.
$$

**Solution:**

1. $f'(x) = 3x^2 - 6x = 3x(x-2)$.
2. Critical points: $x=0,2$.
3. Sign check:

   * $x < 0$: $f'>0$ → increasing.
   * $0<x<2$: $f'<0$ → decreasing.
   * $x>2$: $f'>0$ → increasing.

**Answer:** Increasing on $(-\infty,0)\cup(2,\infty)$; decreasing on $(0,2)$.

---

### **Exercise 3. (Always Increasing Function)**

Show that

$$
f(x) = \frac{x}{x+1}, \quad x>-1,
$$

is monotonically increasing.

**Solution:**

1. $f'(x) = \frac{1}{(x+1)^2}$.
2. Since $(x+1)^2>0$ for all $x>-1$, we have $f'(x) > 0$.

**Answer:** Increasing on $(-1,\infty)$.

---

### **Exercise 4. (Conceptual – True/False)**

Determine whether each is true or false:

1. If $f'(x)>0$, then $f$ is increasing.
2. If $f'(x)=0$, then $f$ must have an extremum.
3. A non-differentiable point can be an extremum.

**Solution:**

1. True.
2. False ($f(x)=x^3$ at $x=0$: no extremum).
3. True ($f(x)=|x|$ has minimum at $x=0$).

---

### **Exercise 5. (First Derivative Test)**

For

$$
f(x) = x^4 - 4x^2,
$$

find all local extrema.

**Solution:**

1. $f'(x) = 4x(x^2-2)$. Critical points: $x=0,\pm\sqrt{2}$.
2. Sign test:

   * $x<-√2$: $f'<0$ → decreasing.
   * $(-√2,0)$: $f'>0$ → increasing.
   * $(0,√2)$: $f'<0$ → decreasing.
   * $(√2,\infty)$: $f'>0$ → increasing.

**Answer:**

* Local min at $x=-√2$, $f(-√2)=-4$.
* Local max at $x=0$, $f(0)=0$.
* Local min at $x=√2$, $f(√2)=-4$.

---

### **Exercise 6. (Second Derivative Test)**

Find and classify extrema of

$$
f(x)=\ln(x)-x, \quad x>0.
$$

**Solution:**

1. $f'(x)=\frac{1}{x}-1$. Critical point: $x=1$.
2. $f''(x)=-\frac{1}{x^2}$. At $x=1$, $f''(1)=-1<0$.

**Answer:** Local maximum at $x=1$, value $f(1)=-1$.

---

### **Exercise 7. (Global Extrema on Closed Interval)**

Find the absolute maximum and minimum of

$$
f(x)=x^2-2x+1, \quad x\in[0,3].
$$

**Solution:**

1. $f(x)=(x-1)^2$.
2. $f'(x)=2(x-1)$. Critical point: $x=1$.
3. Evaluate:

   * $f(0)=1$.
   * $f(1)=0$.
   * $f(3)=4$.

**Answer:** Absolute min: $0$ at $x=1$. Absolute max: $4$ at $x=3$.

---

### **Exercise 8. (Optimization)**

A rectangular plot beside a river is fenced on three sides. Total fence length = 40 m. Maximize area.

**Solution:**

1. Let width = $x$, length = $y$. Constraint: $2x+y=40$. So $y=40-2x$.
2. Area: $A=xy=40x-2x^2$.
3. $A'(x)=40-4x=0 \Rightarrow x=10$. Then $y=20$.

**Answer:** Maximum area $200$ m² with dimensions $10 \times 20$.

---

### **Exercise 9. (Inflection Point)**

Find inflection point of

$$
f(x)=x^3-6x^2+9x.
$$

**Solution:**

1. $f''(x)=6x-12$. Solve: $f''(x)=0 \Rightarrow x=2$.
2. For $x<2$, $f''<0$ (concave down); for $x>2$, $f''>0$ (concave up).
3. $f(2)=8-24+18=2$.

**Answer:** Inflection point at $(2,2)$.

---

### **Exercise 10. (Curve Sketching)**

Sketch $f(x)=\frac{x}{1+x^2}$. Find monotonic intervals, extrema, and inflection points.

**Solution:**

1. Domain: all reals. Symmetry: odd function.
2. $f'(x)=\frac{1-x^2}{(1+x^2)^2}$. Critical points: $x=±1$.

   * $x<-1$: $f'<0$.
   * $(-1,1)$: $f'>0$.
   * $(1,∞)$: $f'<0$.
     → Local min at $(-1,-1/2)$, local max at $(1,1/2)$.
3. $f''(x)=\frac{2x(x^2-3)}{(1+x^2)^3}$. Inflection at $x=0,±√3$.
4. Asymptote: $\lim_{x→±∞} f(x)=0$.

**Answer:**

* Increasing on $(-1,1)$, decreasing elsewhere.
* Local max $(1,1/2)$, local min $(-1,-1/2)$.
* Inflections at $(-√3,-√3/4), (0,0), (√3,√3/4)$.

---



