# HW1

The images are my Learn Git Branching progress screenshots. They were turned into greyscale with the formula `grey = 0.2125 * red + 0.7154 * green + 0.0721 * blue` and converted to txt via numpy.savetxt().

To convert the txt files back to images and look at them you can for example use matplotlib in Jupyter Notebook or Google Colab.

```python
import numpy as np
import matplotlib.pyplot as plt

main = np.loadtxt('MAIN_HW1_KRAVTSOV.txt')
remote = np.loadtxt('REMOTE_HW1_KRAVTSOV.txt')
plt.imshow(main, cmap='gray')
plt.show()
plt.imshow(remote, cmap='gray')
plt.show()
```