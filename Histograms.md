```python
import numpy as np
import matplotlib.pyplot as plt
data = {
    "QL": 0.000056,
    "Jupter": 0.017,
    "Colab": 0.7,
  
}
strings = list(data.keys())
numbers = list(data.values())

plt.bar(strings, numbers)
plt.xticks(np.arange(len(strings)), strings)

plt.xlabel("platform")
plt.ylabel("time(S)")
plt.title("Execution times of einsum")
plt.show()
```


    
![png](output_0_0.png)
    



```python
import numpy as np
import matplotlib.pyplot as plt
data = {
    "QL": 0.00012,
    "Jupter": 0.015,
    "Colab": 0.14,
  
}
strings = list(data.keys())
numbers = list(data.values())

plt.bar(strings, numbers)
plt.xticks(np.arange(len(strings)), strings)

plt.xlabel("platform")
plt.ylabel("time(s)")
plt.title("Execution times of numpy")
plt.show()
```


    
![png](output_1_0.png)
    



```python
import numpy as np
import matplotlib.pyplot as plt
data = {
    "QL": 8.8,
    "Jupter": 16,
    "Colab": 9.3,
  
}
strings = list(data.keys())
numbers = list(data.values())

plt.bar(strings, numbers)
plt.xticks(np.arange(len(strings)), strings)

plt.xlabel("platform")
plt.ylabel("time(micro seconds)")
plt.title("Execution times of for loop")
plt.show()
```


    
![png](output_2_0.png)
    



```python
import numpy as np
import matplotlib.pyplot as plt
data = {
    "For loope": 8.8,
    "einsum": 56,
    "numpy": 120,
  
}
strings = list(data.keys())
numbers = list(data.values())

plt.bar(strings, numbers)
plt.xticks(np.arange(len(strings)), strings)

plt.xlabel("function")
plt.ylabel("time(micro seconds)")
plt.title("Execution times of different implementations on QL")
plt.show()
```


    
![png](output_3_0.png)
    



```python
import numpy as np
import matplotlib.pyplot as plt
data = {
    "For loop": 2.69,
    "einsum inner": 2.77,
    "einsum outer": 2.96,
    "numpy inner": 2.36,
    "numpy outer": 3.29
  
}
strings = list(data.keys())
numbers = list(data.values())

plt.bar(strings, numbers)
plt.xticks(np.arange(len(strings)), strings)

plt.xlabel("function")
plt.ylabel("time(micro seconds)")
plt.title("Execution times using timeit on jupyter ")
plt.show()
```


    
![png](output_4_0.png)
    



```python

```
