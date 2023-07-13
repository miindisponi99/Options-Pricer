# Options Pricing Application
## Instructions
The application is triggered from the ""Start here"" button.<br>
After inserting the user name, the application asks the user if he/she is ready to price the option.<br>
If the answer is yes, the userform appears. From here the user must imput the requirements to price the option, which in the case of Black-Scholes pricing model are:
- Stock price (S0)
– Strike price (K)
– Risk-free rate (r)
– Time (t)
– Volatility (sigma)
– Option type
– Call/put
– Option model
<br>
To use the Montecarlo simulation pricing model, the N° of iterations must be added. Moreover, to use the Binomial pricing model, the N° of steps must be added too.<br>
To remember the option underlying the user is pricing, it is possible to write on the first box the ticker name.<br>
All these values and the Option Price calculated will be stored, in column, in the same worksheet so that the user can look at the historical calculations performed.<br>
On the same worksheet, by clicking on the button "Greeks" it is possible to calculate the greeks of the option, so that the user can have a better understanding on the value of the option.<br>
Furthermore, the user, by clicking on the "At/out/in-the-money" button, can display on the table the option moneyness.
You can even switch to another UserForm by clicking the button "Switch".<br><br>

## Description
The Option Pricing Application allows to price options using three different methods:<br>
The Black-Scholes, the Montecarlo simulation, and the Binomial models.<br>
The Black-Scholes pricing model requires the following inputs:
– Stock price (S0): set always greater than zero
– Strike price (K): set always greater than zero
– Risk-free rate (r): set always greater than zero, must be written as number between 0 and 1 as it is a percentage figure
– Time (t): set always greater than zero, must be written in years term (for example for 18 months write 1.5)
– Volatility (sigma): set always greater than zero, must be written as number between 0 and 1 as it is a percentage figure
– Option type: is the option European or American? In other words, does it allow to exit the position prior to expiration (American) or not (European)?
– Call/put: the call option is set as default, if the user wants to price a put option, "Put" must be written instead.
– Option model: Black-Scholes, Montecarlo, Binomial
<br><br>

## Models
__Below a brief description of the three different models that can be used in the Option Pricer application.__
The Black-Scholes model is based on a specific formula and therefore it determines the price of the option by giving the specific inputs above described. However, this formula can only compute the European option price as the expiration at maturity of the option is embedded in the formula and therefore does not allow to price American options, which can be exercised before the option maturity.<br>
To use the Montecarlo simulation pricing model, the N° of iterations must be added in the inputs, as it is part of the iterative process present in the model. The iteration is indeed the essence of this pricing model, which by randomly creating stock prices allows for a more "empirical" option price result.<br>
To use the Binomial pricing model, the N° of steps must be added too. This is because, as the Montecarlo simulation, this model uses an iterative procedure, defined by how many times to reiterate the process (N° of steps) which ultimately change the final result.
<br><br>

## Steps to follow to price the option
The first step to price the option is to go to the worksheet "Pricer". The user can also click on the above button to proceed faster on the page. After, the user must click the "Calculate Option Price" button, which will open a pop-up form, where the user can insert his/her name. After proceeding, the User Interface to Price Options will appear and will look like the one below. From here, the user can insert the Ticker of the option underlying, the Spot price and the Strike price of the option underlying, the risk-free rate (set in percentage), the Time to expiration (set in years), the volatility, the option type (European or American), the option model (Black-Scholes, Montecarlo, Binomial), the type (Call or Put option) and the additional N° of iterations (for the Montecarlo) and N° of steps (for the Binomial).<br>
Thereafter, the user can calculate the option price by clicking on the first button, called "Calculate option price". The calculated value will be stored in the table and the user can exit the "User interface to price Options" by clicking on the button "Close User Interface". If, however, the user wants to calculate additional information such as option Greeks, implied volatility or wants to have a look at the option graph payoff or if the option is In/ Out/ At-the-money, the user can click on the button called "Switch to additional info UI". Here, a new pop-up form will appear and the user can calculate the above-mentioned values by clicking on the specific buttons named "Greeks", "Implied volatility", "In/ Out/ At-the-money", and "Options graph". After these calculation, the user can exit the form by clicking on the button "Close User Interface" or switch back to the "User Interface to price Options" by clicking on the button "Switch to UI for options".<br>
Moreover, the user can delete a specific row of the table by clicking on the button "Delete a specific row" or delete the entire table by clicking on the button "Delete the entire table".<br>
A further information. If the user has already calculated a first option price, when the "User Interface to price Options" is opened again, the form will show the last values the user has input in the previous calculation, so that the user can easily repeat the same calculation if he/she wants to. This process is the same for the "Additional information" button.
