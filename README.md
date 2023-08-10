# newborn
newby design
pip install matplotlib

import numpy as np
import matplotlib.pyplot as plt

# Tạo dữ liệu mẫu
x = np.linspace(0, 10, 100)
y1 = np.sin(x)
y2 = np.cos(x)
y3 = np.exp(-x/5) * np.cos(2*x)
y4 = np.random.normal(0, 0.2, 100) + y1

# Vẽ đồ thị phức tạp
plt.figure(figsize=(10, 6))

plt.plot(x, y1, label='sin(x)', color='blue')
plt.plot(x, y2, label='cos(x)', color='red')
plt.plot(x, y3, label='exp(-x/5) * cos(2x)', color='green')
plt.scatter(x, y4, label='random + sin(x)', color='purple', marker='o')

plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Complex Graph Example')
plt.legend()

plt.grid(True)
plt.show()
