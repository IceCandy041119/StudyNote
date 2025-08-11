
![[第一章+随机事件和概率.pdf#page=4&rect=85,689,508,768&color=yellow|第一章+随机事件和概率, p.4]]这里的$A-B = A\overline{B}$ 也等于$A-AB$,还有个小技巧进行快速的转换，即减去谁，就把减号移到谁上方，然后变为交的形式。






![[第一章+随机事件和概率.pdf#page=10&rect=84,470,507,523&color=yellow|第一章+随机事件和概率, p.10]]
这里的技巧为$将P(A-B)化为P(A\overline{B})$这是用头上没横的减去两者的交集，例子$P(A-B) = P(A) - P(AB),P(A-BC)=P(A\overline{BC})=P(A) - P(ABC),P(A\overline{B}C) = P(AC) - P(ABC)$





![[第一章+随机事件和概率.pdf#page=13&rect=105,482,516,527]]这里的独立和互斥的理解：
- 互斥就像是`早知哥哥来～我就不来了`突出个对头间的排斥，这里对概率的度量造成了影响，而独立突出一个独字，表示两个事件里，没有关联关系，不会对概率的度量造成影响。
当没有这个条件时，互斥和独立没有必然联系，如当$A = \phi,B = \Omega$时，可以看出独立和互斥都存在。  






![[第一章+随机事件和概率.pdf#page=14&rect=82,596,374,764&color=yellow|第一章+随机事件和概率, p.14]]
这里的两两独立和相互独立的差别，两两独立代表单独的两个事件间，没有关联，不会影响对概率的度量，但有第三者插足，就会造成度量的影响，而相互独立，表示，这一堆东西（事件）都没有什么关联。比如说：
- 有三个事件：
	- 抛硬币A为正面
	- 抛硬币B为正面
	- 为相同面
	- 这三个事件两两独立，但并不相互独立








![[第二章+随机变量及其分布.pdf#page=11&rect=95,303,247,356|第二章+随机变量及其分布, p.11]]
概率密度的充要条件    






![[第二章+随机变量及其分布.pdf#page=19&rect=94,211,506,306&color=yellow|第二章+随机变量及其分布, p.19]]
$Y=FX​(X)$ 的值是随机变量 $X$ 的观测值对应的累积概率，因此 $Y$ 的取值范围在 \[0,1\] 之间，可以映射到 \[0,1\]的数轴上。正是因为对于连续随机变量 $X$，其分布函数 $F(X)​$ 的这种映射关系，使得 $Y$ 的累积分布函数 $F_Y​(y)=P(Y≤y)$ 等于 $y (对于 0≤y≤1)$，这符合 \[0,1\] 上均匀分布的定义。     













![[第三章+多维随机变量及其分布.pdf#page=7&rect=80,353,448,486&color=yellow|第三章+多维随机变量及其分布, p.7]]
当离散型随机变量的分布律出现0时，必不独立。当其构成的分布律行（列）对应成比例时，独立。  










![[第六章+数理统计的基本概念.pdf#page=4&rect=92,383,398,457&color=yellow|第六章+数理统计的基本概念, p.4]]
对于一个随机变量，求其$k$次方的期望称为$k$阶原点矩$EX^k$,而$E(X-EX)^k$则称为k阶中心矩. 表现为期望和方差更为一般的形式.          






![[第八章+区间估计.pdf#page=4&rect=214,487,306,528|第八章+区间估计, p.4]]
这里应为$$\frac{\overline{X}-\overline{Y} - (\mu_1 - \mu_2)}{\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}} \sim N(0,1)$$









![[第九章+假设检验.pdf#page=4&rect=325,104,431,121&color=yellow|第九章+假设检验, p.4]]
p与a相近才作比较.    















![[第五章+大数定律和中心极限定理.pdf#page=3&rect=103,238,298,261&color=yellow|第五章+大数定律和中心极限定理, p.3]]
$\displaystyle\sum^n_{k=1}{X_k}$ and $N(n\mu,n\sigma^2)$











![[第五章+大数定律和中心极限定理.pdf#page=3&rect=85,130,507,230&color=yellow|第五章+大数定律和中心极限定理, p.3]]
伯努利试验本身就具有可加性，即可以将n重伯努利试验拆分成多个基础的伯努利试验，所以这里的$X_n$不需要求和








![[第六章+数理统计的基本概念.pdf#page=9&rect=118,346,285,398&color=yellow|第六章+数理统计的基本概念, p.9]]
**定理：** 设 $X_1, X_2, \dots, X_n$ 是从正态总体 $N(\mu, \sigma^2)$ 中抽取的容量为 $n$ 的一个简单随机样本。记样本均值 $\bar{X} = \frac{1}{n}\sum_{i=1}^{n}X_i$ 和样本方差 $S^2 = \frac{1}{n-1}\sum_{i=1}^{n}(X_i - \bar{X})^2$。则有：
1.  $\frac{(n-1)S^2}{\sigma^2} \sim \chi^2(n-1)$。
2.  $\bar{X}$ 和 $S^2$ 相互独立。

**证明：**

考虑以下恒等式：
$$ \sum_{i=1}^{n}(X_i - \mu)^2 = \sum_{i=1}^{n}(X_i - \bar{X} + \bar{X} - \mu)^2 $$
展开右边：
$$ \sum_{i=1}^{n}((X_i - \bar{X}) + (\bar{X} - \mu))^2 = \sum_{i=1}^{n}(X_i - \bar{X})^2 + 2\sum_{i=1}^{n}(X_i - \bar{X})(\bar{X} - \mu) + \sum_{i=1}^{n}(\bar{X} - \mu)^2 $$
对于中间项：
$$ 2\sum_{i=1}^{n}(X_i - \bar{X})(\bar{X} - \mu) = 2(\bar{X} - \mu)\sum_{i=1}^{n}(X_i - \bar{X}) = 2(\bar{X} - \mu)(n\bar{X} - n\bar{X}) = 0 $$
所以，恒等式简化为：
$$ \sum_{i=1}^{n}(X_i - \mu)^2 = \sum_{i=1}^{n}(X_i - \bar{X})^2 + n(\bar{X} - \mu)^2 $$
将两边同时除以 $\sigma^2$：
$$ \sum_{i=1}^{n}\frac{(X_i - \mu)^2}{\sigma^2} = \frac{1}{\sigma^2}\sum_{i=1}^{n}(X_i - \bar{X})^2 + \frac{n(\bar{X} - \mu)^2}{\sigma^2} $$
将左边改写为标准正态变量的平方和，右边第一项改写为 $(n-1)S^2/\sigma^2$，右边第二项改写为样本均值标准化的平方：
$$ \sum_{i=1}^{n}\left(\frac{X_i - \mu}{\sigma}\right)^2 = \frac{(n-1)S^2}{\sigma^2} + \left(\frac{\bar{X} - \mu}{\sigma/\sqrt{n}}\right)^2 $$
令 $Z_i = \frac{X_i - \mu}{\sigma}$。由于 $X_i \sim N(\mu, \sigma^2)$ 且相互独立，则 $Z_i \sim N(0, 1)$ 且相互独立。
根据卡方分布的定义，$\sum_{i=1}^{n}Z_i^2$ 服从自由度为 $n$ 的卡方分布，即 $\chi^2(n)$。
同时，由于 $\bar{X} \sim N(\mu, \sigma^2/n)$，则 $\frac{\bar{X} - \mu}{\sigma/\sqrt{n}} \sim N(0, 1)$。所以 $\left(\frac{\bar{X} - \mu}{\sigma/\sqrt{n}}\right)^2$ 服从自由度为 1 的卡方分布，即 $\chi^2(1)$。

因此，我们可以将上述等式写为：
$$ \chi^2(n) = \frac{(n-1)S^2}{\sigma^2} + \chi^2(1) $$
根据 Fisher's Theorem (或 Cochran's Theorem)，在正态总体条件下，$\bar{X}$ 和 $S^2$ 是相互独立的。这同时也意味着 $\frac{(n-1)S^2}{\sigma^2}$ 和 $\left(\frac{\bar{X} - \mu}{\sigma/\sqrt{n}}\right)^2$ 是相互独立的。

由于 $\chi^2(n) = \chi^2(n-1) + \chi^2(1)$ 的可加性，且 $\chi^2(1)$ 部分是独立于 $\frac{(n-1)S^2}{\sigma^2}$ 的，因此可以推断出 $\frac{(n-1)S^2}{\sigma^2}$ 必须服从自由度为 $n-1$ 的卡方分布。

所以，我们得出结论：
$$ \frac{(n-1)S^2}{\sigma^2} \sim \chi^2(n-1) $$
且 $\bar{X}$ 和 $S^2$ 相互独立。

**证毕。**


















![[第六章+数理统计的基本概念.pdf#page=4&rect=119,101,172,120&color=yellow|第六章+数理统计的基本概念, p.4]]
**定理：** 设 $X_1, X_2, \dots, X_n$ 是从总体 $X$ 中抽取的容量为 $n$ 的一个简单随机样本，且 $E(X) = \mu$ 和 $Var(X) = \sigma^2$ 存在。记样本均值 $\bar{X} = \frac{1}{n}\sum_{i=1}^{n}X_i$ 和样本方差 $S^2 = \frac{1}{n-1}\sum_{i=1}^{n}(X_i - \bar{X})^2$。则 $S^2$ 是总体方差 $\sigma^2$ 的无偏估计量，即 $E(S^2) = \sigma^2$。

**证明：**

我们的目标是证明 $E(S^2) = \sigma^2$。

根据样本方差的定义：
$$ S^2 = \frac{1}{n-1}\sum_{i=1}^{n}(X_i - \bar{X})^2 $$

首先，我们对求和项 $\sum_{i=1}^{n}(X_i - \bar{X})^2$ 进行代数变换。我们将 $X_i - \bar{X}$ 表示为 $(X_i - \mu) - (\bar{X} - \mu)$：(理论证明这里必须使用$\mu$)
$$ \sum_{i=1}^{n}(X_i - \bar{X})^2 = \sum_{i=1}^{n}[(X_i - \mu) - (\bar{X} - \mu)]^2 $$
展开平方项：
$$ = \sum_{i=1}^{n}[(X_i - \mu)^2 - 2(X_i - \mu)(\bar{X} - \mu) + (\bar{X} - \mu)^2] $$
利用求和的线性性质，将各项分开：
$$ = \sum_{i=1}^{n}(X_i - \mu)^2 - 2\sum_{i=1}^{n}(X_i - \mu)(\bar{X} - \mu) + \sum_{i=1}^{n}(\bar{X} - \mu)^2 $$
简化中间项和最后一项：
* 对于中间项，由于 $(\bar{X} - \mu)$ 对于求和符号是常数，可以提到外面：
    $$ -2\sum_{i=1}^{n}(X_i - \mu)(\bar{X} - \mu) = -2(\bar{X} - \mu)\sum_{i=1}^{n}(X_i - \mu) $$
    我们知道 $\sum_{i=1}^{n}(X_i - \mu) = \sum_{i=1}^{n}X_i - \sum_{i=1}^{n}\mu = n\bar{X} - n\mu = n(\bar{X} - \mu)$。
    所以，中间项变为：
    $$ -2(\bar{X} - \mu) \cdot n(\bar{X} - \mu) = -2n(\bar{X} - \mu)^2 $$
* 对于最后一项，$(\bar{X} - \mu)^2$ 对于求和符号也是常数：
    $$ \sum_{i=1}^{n}(\bar{X} - \mu)^2 = n(\bar{X} - \mu)^2 $$
将这些代入展开式：
$$ \sum_{i=1}^{n}(X_i - \bar{X})^2 = \sum_{i=1}^{n}(X_i - \mu)^2 - 2n(\bar{X} - \mu)^2 + n(\bar{X} - \mu)^2 $$
合并同类项：
$$ \sum_{i=1}^{n}(X_i - \bar{X})^2 = \sum_{i=1}^{n}(X_i - \mu)^2 - n(\bar{X} - \mu)^2 $$

现在，我们对这个结果取期望：
$$ E\left[\sum_{i=1}^{n}(X_i - \bar{X})^2\right] = E\left[\sum_{i=1}^{n}(X_i - \mu)^2 - n(\bar{X} - \mu)^2\right] $$
利用期望的线性性质：
$$ = E\left[\sum_{i=1}^{n}(X_i - \mu)^2\right] - E\left[n(\bar{X} - \mu)^2\right] $$
$$ = \sum_{i=1}^{n}E[(X_i - \mu)^2] - nE[(\bar{X} - \mu)^2] $$

分别计算这两个期望项：
* 对于第一项：根据方差的定义，$E[(X_i - \mu)^2] = Var(X_i)$。由于 $X_i$ 是从总体中抽取的，其方差等于总体方差 $\sigma^2$。
    $$ \sum_{i=1}^{n}E[(X_i - \mu)^2] = \sum_{i=1}^{n}\sigma^2 = n\sigma^2 $$
* 对于第二项：$E[(\bar{X} - \mu)^2] = Var(\bar{X})$。我们知道样本均值的方差为 $Var(\bar{X}) = \frac{\sigma^2}{n}$。
    $$ nE[(\bar{X} - \mu)^2] = n \cdot Var(\bar{X}) = n \cdot \frac{\sigma^2}{n} = \sigma^2 $$

将这两个结果代回 $E\left[\sum_{i=1}^{n}(X_i - \bar{X})^2\right]$ 的表达式中：
$$ E\left[\sum_{i=1}^{n}(X_i - \bar{X})^2\right] = n\sigma^2 - \sigma^2 = (n-1)\sigma^2 $$

最后，我们回到 $E(S^2)$：
$$ E(S^2) = E\left[\frac{1}{n-1}\sum_{i=1}^{n}(X_i - \bar{X})^2\right] $$
将前面的结果代入：
$$ E(S^2) = \frac{1}{n-1} E\left[\sum_{i=1}^{n}(X_i - \bar{X})^2\right] = \frac{1}{n-1} (n-1)\sigma^2 = \sigma^2 $$

**证毕。**












![[第七章+点估计与估计量的评价.pdf#page=1&rect=86,381,178,405&color=yellow|第七章+点估计与估计量的评价, p.1]]

在统计学中，**点估计**是指用样本的统计量来估计总体的未知参数。例如，用样本均值 $\bar{X}$ 来估计总体均值 $\mu$，用样本方差 $S^2$ 来估计总体方差 $\sigma^2$。

**估计量 (Estimator)**：用于估计总体参数的统计量，通常用 $\hat{\theta}$ 表示。
**估计值 (Estimate)**：将具体样本数据代入估计量后计算出的数值。














![[第七章+点估计与估计量的评价.pdf#page=5&rect=85,562,250,588&color=yellow|第七章+点估计与估计量的评价, p.5]]

评价一个点估计量的好坏，主要考虑以下几个性质：

无偏性 (Unbiasedness)

* **定义**：如果估计量 $\hat{\theta}$ 的期望值等于被估计的总体参数 $\theta$ 的真值，则称 $\hat{\theta}$ 是 $\theta$ 的无偏估计量。
    $$ E(\hat{\theta}) = \theta $$
* **直观理解**：在大量重复抽样中，无偏估计量的平均值会精确地落在总体参数的真值上，不会系统性地高估或低估。
* **性质**：这是**有限样本性质**，适用于任何给定的样本量。

一致性 (Consistency)

* **定义**：如果当样本容量 $n$ 趋于无穷大时，估计量 $\hat{\theta}_n$ (强调依赖于 $n$) 依概率收敛于总体参数 $\theta$ 的真值，则称 $\hat{\theta}_n$ 是 $\theta$ 的一致估计量。
    $$ \lim_{n \to \infty} P(|\hat{\theta}_n - \theta| < \epsilon) = 1, \quad \forall \epsilon > 0 $$
* **直观理解**：随着样本量的增大，一致估计量会越来越接近总体参数的真值，最终无限趋近。
* **性质**：这是**大样本性质**或**渐近性质**。

有效性 (Efficiency)

* **定义**：在所有无偏估计量中，方差最小的估计量称为**有效估计量**。方差越小，估计量的波动性越小，估计越精确。
* **性质**：通常与**克拉默-拉奥下界 (Cramer-Rao Lower Bound)** 相关联。






![[第七章+点估计与估计量的评价.pdf#page=1&rect=90,238,190,258&color=yellow|第七章+点估计与估计量的评价, p.1]]
矩估计 (Method of Moments, MoM)

* **核心思想**：用样本的经验矩（通过样本计算）来匹配总体的理论矩（由未知参数表示），然后解方程组求出参数估计值。

* **步骤**：
    1.  写出总体的理论矩（通常是前几阶原点矩或中心矩）表达式，它们是未知参数的函数。
        * $k$ 阶原点矩：$\mu_k' = E(X^k)$
    2.  计算样本的经验矩：
        * $k$ 阶样本原点矩：$M_k' = \frac{1}{n}\sum_{i=1}^{n}X_i^k$
    3.  如果总体有 $m$ 个未知参数，则令前 $m$ 阶理论矩等于对应的样本经验矩，建立 $m$ 个方程，并解出未知参数。
        * $E(X) = \frac{1}{n}\sum_{i=1}^{n}X_i$
        * $E(X^2) = \frac{1}{n}\sum_{i=1}^{n}X_i^2$
        * ...

* **例子**：估计泊松分布 $X \sim Poisson(\lambda)$ 的参数 $\lambda$。
    * 理论矩：$E(X) = \lambda$
    * 样本矩：$\bar{X} = \frac{1}{n}\sum_{i=1}^{n}X_i$
    * 令两者相等：$\hat{\lambda}_{MoM} = \bar{X}$

* **优缺点**：
    * **优点**：概念直观，计算相对简单，通常具有一致性。
    * **缺点**：不一定有效，估计值可能超出参数空间。








![[第七章+点估计与估计量的评价.pdf#page=2&rect=89,641,234,663&color=yellow|第七章+点估计与估计量的评价, p.2]]


最大似然估计 (Maximum Likelihood Estimation, MLE)

* **核心思想**：寻找使当前观测到的样本数据出现的概率（或概率密度）最大的未知参数值。

* **步骤**：
    1.  **写出似然函数 $L(\theta)$**：
        * 对于独立同分布的样本 $X_1, \dots, X_n$：
            $$ L(\theta; x_1, \dots, x_n) = \prod_{i=1}^{n} f(x_i; \theta) \quad (\text{连续型}) $$
            $$ L(\theta; x_1, \dots, x_n) = \prod_{i=1}^{n} P(X_i=x_i; \theta) \quad (\text{离散型}) $$
    2.  **取对数似然函数 $l(\theta) = \ln L(\theta)$**：这通常是为了简化计算。
        $$ l(\theta) = \sum_{i=1}^{n} \ln f(x_i; \theta) $$
    3.  **对参数求偏导并令其为零**：解似然方程，找到使 $l(\theta)$ 最大的 $\hat{\theta}_{MLE}$。
        $$ \frac{\partial l(\theta)}{\partial \theta_j} = 0, \quad \forall \theta_j $$
    4.  **验证是最大值 (可选)**：检查二阶导数或 Hessian 矩阵。

* **例子**：估计泊松分布 $X \sim Poisson(\lambda)$ 的参数 $\lambda$。
    * PMF：$P(X=x; \lambda) = \frac{e^{-\lambda}\lambda^x}{x!}$
    * 对数似然函数：
        $$ l(\lambda) = -n\lambda + (\sum_{i=1}^{n} x_i) \ln\lambda - \sum_{i=1}^{n} \ln(x_i!) $$
    * 求导并置零：
        $$ \frac{\partial l(\lambda)}{\partial \lambda} = -n + \frac{1}{\lambda}(\sum_{i=1}^{n} x_i) = 0 $$
        解得：$\hat{\lambda}_{MLE} = \bar{X}$

* **优缺点**：
    * **优点**：在大样本下通常具有优良的渐近性质（一致性、渐近无偏性、渐近有效性）。
    * **缺点**：计算可能复杂，需要知道精确的总体分布形式。

##  常用估计量的性质示例

###  样本均值 $\bar{X}$

* **是总体均值 $\mu$ 的无偏估计量**：
    $$ E(\bar{X}) = E\left(\frac{1}{n}\sum_{i=1}^{n}X_i\right) = \frac{1}{n}\sum_{i=1}^{n}E(X_i) = \frac{1}{n}\sum_{i=1}^{n}\mu = \frac{n\mu}{n} = \mu $$
* **是总体均值 $\mu$ 的一致估计量**：由大数定律保证。
* **方差**：
    $$ Var(\bar{X}) = \frac{Var(X)}{n} = \frac{\sigma^2}{n} $$

###  样本方差 $S^2$

* **是总体方差 $\sigma^2$ 的无偏估计量**：
    $$ S^2 = \frac{1}{n-1}\sum_{i=1}^{n}(X_i - \bar{X})^2 $$
    **证明 $E(S^2) = \sigma^2$：**
    $$ E(S^2) = E\left[\frac{1}{n-1}\sum_{i=1}^{n}(X_i - \bar{X})^2\right] $$
    我们先对求和项进行变换：
    $$ \sum_{i=1}^{n}(X_i - \bar{X})^2 = \sum_{i=1}^{n}[(X_i - \mu) - (\bar{X} - \mu)]^2 $$
    $$ = \sum_{i=1}^{n}(X_i - \mu)^2 - 2n(\bar{X} - \mu)^2 + n(\bar{X} - \mu)^2 $$
    $$ = \sum_{i=1}^{n}(X_i - \mu)^2 - n(\bar{X} - \mu)^2 $$
    对这个结果取期望：
    $$ E\left[\sum_{i=1}^{n}(X_i - \bar{X})^2\right] = E\left[\sum_{i=1}^{n}(X_i - \mu)^2\right] - E\left[n(\bar{X} - \mu)^2\right] $$
    $$ = \sum_{i=1}^{n}E[(X_i - \mu)^2] - nE[(\bar{X} - \mu)^2] $$
    由于 $E[(X_i - \mu)^2] = Var(X_i) = \sigma^2$ 且 $E[(\bar{X} - \mu)^2] = Var(\bar{X}) = \frac{\sigma^2}{n}$：
    $$ = \sum_{i=1}^{n}\sigma^2 - n\left(\frac{\sigma^2}{n}\right) $$
    $$ = n\sigma^2 - \sigma^2 = (n-1)\sigma^2 $$
    代回 $E(S^2)$ 的表达式：
    $$ E(S^2) = \frac{1}{n-1} E\left[\sum_{i=1}^{n}(X_i - \bar{X})^2\right] = \frac{1}{n-1} (n-1)\sigma^2 = \sigma^2 $$
* **是总体方差 $\sigma^2$ 的一致估计量。**
* **与卡方分布的关系 (若总体为正态分布 $N(\mu, \sigma^2)$)**：
    $$ \frac{(n-1)S^2}{\sigma^2} \sim \chi^2(n-1) $$


##  自由度 (Degrees of Freedom, DF)

* **概念**：在估计某个参数或进行统计检验时，可以自由变化的独立观测值的数量。
* **直观解释**：当你使用样本数据计算某个统计量时，每使用一个估计量来替换一个未知参数，就会失去一个自由度。
    * 例如，计算样本方差 $S^2$ 时，需要先计算样本均值 $\bar{X}$。一旦 $\bar{X}$ 确定，则 $n$ 个离差 $(X_i - \bar{X})$ 中只有 $n-1$ 个是独立的，因为它们的和 $\sum(X_i - \bar{X})$ 总是为零。因此，自由度为 $n-1$。
* **重要性**：自由度影响统计量的抽样分布形状（如 t 分布、卡方分布、F 分布），进而影响统计推断的准确性（如临界值和 p 值）。

---








![[第一章+随机事件和概率.pdf#page=9&rect=93,124,460,203&color=yellow|第一章+随机事件和概率, p.9]]
选D.在连续概率区间内这是可能成立的.从 $P = 0$不能推出事件为空集，因为可能会存在零概率事件，如在一条线段选中一个点，就是一个零概率事件，说明事件的概率很小很小，如事件$A$为飞镖落在$[0,0.5]$区间，事件$B$为飞镖落在$[0.5]$这个位置，就可以做到这个效果。同样，$A \subset B \implies P(AB) = P(A)$但$P(AB) = P(A) \not\implies A \subset B$。可以想象成A的大面积在B内，但是，有一些离散点在B外，而落在这些点的概率为0，所以不能推出来。概率是可能性的度量。做这类题要小心。