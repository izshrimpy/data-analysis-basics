import matplotlib.pyplot as plt
import numpy as np
class HeightsCalculator:
def __init__(self, heights, labels):
self.heights = heights # [600, 470, 170, 430, 300]
self.labels = labels # [1, 2, 3, 4, 5]
def get_sum(self, terms: list) -> int:
sum = 0
for index in range(0, len(terms)):
sum = sum + terms[index]
return sum
def get_average(self, sum: int, number_of_terms: int) -> int:
return sum / number_of_terms
def get_variance(self, heights: list, average: int) -> int:
variance = 0
for index in range(0, len(heights)):
variance = variance + (heights[index] - average) ** 2
return variance / len(heights)
def get_std(self, variance: int) -> int:
return variance ** (1 * 0.5)
def get_scatter_plot(self):
X = np.array(self.heights)
Y = np.array(self.labels)
plt.scatter(Y, X)
plt.show()
def print_std(self):
print(
self.get_std(
self.get_variance(
self.heights,
average=self.get_average(
self.get_sum(terms=self.heights),
number_of_terms=len(self.heights),
),
)
)
)
dog_heights_calculator = HeightsCalculator(
heights=[600, 470, 170, 430, 300], labels=[1, 2, 3, 4, 5]
)
dog_heights_calculator.get_scatter_plot()
