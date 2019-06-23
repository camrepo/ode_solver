# Examples for Numerical Differential Equation Solving
Use numerical methods to solve ordinary differential equations.
## Lotka-Volterra model
<img align="right" src="https://user-images.githubusercontent.com/31299606/59965938-ddf09f80-954f-11e9-9086-2060327ba72e.png" width=50%>
The model can be described by<br><br>

du/dt = au - bu*v<br>
dv/dt = -cv + dbu*v<br>
<br>
with the following notations:
- u: number of preys (for example, rabbits)
- v: number of predators (for example, foxes)
- a, b, c, d are constant parameters defining the behavior of the population:
    - a: the natural growing rate of rabbits, when there's no fox
    - b: the natural dying rate of rabbits, due to predation
    - c: the natural dying rate of fox, when there's no rabbit
    - d: the factor describing how many caught rabbits let create a new fox

## ODE solver
- Python
    - [scipy.integrate.odeint](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.odeint.html)
    - [scipy.integrate.ode](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.ode.html)
- Julia
    - [Sundials.jl](https://github.com/JuliaDiffEq/Sundials.jl)
    - [ODE.jl](https://github.com/JuliaDiffEq/ODE.jl)

## License
[MIT](/LICENSE)