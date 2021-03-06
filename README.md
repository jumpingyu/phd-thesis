博士学位论文 | Ph.D. Thesis
===========================

标题 | Title
------------
* SKA EoR 探测实验的射电晕前景建模以及 EoR 信号分离算法的研究
* A Study of Foreground Modeling of Radio Halos and
  EoR Signal Separation Method for the SKA EoR Experiment

作者 | Author
-------------
* 李维天
* Weitian Li

导师 | Advisor
--------------
* 徐海光
* Haiguang Xu

专业 | Major
------------
* 物理学
* Physics

单位 | Institution
------------------
* 上海交通大学, 物理与天文学院
* School of Physics and Astronomy, Shanghai Jiao Tong University

日期 | Date
-----------
* 2019 年 9 月 6 日
* September 6, 2019

许可证 | License
----------------
* 知识共享协议 -- 署名 4.0 国际 (CC BY 4.0)
* Creative Commons -- Attribution 4.0 International (CC BY 4.0)

关键词 | Key words
------------------
* 低频射电天文 (low-frequency radio astronomy)
* 再电离时期 (epoch of reionization)
* 射电晕 (radio halo)
* 微弱信号分离 (week signal separation)
* 深度学习 (deep learning)

摘要
----
再电离时期 (Epoch of Reionization, EoR) 是宇宙演化早期尚不为人所透彻了解的一个
重要时期，从宇宙大爆炸之后约 3 亿年延续到约 10 亿年，对应的红移范围约为 6–15。
第一代恒星和星系在这个时期刚形成不久，产生紫外和软 X 射线辐射使中性重子物质逐
渐被再次电离。研究 EoR 对于理解第一代天体和宇宙早期结构的形成具有重要意义，是
建立完整的宇宙演化图景的关键之一。在低频射电波段 (~50–200 MHz) 探测源自 EoR 的
中性氢 21 cm 谱线是目前已提出的研究该时期的最直接和有效的办法。然而，由于 EoR
信号非常微弱，且淹没在比它强约 4–5 个数量级的前景干扰之中，因此在研究 EoR 时必
须深刻理解各个前景干扰成分的性质，研发具有针对性的前景扣除和 EoR 信号分离算法。

在多种 EoR 前景干扰成分中，银河系同步辐射和自由—自由辐射、河外点源等几种主要成
分，已被较广泛地研究过，它们的低频辐射特征以及对 EoR 探测的干扰行为已经基本被
弄清楚。另一方面，星系团射电晕作为一类较常⻅的河外射电展源，也将对 EoR 信号探
测产生一定程度的影响。在以往的前景研究中，只有很少几项工作比较简单地触及了射电
晕的低频射电辐射。这些工作对射电晕图像和频谱的建模过于简化，而且未进一步分析射
电晕辐射对 EoR 信号探测的具体影响。因此，针对 EoR 探测实验的前景干扰和信号分离
难题，本文分两个方面开展研究：首先是对射电晕的低频射电辐射特征进行更完善、更物
理的建模，构建更逼真的前景模型，并在考虑 SKA1-Low 阵列仪器效应的前提下评估射电
晕辐射对 EoR 信号探测的影响；其次是利用改进的前景模型，基于深度学习研发微弱信
号分离算法，用于分离 EoR 信号和前景干扰。

基于 Press–Schechter 理论和湍流再加速模型，实现了针对射电晕形成和演化过程的完
整建模，并据此生成了射电晕的模拟天图，再利用目前最新的 SKA1-Low 阵列布局模拟了
包含仪器效应的 SKA1-Low 射电晕图像。通过在 120–128、154–162 和 192–200 MHz 三个
频带内比较射电晕和 EoR 信号的一维功率谱，发现在 0.1 Mpc^{−1} < k < 2 Mpc^{−1}
(约对应于 1.2' < s < 24') 尺度范围射电晕在三个频带内的典型功率分别约为 EoR 信
号的 10000、1000 和 300 倍。同时通过研究二维功率谱以及 EoR 窗口发现，
在 0.5 Mpc^{−1} ≲ k ≲ 1 Mpc^{−1} (约对应于 2.4' ≲ s ≲ 4.8') 尺度范围以及 68%
误差范围内，射电晕辐射与 EoR 信号的功率比在三个频带内分别可达约 230–800%、
18–95% 和 7–40%。这说明射电晕辐射在 EoR 窗口内所泄漏的功率是不可忽略的——尤其在
~120 MHz 的较低频率更为显著。此外，我们还发现仪器响应所产生的频谱伪结构会显著
增强射电晕辐射在 EoR 窗口内的泄漏，而且旁瓣里的射电晕辐射使这个问题更加严重。
这些结果说明射电晕是一个此前尚未引起充分重视的前景干扰成分，需要在 EoR 观测中
认真对待。

基于上述改进的前景模型以及模拟的 SKA1-Low 图像，进一步研究了干涉阵列波束效应对
前景辐射频谱光滑性的影响。干涉阵列波束的频率依赖效应会使原本光滑的前景频谱产生
快速变化的起伏，损坏频谱的光滑性，导致传统前景扣除方法不再适用。为了解决这个问
题，我们基于深度学习方法设计了一个包含 9 个卷积层的卷积去噪自编码器
(Convolutional Denoising AutoEncoder, CDAE) 用来分离 EoR 信号。使用模拟的
SKA1-Low 图像进行训练和测试，发现由 CDAE 重建的 EoR 信号与输入的 EoR 信号之间
的相关系数达到 ξ\_{cdae} = 0.929 ± 0.045，即表明 CDAE 准确地分离了 EoR 信号。
与此相比，传统的多项式拟合法和连续小波变换法在分离 EoR 信号时并不成功，分别仅有
ξ\_{poly} = 0.296 ± 0.121 和 ξ\_{cwt} = 0.198 ± 0.160。因此，CDAE 能够有效克服
波束效应对前景辐射频谱光滑性的破坏，并且准确地分离 EoR 信号，反映了深度学习方
法在未来 EoR 实验中的潜在重要作用。

Abstract
--------
The epoch of reionization (EoR) is an important stage in the early Universe
that is expected to last from about 300 Myr to 1 Gyr after the Big Bang,
corresponding to a redshift range of about 6–15. During the EoR, the first
stars and galaxies have just formed and start emitting ultraviolet and soft
X-ray photons, which gradually reionize the surrounding neutral baryonic
matter. Studying the EoR is invaluable in understanding the properties of the
first stars and galaxies and the structure formation of the early Universe.
Among the methods to probe the EoR, detecting the 21 cm line of neutral
hydrogen originating from the EoR in the low-frequency radio band (~50–200 MHz)
is regarded as the most promising and effective method.  However, the EoR
signal is extremely faint and is buried in the overwhelming foreground
contamination of about 4–5 orders of magnitude stronger. Therefore, it is
indispensable to comprehend every foreground component and to develop specific
foreground removal and EoR signal separation methods.

Among various foreground components, the Galactic synchrotron and free–free
radiations and the extragalactic point sources are the major components and
have been rather extensively investigated in the literature. Their
low-frequency radio properties and contamination on the EoR detection are
basically understood.  On the other hand, radio halos in galaxy clusters, which
are common extragalactic extended sources, are also expected to have an impact
on the EoR signal detection.  However, only several works that investigate the
EoR foreground have preliminarily explored radio halos. Those works made
oversimplifications in simulating the images and spectra of radio halos and did
not further analyze the impacts of radio halo emission on the EoR detection. In
this work, we carry out two studies concerning the EoR foreground contamination
and signal separation problems. First, we construct a more complete and
physical model for simulating the radio halo emission and build a more
realistic foreground model. By taking into account the SKA1-Low instrument
effects, we evaluate the contamination of radio halo emission on the EoR signal
detection. Secondly, based on the improved foreground model, we develop a new
EoR signal separation method by utilizing the deep learning algorithms, in
order to achieve accurate separation of the EoR signal.

By employing the Press–Schechter formalism and the turbulent re-acceleration
theory, we model the formation and evolution of radio halos and simulate their
sky maps in the low-frequency band. Then, we adopt the latest SKA1-Low layout
configuration and simulate the SKA1-Low images of radio halos with instrument
effects incorporated. By comparing the one-dimensional power spectra of radio
halos and the EoR signal in the 120–128, 154–162, and 192–200 MHz frequency
bands, we find that radio halos are generally about 10000, 1000, and 300 times
more luminous than the EoR signal on scales of 0.1 Mpc^{−1} < k < 2 Mpc^{−1}
(corresponding to scales of about 1.2' < s < 24') in the three bands,
respectively. After examining the two-dimensional power spectra inside the
appropriately defined EoR windows, we find that the power leaked by radio halos
can still be significant, as the power ratios of radio halos to the EoR signal
on scales of 0.5 Mpc^{−1} ≲ k ≲ 1 Mpc^{−1} (corresponding to scales of about
2.4' ≲ s ≲ 4.8') can be up to about 230–800%, 18–95%, and 7–40% in the three
bands, when the 68% uncertainties caused by the variation of the number density
of bright radio halos are considered. Furthermore, we find that frequency
artifacts resulted from instrument response can remarkably increase the power
leakage of radio halos in the EoR window, which becomes more severe due to the
radio halos located inside the side-lobes. These results show that radio halos
are severe foreground sources and need serious treatments in future EoR
experiments.

Based on the improved foreground model and simulated SKA1-Low images obtained
above, we further investigate the beam effects of interferometers and their
impacts on the spectral smoothness of the foreground emission. The
frequency-dependent beam effects will cause rapid fluctuations along the
frequency dimension and damage the spectral smoothness of the foreground
emission, which makes traditional foreground removal methods inapplicable. To
address this issue, we propose a deep-learning-based method that employs a
9-layer convolutional denoising autoencoder (CDAE) to separate the EoR signal.
After being trained and tested on the simulated SKA1-Low images, the CDAE
achieves excellent performance as the mean correlation coefficient between the
reconstructed and input EoR signals reaches ξ\_{cdae} = 0.929 ± 0.045. In
comparison, the two representative traditional methods, namely the polynomial
fitting method and the continuous wavelet transform method, both have
difficulties in modeling and removing the foreground emission that is
complicated with the beam effects, yielding only ξ\_{poly} = 0.296 ± 0.121 and
ξ\_{cwt} = 0.198 ± 0.160, respectively. In consequence, the CDAE can
effectively deal with the spectral smoothness damage caused by the beam effects
and thus accurately separate the EoR signal. This result also exhibits the
great potential of deep- learning-based methods in future EoR experiments.
