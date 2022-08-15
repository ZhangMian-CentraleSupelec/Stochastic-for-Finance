# Stochastic in Finance

## Summary

- This project is based on the course of 3A CentraleSupélec - Stochastic in Finance. 
- This project contains 5 parts. 

### Part1. The Monte-Carlo simulation and Black-Scholes
- Implement the price of Black-Scholes and Calculate the Greeks with $S_0$
- Implement the Monte-Carlo and observe the convergence
- Verify and show the normal distribution of Monte-Carlo
- Verify and show the speed of converge

### Part2. Asian Option 
- Plot the price of the asian option with the variation of $S_0$
- Plot the price of the asian option with the variation of maturity
- Analyse the method of reduce variance for the asian option

### Part3. Numerical Method

- The method for Black-Scholes.
- The partial differential equation of the Black Scholes
- Plot the average error of the price with the variation of N
- Plot the average error of the price with the variation of M
- Plotting the point error

### Part4. Barrier Option
- Plot the price of the call option with barrier up-out with variation $S_0$
- Plot the price of the call option with maturity increase and verify the convergence.
- Plot the call option with barrier down and in.
- Analyse the variation reduction of the estimation of Monte Carlo 

### Part5. Euler Method
- Solve the Black-Scholes Equation with Euler method and Milstein method, and plot the convergence.
- Calculate the price of call with Hestion model and Euler method
- Calculate the implied volatility
- Plot the implied volatility - volatility smile with Heston method
- Decompose of the volatility smile with parameters of the volatility ( $\alpha$, $\nu$, $\rho$ )


## Presentation of the result

### Part1. The Monte-Carlo simulation and Black-Scholes

- Implement the price of Black-Scholes and Calculate the Greeks with $S_0$
![image](https://user-images.githubusercontent.com/110284601/184559743-80224e7a-7aa0-4be4-a33b-5c643f22a975.png)

- Implement the Monte-Carlo and observe the convergence
![image](https://user-images.githubusercontent.com/110284601/184559810-1eabe3bf-895e-4cde-8b4e-96d5b01ff706.png)

- Verify and show the normal distribution of Monte-Carlo
![image](https://user-images.githubusercontent.com/110284601/184559834-ca8247fb-81e1-4a18-84cf-8e12ad01c2d6.png)

```
jb_test=jarque_bera(MC_Norm)
print("The test statistic is",round(jb_test[0],4),"and the corresponding p-value is"
      ,round(jb_test[1],4),".") 
print('')
```
The test statistic is 0.1542 and the corresponding p-value is 0.9258 .

- Verify and show the speed of converge
![image](https://user-images.githubusercontent.com/110284601/184559984-768a698f-04e3-43fa-8c1f-97b3e2a8fcd7.png)

## Part2. Asian Option


