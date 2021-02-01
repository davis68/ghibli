# ghibli
Studio Ghibli-inspired color palettes for Python's MatPlotLib

Inspired by [`ewenme`'s `ghibli` package](https://ewenme.github.io/ghibli/index.html) for R/`ggplot2`.  Original palettes from [Movies in Color](http://moviesincolor.com/).

Usage:

```py
import matplotlib as mpl
import matplotlib.pyplot as plt
import numpy as np
import ghibli
ghibli.set_palette('LaputaMedium')

x = np.linspace(-5,+5,101)
y1 = np.sin(x)
y2 = np.cos(x)
y3 = np.tan(x)
y4 = np.sinh(x)
y5 = np.cosh(x)
y6 = np.tanh(x)
y7 = np.exp(x)

plt.plot(x,y1,linewidth=1)
plt.plot(x,y2,linewidth=2)
plt.plot(x,y3,linewidth=3)
plt.plot(x,y4,linewidth=4)
plt.plot(x,y5,linewidth=5)
plt.plot(x,y6,linewidth=6)
plt.plot(x,y7,'o')

plt.show()
```
