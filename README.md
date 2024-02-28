# HFT Prop Pass Expert Advisor

This is the code for the HFT Prop Pass Expert Advisor, developed by the Forex Robot Easy Team. Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

For detailed reviews and trading results of this product, please visit [here](https://forexroboteasy.com/forex-robot-review/hft-prop-pass-review-high-speed-forex-trading-ea-success/).

## Description

The HFT Prop Pass Expert Advisor is designed for high-speed forex trading. It utilizes a custom indicator for market analysis and opens buy or sell trades based on the indicator signals. The EA calculates the lot size based on the risk percentage per trade and the stop loss in pips.

## Input Parameters

- `riskPercentage`: Risk percentage per trade (default: 2.0)
- `stopLossPips`: Stop loss in pips (default: 10)
- `takeProfitPips`: Take profit in pips (default: 20)

## Global Variables

- `lotSize`: Calculated lot size based on risk percentage and stop loss
- `accountBalance`: Current account balance
- `riskAmount`: Calculated risk amount based on risk percentage and account balance

## Custom Indicator

The custom indicator function `CustomIndicator()` is where you can add your own custom indicator logic.

## Initialization Function

The `OnInit()` function is called during the EA initialization process. It calculates the lot size based on the risk percentage and account balance.

## Start Function

The `OnTick()` function is called on every tick and performs market analysis using the custom indicator. If the indicator signal is 1, a buy trade is opened. If the indicator signal is -1, a sell trade is opened. The entry price, stop loss price, and take profit price are calculated based on the current market prices and the defined stop loss and take profit in pips.

## Deinitialization Function

The `OnDeinit()` function is called when the EA is being deinitialized. You can add any necessary cleanup code here.

## Stop Function

The `OnStop()` function is called when the EA is being stopped. You can add any necessary stop code here.

Please refer to the official developer of this product for more information and support.
