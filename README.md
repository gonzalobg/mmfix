C++ Memory Model Litmus tests
============================

Collection of C++ Memory Model litmus tests in `.litmus` format and reference memory models in `.cat`.

# References

- [models/rc11.cat](./models/rc11.cat): sourced from [herd], originally written by Simon Colin.
- [tests/popl15](./tests/popl15): sourced from [herd], originally from: Viktor Vafeiadis, Thibaut Balabonski, Soham Chakraborty, Robin Morisset, and Francesco Zappa Nardelli, _Common Compiler Optimisations are Invalid in the C11 Memory Model and what we can do about it_, POPL '15.
- [tests/herd](./tests/herd): sourced from [hers].
- [tests/pldi17](./tests/pld17): Ori Lahav, Viktor Vafeiadis, Jeehoon Kang, Chung-Kil Hur, and Derek Dreyer, _Repairing sequential consistency in C/C++11_, PLDI '17.
- [tests/dat3m](./tests/dat3m): sourced from Dartagnan's test suite at [Dat3M](https://github.com/hernanponcedeleon/Dat3M).
- [tests/cpp17]: sourced from Hans Boehm, Olivier Giroux, and Viktor Vafeiades, [P0982R1: Weaken Release Sequences](https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0982r1.html), 2018.
- [tests/paul_oota]: https://github.com/paulmckrcu/oota/tree/master/litmus

[herd]: https://github.com/herd/herdtools7

TODO:
- Add more tests:
  - https://github.com/rymrg/rocker/tree/popl21/examples
  - https://github.com/rymrg/rocker/tree/pldi19/examples/submission
  - Bridging the Gap between Programming Languages and Hardware Weak Memory Models
  - mp-release-sequence-store-and-external-store.litmus should not be accepted by rc11? need to talk with Ori
- Include new lb shapes (from LICM, MRD, ...)
