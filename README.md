# Stochastic in Finance

- This project is basically based on the course - Stochastic Finance of 3A CentraleSupélec.

### What we have got

The volatility surface of a call option

![image](https://user-images.githubusercontent.com/110284601/186156541-15db15f3-20b9-49f8-a29c-a48043d66975.png)

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

- Plot the price of the asian option with the variation of $S_0$.
![image](https://user-images.githubusercontent.com/110284601/184614220-aa9d567b-1738-43d9-96e8-f2da53100c21.png)

- Plot the price of the asian option with the variation of maturity.
![image](https://user-images.githubusercontent.com/110284601/184614291-52c7667a-db85-4791-b677-db8b126f8ed6.png)

- Analyse the method of reduce variance for the asian option.
      - Here we try the antithetic variable method and also control variable method.
      
```
Méthode anthitétique : 
Variance de l estimateur simple : 0.0076
Variance de l estimateur antithétique : 0.0036

Méthode de contrôle :
Variance de l estimateur simple : 0.0073
Variance de l estimateur de contrôle : 0.0074
```
## Part3. Numerical Method

- The partial differential equation of the Black Scholes
![image](https://user-images.githubusercontent.com/110284601/184615526-573d209d-f7db-4241-907a-88fce7045bd7.png)

- Plot the average error of the price with the variation of N.
![image](https://user-images.githubusercontent.com/110284601/184615575-22e77c24-7ed8-432e-bef4-671f0ae9d483.png)

- Plot the average error of the price with the variation of M.
![image](https://user-images.githubusercontent.com/110284601/184615648-791c916a-7b63-4a13-8e4e-101db667c85d.png)

- Plot the point error
![image](https://user-images.githubusercontent.com/110284601/184615684-4a6cce04-de18-4efd-b38d-f063954b50d6.png)

## Part5. Barrier Option
- Plot the price of the call option with barrier up-out with variation $S_0$
![image](https://user-images.githubusercontent.com/110284601/184615873-81eff518-1d27-4a6b-b50d-055fc913df4c.png)

- Plot the price of the call option with maturity increase and verify the convergence.
![image](https://user-images.githubusercontent.com/110284601/184615886-29e2a892-79d7-4d47-84f2-0e73546f413c.png)

- Plot the call option with barrier down and in.
![image](https://user-images.githubusercontent.com/110284601/184615922-27a7c3e9-775e-4652-ac21-fdab2ab7f833.png)

- Analyse the variation reduction of the estimation of Monte Carlo 
```
Variance de l estimateur du prix Call DI MC : 180.2655
Variance de l estimateur du prix Call DI MC Conditionnel : 5.9573
```
## Part6. Euler Method
- Solve the Black-Scholes Equation with Euler method and Milstein method, and plot the convergence.
![image](https://user-images.githubusercontent.com/110284601/184616260-f2291fd5-e52e-4404-ab7a-834a2f60623f.png)

- Calculate the price of call with Hestion model and Euler method
![image](https://user-images.githubusercontent.com/110284601/184616302-860f8146-540c-4a6a-8034-46e572434a07.png)

- Calculate the implied volatility
![image](https://user-images.githubusercontent.com/110284601/184616339-11992223-d4ee-4e85-8c8f-ce699ac9ee2c.png)

- Plot the implied volatility - volatility smile with Heston method
![image](https://user-images.githubusercontent.com/110284601/184616375-618dd169-9d32-49ac-bf05-51412aa88997.png)
![image](https://user-images.githubusercontent.com/110284601/184616399-5e8dc5fd-f998-4ad6-9087-1e5cf6edc8bc.png)

- Decompose of the volatility smile with parameters of the volatility ( $\alpha$, $\nu$, $\rho$)
![image](https://user-images.githubusercontent.com/110284601/184616683-4ec32223-ce47-419f-a090-58307da88a2c.png)
![image](https://user-images.githubusercontent.com/110284601/184616448-a6ebeb11-6f92-44bf-9e17-83665830db25.png)
![image](https://user-images.githubusercontent.com/110284601/184616478-f7097415-aae6-429a-a8e7-f03ccfd8bab0.png)
![image](https://user-images.githubusercontent.com/110284601/184616497-79702596-39c4-4ed7-9732-d22d5ebd8de3.png)
