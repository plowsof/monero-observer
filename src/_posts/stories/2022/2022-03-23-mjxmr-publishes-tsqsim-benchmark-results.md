---
layout: post
category: story
title: "mjxmr publishes tsqsim benchmark results"
description: "mjxmr has published the benchmark results for the Time Series Quick Simulator (tsqsim) tool."
tags: research
image: tsqsim-native-cpp.png
date: 2022-03-23 21:00
---

mjxmr[^1] has published the benchmark results[^2] for his *Time Series Quick Simulator* (tsqsim)[^3] tool:

> In order to limit the strain on this quarter’s budget, I resorted to testing against only the following frameworks: statsmodels[^4], darts[^5]

The simulator was written for the Monero Research Lab[^6] in order to predict the number of near future transactions.

> Below are the results of the benchmark against the (almost) equivallent native C++ implementation of the AutoRegressive (AR) model with lags of 2.

### Results

```
Benchmarked 'py_statsmodels.py' Time taken = 10.922s Ratio Pred2Base     = 0.705 [===       ] (the lower the better) 
Benchmarked 'py_darts.py'   Time taken = 14.307s Ratio Pred2Base     = 0.711 [===       ] 
Benchmarked 'Native C++'    Time taken = 0.144s  Ratio Pred2Base     = 0.68  [===       ]
```

Benchmark images and steps to reproduce the experiment are included in the Reddit thread[^2].

According to fellow researcher Rucknium[^7], the results show an *almost two orders of magnitude speedup*[^8].

To learn more about mjxmr’s work, consult my previous report[^9]. You can support his continued work on Monero by donating to his CCS proposal[^10].

---

[^1]: https://github.com/mj-xmr
[^2]: [https://libredd.it/tl5w1b/](https://libredd.it/tl5w1b/){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/mj-xmr/tsqsim
[^4]: https://www.statsmodels.org/
[^5]: https://github.com/unit8co/darts
[^6]: https://github.com/monero-project/research-lab
[^7]: https://github.com/rucknium
[^8]: https://libredd.it/r/Monero/comments/tl5w1b/tsqsims_benchmark_new_tool_designed_for_monero/i1u372t/?context=3
[^9]: [/mjxmr-replacement-ccs-proposal-q2-2022/](/mjxmr-replacement-ccs-proposal-q2-2022/)
[^10]: [/mjxmr-ccs-proposal-q2-2022-ready-funding/](/mjxmr-ccs-proposal-q2-2022-ready-funding/)
