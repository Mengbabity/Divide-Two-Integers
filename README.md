# Divide-Two-Integers

问题：作除法。

解决：开始的想法是 将初始值赋为除数，大于被除数--，小于被除数++（正数），但每次加1减1效果太慢。
     首先对正数负数设置一个flag，返回结果时用到。
     当除数大于等于被除数的时候，若被除数大于除数*2（即左移一位），除数*2，且计数器*2，计数器记录做乘法的次数。
     小于的话，被除数-已经乘过的除数之积作为新的被除数，继续新一轮计算。
