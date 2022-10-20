# 多元函数微分学
## 偏导数与全微分
我们把二元函数 $f(x, y)$ 看作两个独立自变量的函数, 如果固定 $y$, 可以将 $f(x, y)$ 看 作只关于 $x$ 的函数, 并可以计算导数，记为 $f(x, y)$ 关于自变量 $x$ 的偏导数 $\partial_x f$ 。用极限的 语言定义是

$$
\partial_x f(x, y)=\lim _{\Delta x \rightarrow 0} \frac{f(x+\Delta x)-f(x)}{\Delta x}
$$

我们注意到偏导数 $\partial_x f$ 也是一个二元函数, 因此我们可以讨论 $\partial_x f(x, y)$ 的连续性 和 $\partial_x f(x, y)$ 的导数。偏导数 $\partial_x f$ 的导数被称为二阶偏导数, 记为 $\partial_{x x} f$ 和 $\partial_{x y} f$, 其中形 如 $\partial_{x y} f$ 的对不同自变量求偏导数得到的二阶偏导数被称为混合偏导数。依次类推还可 以得到高阶偏导数。与一元函数类似, 我们称具有更高阶导数的函数具有更高的光滑 性。

### 高级偏导数
二阶偏导数的计算本身难度不大, 其核心是先算出一阶偏导数的表达式然后再对指定自变量求偏导。关于混合偏导数有一个有趣的结论：如果二元函数 $f(x, y)$ 的两个 混合偏导数在区域 $D$ 存在且连续, 那么两个混合偏导数 $\partial_{x y} f=\partial_{y x} f$ 在 $D$ 成立。这也使 得我们在研究混合偏导数时, 不需关心先对 $f$ 的哪个自变量求导, 只要 $f$ 有足够的光滑性, 那么 $f$ 的两个混合偏导数是一致的。

### 全微分
我们指出过, 偏导数和高阶偏导数都是独立自变量意义下的概念, 因此偏导数和高阶偏导数都只能体现 $f(x, y)$ 固定一个自变量时另一自变量的变化率。如果想收集点 $(x, y)$ 靠近点 $\left(x_0, y_0\right)$ 时 $f(x, y)$ 的整体变化率, 仅仅体现单个方向变化的偏导数远远不够。接着我们引入全微分。

对二元函数使用微分的化曲为直思想, 就可以用二元线性函数 $A \Delta x+B \Delta y$ 去近似 变化值 $\Delta f=f\left(x_0+\Delta x, y_0+\Delta y\right)-f\left(x_0, y_0\right)$, 其中 $A, B$ 是待定常数。用严格的数学语 言叙述: 如果 $f(x, y)$ 在点 $\left(x_0, y_0\right)$ 某邻域里有定义, 并且存在实数 $A, B$ 使得 $\Delta u=u\left(x_0+\Delta x, y_0+\Delta y\right)-u\left(x_0, y_0\right)=A \Delta x+B \Delta y+o(\rho), \quad(\Delta x, \Delta y) \rightarrow(0,0),(30)$ 其中 $\rho=\sqrt{(\Delta x)^2+(\Delta y)^2}$ 。那么称二元线性函数 $A \Delta x+B \Delta y$ 为 $f(x, y)$ 在点 $\left(x_0, y_0\right)$ 的全 微分, 此时 $f$ 在点 $\left(x_0, y_0\right)$ 可微。为了方便起见, 我们一般将全微分记做

$$
\mathrm{d} u=A \mathrm{~d} x+B \mathrm{~d} y .
$$

当题目需要我们计算全微分时, 结果就是形如上面的式子的形式。
