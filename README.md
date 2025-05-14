## 📝 Purpose & Overview

This notebook benchmarks three statistical methods for estimating confidence intervals (CIs) of the mean on simulated right-skewed, overdispersed data.

- **Context**: Hospital length of stay for autoimmune encephalitis is often skewed and highly variable.
- **Goal**: Evaluate coverage probability and interval width of:
  - t-distribution method
  - z-distribution method
  - Bootstrap percentile method
- **Approach**: Simulate data, apply methods, and compare performance across varying sample sizes and skewness.