# ATS Infinity MT5

ATS Infinity MT5 is a forex robot developed by the Forex Robot Easy Team. This robot is designed to automate trading on the MetaTrader 5 platform. It is capable of opening pending orders based on significant price movements.

## Product Description

ATS Infinity MT5 is an expert advisor that utilizes advanced algorithms to identify significant price movements in the forex market. When a significant price movement is detected, the robot opens pending orders to take advantage of potential profit opportunities.

Key Features:
- Automatic trading: The robot automatically executes trading logic based on predefined rules.
- Pending orders: The robot opens buy stop and sell stop pending orders to capture potential market movements.
- Risk management: The robot allows users to define the lot size, stop loss, and take profit levels for each trade.

To use ATS Infinity MT5, simply include the necessary libraries and define the required constants. The robot will then execute the trading logic on each tick.

## Code Explanation

The code begins with necessary library inclusions. The `Trade.mqh` library is used for trading operations, while the `Math.mqh` library is used for mathematical calculations.

Next, constants are defined for the symbol, lot size, stop loss, and take profit levels. These values can be adjusted according to the user's preferences.

The trade object is initialized using the `CTrade` class. This object will be used to execute trading operations.

The `OpenPendingOrders` function is defined to open buy stop and sell stop pending orders. It calculates the buy stop and sell stop levels based on the current price and opens the orders using the `BuyStop` and `SellStop` functions of the trade object.

The `IsSignificantMovement` function checks for significant price movements by comparing the current price with the previous price. If the percentage change is greater than or equal to 1%, it returns true, indicating a significant movement.

The `ExecuteTradingLogic` function is responsible for executing the trading logic. It calls the `IsSignificantMovement` function and if a significant movement is detected, it calls the `OpenPendingOrders` function to open pending orders.

The `OnTick` function is the entry point of the expert advisor. It is called on each tick of the market data. In this function, the `ExecuteTradingLogic` function is called, which triggers the trading logic.

## Disclaimer

Please note that Forex Robot Easy is not the official developer of ATS Infinity MT5. This code is a sample implementation that demonstrates how the product can work. For detailed reviews and trading results of this product, please visit the official developer's website at [https://forexroboteasy.com/forex-robot-review/review-ats-infinity-mt5-real-results-and-download-options/](https://forexroboteasy.com/forex-robot-review/review-ats-infinity-mt5-real-results-and-download-options/).

To find the official developer of this product and obtain the official version, please use the MQL5 marketplace or contact the official developer directly.
