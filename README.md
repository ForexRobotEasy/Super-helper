# Super Helper - ReadMe

Super Helper is a trading code developed by Forex Robot Easy Team. This code is designed to automate forex trading using arrow indicators. Please note that ForexRobotEasy is not the official developer of this product. We are only showcasing sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Indicator Signal Settings

- **IndicatorName** - Name of the indicator used for generating signals.
- **SubwindowNumber** - Subwindow number where the indicator is displayed.
- **BuySignalBuffer** - Buffer number for buy signals.
- **SellSignalBuffer** - Buffer number for sell signals.

## Connecting the Indicator

The code connects to the indicator and retrieves the signal arrow buffer using the `iCustom` function.

## Trading Functions

### OnTick

The `OnTick` function is called on every tick and contains the main trading logic. It calculates the moving average value and checks for a buy or sell signal.

If the moving average value is 0, it checks for a buy signal using the `SignalBuy` function. If a buy signal is detected, it opens a buy order using the `OpenBuyOrder` function.

If there is no buy signal, it checks for a sell signal using the `SignalSell` function. If a sell signal is detected, it opens a sell order using the `OpenSellOrder` function.

### SignalBuy

The `SignalBuy` function checks if the signal arrow buffer is positive and retrieves the buy signal value from the indicator using the `iCustom` function. If the buy signal value is not 0, it returns true indicating a buy signal.

### SignalSell

The `SignalSell` function checks if the signal arrow buffer is positive and retrieves the sell signal value from the indicator using the `iCustom` function. If the sell signal value is not 0, it returns true indicating a sell signal.

### OpenBuyOrder

The `OpenBuyOrder` function opens a buy order with the specified parameters. It sets the lot size, stop loss, take profit, and sends the order using the `OrderSend` function.

### OpenSellOrder

The `OpenSellOrder` function opens a sell order with the specified parameters. It sets the lot size, stop loss, take profit, and sends the order using the `OrderSend` function.

## Product Description

Super Helper is an automated forex trading code developed by the Forex Robot Easy Team. It is designed to assist traders in automating their trading strategies using arrow indicators. This code connects to the specified indicator and generates buy or sell signals based on the arrow buffers.

To use Super Helper, traders need to input the indicator name, subwindow number, buy signal buffer, and sell signal buffer. The code will then connect to the indicator and retrieve the signal arrow buffer. On every tick, the code calculates the moving average value and checks for buy or sell signals.

Traders can customize the lot size, stop loss, and take profit values in the `OpenBuyOrder` and `OpenSellOrder` functions according to their trading preferences.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Review: Super Helper](https://forexroboteasy.com/forex-robot-review/review-super-helper-automate-forex-trading-with-arrow-indicators/). Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work as described in this product. To find the official developer of this product, please use MQL5.
