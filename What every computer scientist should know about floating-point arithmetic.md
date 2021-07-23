---
bibtex: @article{goldberg1991every,
  title={What every computer scientist should know about floating-point arithmetic},
  author={Goldberg, David},
  journal={ACM computing surveys (CSUR)},
  volume={23},
  number={1},
  pages={5--48},
  year={1991},
  publisher={ACM New York, NY, USA}
}
---

# What every computer scientist should know about floating-point arithmetic

> Squeezing infinitely many real numbers into a finite number of bits requires an approximate representation. Although there are infinitely many integers, in most programs the result of integer computations can be stored in 32 bits. In contrast, given any fixed number of bits, P = 24, the decimal number 0.1 cannot most calculations with real numbers will produce quantities that cannot be exactly represented using that many bits. (p6)

>  The IEEE standard goes further than just requiring the use of a guard digit. It gives an algorithm for addition, subtrac- tion, multiplication, division, and square root and requires that implementations produce the same result as that algo- rithm. Thus, when a program is moved from one machine to another, the results of the basic operations will be the same in every bit if both machines support the IEEE standard.  (p6)

> There are two reasons why a real number might not be exactly representable as a floating-point number. The most common situation is illustrated by the decimal number 0.1. Although it has a finite decimal representation, in binary it has an infinite repeating representation.  (p7)

Different processors can compute FPNs differently. The IEEE standard requires identical implementation for `+, -, *, /`.

Other operations can produce NaNs ... inf + -inf, 0 * inf, 0/0, inf/inf, sqrt(-1), inf mod y.

For the equality sqrt(1/z) = 1/sqrt(z), computed answers match analytic answers when z > 0. When z < 0, computed answers diverge from analytic ones.

> Probably the most interesting use of signed zero occurs in complex arithmetic. As an example, consider the equation ~ = ~/&. This is certainly true when z = O.If z = —1. the obvious computation gives ~~ = ~ = i and I/n= I/i = –i. Thus, ~#1/W ! The problem can be traced to the fact that square root is multivalued, and there is no way to select the values so they are continuous in the entire complex plane. (23)

