# Matplotlib

- It is the single most used package for 2-D graphics. It provides a very quick way to visualize data

## IPython

- Enhanced interactive Python shell
- Allows matplotlib sessions to have Matlab functionality

## pyplot

- Interface to the matplotlib library

## Simple Plot

- `import numpy as np`
  - `X = np.linspace(-np.pi, np.pi, 256, endpoint=True)`
  - `C, S = np.cos(X), np.sin(X)`

## Changing colors and line widths

- `plt.figure(figsize=(10,6), dpi=80)`
- `plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-")`
- `plt.plot(X, S, color="red", linewidth=2.5, linestyle="-")`

## Setting Limits

- `plt.xlim(X.min()*1.1, X.max()*1.1)`
- `plt.ylim(C.min()*1.1, C.max()*1.1)`

## Setting ticks

- `plt.xticks([num, num, 0, num, num])`
- `plt.yticks([num, num, 0, num, num])`

## Adding a legend

- `plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-", label="label")`
- `plt.plot(X, S, color="red", linewidth=2.5, linestyle="-", label="label")`
- `plt.legend(loc='upper left', frameon=False)`

## Annotate some points

- `plt.annotate()`

## Types of Plots

1. Regular Plot
2. Scatter Plot
3. Bar Plot
4. Contour Plot
5. IMSHOW
6. Quiver Plot
7. Pie Chart
8. Grid
9. Multiplot
10. Polar Axis
11. 3D Plots
12. Text
13. Regular Plots

# Useful Links

- [Matplotlib Tutorial](https://github.com/rougier/matplotlib-tutorial)