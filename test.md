# 📚 微积分函数极限练习题

## 🎯 题目1：基本极限计算

**题目**：计算 $\lim_{x \to 2} \frac{x^2 - 4}{x - 2}$

**解答**：
这是一个 $\frac{0}{0}$ 型未定式。

方法一：因式分解
$$\lim_{x \to 2} \frac{x^2 - 4}{x - 2} = \lim_{x \to 2} \frac{(x-2)(x+2)}{x - 2} = \lim_{x \to 2} (x+2) = 4$$

方法二：洛必达法则
$$\lim_{x \to 2} \frac{x^2 - 4}{x - 2} = \lim_{x \to 2} \frac{2x}{1} = 4$$

**答案**：4

---

## 🎯 题目2：三角函数极限

**题目**：计算 $\lim_{x \to 0} \frac{\sin 3x}{x}$

**解答**：
利用重要极限 $\lim_{t \to 0} \frac{\sin t}{t} = 1$

$$\lim_{x \to 0} \frac{\sin 3x}{x} = \lim_{x \to 0} \frac{\sin 3x}{3x} \cdot 3 = 3 \lim_{x \to 0} \frac{\sin 3x}{3x}$$

令 $t = 3x$ ，当 $x \to 0$ 时， $t \to 0$ ：
$$3 \lim_{t \to 0} \frac{\sin t}{t} = 3 \cdot 1 = 3$$

**答案**：3

---

## 🎯 题目3：无穷远处的极限

**题目**：计算 $\lim_{x \to +\infty} \frac{3x^2 + 2x - 1}{2x^2 - x + 5}$

**解答**：
分子分母同时除以 $x^2$（最高次项）：

$$\lim_{x \to +\infty} \frac{3x^2 + 2x - 1}{2x^2 - x + 5} = \lim_{x \to +\infty} \frac{3 + \frac{2}{x} - \frac{1}{x^2}}{2 - \frac{1}{x} + \frac{5}{x^2}}$$

当 $x \to +\infty$ 时：
- $\frac{2}{x} \to 0$ ， $\frac{1}{x^2} \to 0$ ， $\frac{1}{x} \to 0$ ， $\frac{5}{x^2} \to 0$

因此：
$$\lim_{x \to +\infty} \frac{3 + 0 - 0}{2 - 0 + 0} = \frac{3}{2}$$

**答案**： $\frac{3}{2}$

---

## 🎯 题目4：指数函数极限

**题目**：计算 $\lim_{x \to 0} \frac{e^x - 1}{x}$

**解答**：
这是一个 $\frac{0}{0}$ 型未定式。

方法一：洛必达法则
$$\lim_{x \to 0} \frac{e^x - 1}{x} = \lim_{x \to 0} \frac{e^x}{1} = e^0 = 1$$

方法二：泰勒展开
$e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots$

$$\lim_{x \to 0} \frac{e^x - 1}{x} = \lim_{x \to 0} \frac{x + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots}{x} = \lim_{x \to 0} (1 + \frac{x}{2!} + \frac{x^2}{3!} + \cdots) = 1$$

**答案**：1

---

## 🎯 题目5：复合函数极限

**题目**：计算 $\lim_{x \to 1} \frac{\sqrt{x+3} - 2}{x - 1}$

**解答**：
这是一个 $\frac{0}{0}$ 型未定式。

方法一：分子有理化
$$\lim_{x \to 1} \frac{\sqrt{x+3} - 2}{x - 1} = \lim_{x \to 1} \frac{(\sqrt{x+3} - 2)(\sqrt{x+3} + 2)}{(x - 1)(\sqrt{x+3} + 2)}$$

$$= \lim_{x \to 1} \frac{(x+3) - 4}{(x - 1)(\sqrt{x+3} + 2)} = \lim_{x \to 1} \frac{x - 1}{(x - 1)(\sqrt{x+3} + 2)}$$

$$= \lim_{x \to 1} \frac{1}{\sqrt{x+3} + 2} = \frac{1}{\sqrt{4} + 2} = \frac{1}{4}$$

**答案**： $\frac{1}{4}$

---

## 🎯 题目6：三角函数复合极限

**题目**：计算 $\lim_{x \to 0} \frac{1 - \cos x}{x^2}$

**解答**：
这是一个 $\frac{0}{0}$ 型未定式。

方法一：三角恒等式变换
利用 $1 - \cos x = 2\sin^2(\frac{x}{2})$：

$$\lim_{x \to 0} \frac{1 - \cos x}{x^2} = \lim_{x \to 0} \frac{2\sin^2(\frac{x}{2})}{x^2}$$

$$= \lim_{x \to 0} \frac{2\sin^2(\frac{x}{2})}{4(\frac{x}{2})^2} = \frac{2}{4} \lim_{x \to 0} \left(\frac{\sin(\frac{x}{2})}{\frac{x}{2}}\right)^2 = \frac{1}{2} \cdot 1^2 = \frac{1}{2}$$

方法二：洛必达法则（两次）
$$\lim_{x \to 0} \frac{1 - \cos x}{x^2} = \lim_{x \to 0} \frac{\sin x}{2x} = \lim_{x \to 0} \frac{\cos x}{2} = \frac{1}{2}$$

**答案**： $\frac{1}{2}$

---

## 🎯 题目7：分段函数极限


**题目**：设    
$$
f(x) = \begin{cases}
x^2 + 1, & x < 2 \\
3x - 1, & x \geq 2
\end{cases}
$$ 

求 $\lim_{x \to 2} f(x)$

**解答**：
需要分别计算左极限和右极限。

左极限：
$$\lim_{x \to 2^-} f(x) = \lim_{x \to 2^-} (x^2 + 1) = 2^2 + 1 = 5$$

右极限：
$$\lim_{x \to 2^+} f(x) = \lim_{x \to 2^+} (3x - 1) = 3 \cdot 2 - 1 = 5$$

因为左极限 = 右极限 = 5，所以：
$$\lim_{x \to 2} f(x) = 5$$

**答案**：5

---

## 🎯 题目8：无穷小比较

**题目**：计算 $\lim_{x \to 0} \frac{\tan x - \sin x}{x^3}$

**解答**：
这是一个 $\frac{0}{0}$ 型未定式。

方法一：泰勒展开
$$\sin x = x - \frac{x^3}{6} + \frac{x^5}{120} + O(x^7)$$
$$\tan x = x + \frac{x^3}{3} + \frac{2x^5}{15} + O(x^7)$$

因此：
$$\tan x - \sin x = \left(x + \frac{x^3}{3} + \frac{2x^5}{15}\right) - \left(x - \frac{x^3}{6} + \frac{x^5}{120}\right)$$
$$= \frac{x^3}{3} + \frac{x^3}{6} + O(x^5) = \frac{x^3}{2} + O(x^5)$$

所以：
$$\lim_{x \to 0} \frac{\tan x - \sin x}{x^3} = \lim_{x \to 0} \frac{\frac{x^3}{2} + O(x^5)}{x^3} = \frac{1}{2}$$

**答案**： $\frac{1}{2}$

---

## 🎯 题目9：重要极限应用

**题目**：计算 $\lim_{x \to 0} (1 + 2x)^{\frac{1}{x}}$

**解答**：
利用重要极限 $\lim_{t \to 0} (1 + t)^{\frac{1}{t}} = e$

令 $t = 2x$ ，当 $x \to 0$ 时， $t \to 0$ ：
$$\lim_{x \to 0} (1 + 2x)^{\frac{1}{x}} = \lim_{x \to 0} (1 + 2x)^{\frac{2}{2x}} = \lim_{x \to 0} [(1 + 2x)^{\frac{1}{2x}}]^2$$

$$= \lim_{t \to 0} [(1 + t)^{\frac{1}{t}}]^2 = e^2$$

**答案**： $e^2$

---

## 🎯 题目10：综合应用题

**题目**：计算 $\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^{2n}$

**解答**：
这是重要极限的变形。

方法一：直接变换
$$\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^{2n} = \lim_{n \to \infty} \left[\left(1 + \frac{1}{n}\right)^n\right]^2$$

利用 $\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n = e$：
$$= \left[\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n\right]^2 = e^2$$

方法二：取对数
令 $y = \left(1 + \frac{1}{n}\right)^{2n}$，则 $\ln y = 2n \ln\left(1 + \frac{1}{n}\right)$

$$\lim_{n \to \infty} \ln y = \lim_{n \to \infty} 2n \ln\left(1 + \frac{1}{n}\right) = \lim_{n \to \infty} \frac{2\ln\left(1 + \frac{1}{n}\right)}{\frac{1}{n}}$$

这是 $\frac{0}{0}$ 型，使用洛必达法则：
$$= \lim_{n \to \infty} \frac{2 \cdot \frac{1}{1 + \frac{1}{n}} \cdot \left(-\frac{1}{n^2}\right)}{-\frac{1}{n^2}} = \lim_{n \to \infty} \frac{2}{1 + \frac{1}{n}} = 2$$

因此： $\lim_{n \to \infty} y = e^2$

**答案**： $e^2$

---

## 📝 总结要点

### 重要极限公式：
1. $\lim_{x \to 0} \frac{\sin x}{x} = 1$
2. $\lim_{x \to 0} (1 + x)^{\frac{1}{x}} = e$
3. $\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n = e$

### 常用方法：
1. **因式分解**：处理多项式的 $\frac{0}{0}$ 型
2. **有理化**：处理根式的未定式
3. **洛必达法则**：处理 $\frac{0}{0}$ 或 $\frac{\infty}{\infty}$ 型
4. **泰勒展开**：精确计算复杂函数的极限
5. **等价无穷小替换**：简化计算过程

### 注意事项：
- 检查极限是否存在（左右极限是否相等）
- 识别未定式的类型
- 选择合适的方法求解
- 验证计算结果的合理性
