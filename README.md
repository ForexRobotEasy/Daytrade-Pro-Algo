# Daytrade Pro Algo ReadMe

## Introduction
This is the ReadMe file for the Daytrade Pro Algo code. The Daytrade Pro Algo is a trading algorithm developed by the Forex Robot Easy Team. It is designed to trade multiple currency pairs based on price action and support/resistance levels.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Daytrade Pro Algo Review](https://forexroboteasy.com/forex-robot-review/daytrade-pro-algo-review-limited-offer-with-real-results/). Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in the product. To find the official developer of this product, please use MQL5.

## Code Description
The code includes necessary libraries and defines a list of currency pairs to trade. It then implements the main function `OnTick()` which is called on each tick of the market.

Within the `OnTick()` function, the code checks if trading is allowed based on market hours. If trading is allowed, it loops through each pair in the list and checks if the pair is allowed for trading. It then retrieves the current price, support level, and resistance level for the pair.

The code then checks if the current price is near a support or resistance level. If so, it executes a trade based on the price action. If the current price is above the resistance level, it executes a buy trade. If the current price is below the support level, it executes a sell trade.

The code also includes several helper functions to check if trading is allowed, if a pair is allowed for trading, to calculate the support and resistance levels, and to check if the current price is near a support or resistance level. It also includes empty functions to execute buy and sell trades.

## Usage
To use the Daytrade Pro Algo, follow these steps:
1. Include the necessary libraries `Trade.mqh` and `TradeState.mqh`.
2. Define the list of currency pairs to trade in the `pairs` array.
3. Implement the necessary logic in the `IsTradeAllowed()` and `IsPairAllowed()` functions to check if trading is allowed based on market hours and if a specific pair is allowed for trading.
4. Implement the necessary logic in the `GetSupportLevel()` and `GetResistanceLevel()` functions to calculate the support and resistance levels for each pair.
5. Implement the necessary logic in the `IsNearSupport()` and `IsNearResistance()` functions to check if the current price is near a support or resistance level.
6. Implement the necessary logic in the `Buy()` and `Sell()` functions to execute buy and sell trades.

## License
The Daytrade Pro Algo code is provided under the [MIT License](https://opensource.org/licenses/MIT).
