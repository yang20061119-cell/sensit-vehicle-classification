# Resume update — replace GTA project with SensIT ML

Replace the **Video Game Culture & Mechanic Analysis (GTA)** section with the block below.
Metrics are from the executed midterm notebook (stratified 80/20 holdout).

---

## English (replace GTA section)

**SensIT Vehicle Classifier — Multi-Class Machine Learning** · Oct 2026

- Built an end-to-end supervised ML pipeline in Python (pandas, scikit-learn) on OpenML SensIT-Vehicle-Combined (98,528 samples, 100 acoustic/seismic features) to classify AAV, DW, and noise
- Performed EDA (class balance ≈1:1:2, correlations, outlier screening); applied StandardScaler and SelectKBest (ANOVA F, k≈50–60) inside Pipelines to prevent leakage
- Trained and compared Logistic Regression and Random Forest with class weighting; tuned via RandomizedSearchCV and validated with stratified 5-fold CV (RF CV macro-F1 ≈ 0.83)
- Achieved **83.6% test accuracy and 0.83 macro-F1** with tuned Random Forest; reduced overfitting by constraining tree depth / leaf size while keeping competitive generalization
- Analyzed confusion matrices and top ANOVA-selected sensors to explain residual errors (primarily vehicle vs noise)

---

## 中文（替换电子游戏分析条目）

**SensIT 车辆分类器——多类机器学习** · 2026.10

- 使用 Python（pandas、scikit-learn）在 OpenML SensIT-Vehicle-Combined（98,528 样本、100 维声学/地震特征）上搭建端到端监督分类流水线，区分 AAV、DW 与 noise
- 完成探索性分析（类别约 1:1:2、相关性与异常值筛查）；在 Pipeline 中使用 StandardScaler 与 SelectKBest（ANOVA F，k≈50–60）特征选择，避免信息泄漏
- 训练并对比逻辑回归与随机森林（class_weight 处理不平衡）；通过 RandomizedSearchCV 调参，并以分层 5 折交叉验证评估（RF CV 宏 F1 ≈ 0.83）
- 调参后随机森林达到 **测试准确率 83.6%、宏平均 F1 0.83**；通过限制树深与叶节点样本量缓解过拟合，保持稳定泛化
- 结合混淆矩阵与 ANOVA 入选特征，解释主要误差来源（车辆类别与噪声混淆）

---

## Placement tip

- Lead with **SensIT** for DS/ML roles (≈250× more rows than the Dating App project, plus CV + tuning).
- Keep Dating App as a shorter second ML bullet if space allows.
- Remove the GTA “Critical Systems Thinking” project from the one-page resume.
