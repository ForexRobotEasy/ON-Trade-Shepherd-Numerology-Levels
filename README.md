# ON Trade Shepherd Numerology Levels

This code is a sample implementation of the ON Trade Shepherd Numerology Levels trading strategy. It utilizes the Shepherd Numerology Levels Indicator to identify potential support and resistance levels in the market. The strategy aims to execute trades based on these identified levels.

## Developer's Site

Forex Robot Easy Team is the development team behind this strategy. They provide various forex trading solutions and can be found on their website [forexroboteasy.com](https://forexroboteasy.com).

## Dependencies

The following libraries and dependencies are required for this code to work:

- `stdlib.mqh`
- `math.mqh`
- `TradeAlgorithms.mqh`

## Global Variables

The code defines the following global variables that can be adjusted:

- `numerologyPeriod`: The numerology period for the Square of Nine method. Default is 9.
- `tolerance`: The tolerance for price comparison. Default is 0.0001.
- `maxBars`: The maximum number of bars to consider for analysis. Default is 500.

## Helper Functions

The code includes the following helper functions:

### `GetNumerologyLevel(double price, double referencePrice)`

Calculates the numerology level based on the Square of Nine method.

- Input:
  - `price`: The current price value.
  - `referencePrice`: The reference price value.
- Output: The calculated numerology level.

### `IsPotentialTurningPoint(double price, double referencePrice, double level)`

Checks if a price is a potential turning point based on the numerology level.

- Input:
  - `price`: The current price value.
  - `referencePrice`: The reference price value.
  - `level`: The numerology level.
- Output: True if the price is a potential turning point, false otherwise.

### `FindSupportResistanceLevel(double price, double referencePrice)`

Finds the support or resistance level based on the numerology principles.

- Input:
  - `price`: The current price value.
  - `referencePrice`: The reference price value.
- Output: The identified support or resistance level, or 0.0 if none found.

## Main Trading Function

The main trading function is defined as `OnTrade()`. It performs the following steps:

1. Get the current price and reference price for analysis.
2. Perform analysis on previous bars.
3. Identify support and resistance levels using the Shepherd Numerology Levels Indicator.
4. Execute trading logic based on the identified support/resistance level.

## Entry Point

The entry point of the program is defined as `OnInit()`. It initializes necessary indicators and settings. The function returns `INIT_SUCCEEDED` if initialization is successful.

## Update Trading Logic

The trading logic is updated on every tick through the `OnTick()` function.

## Error Handling

The program defines the `OnDeinit(const int reason)` function to handle any unexpected behavior and clean up resources.

## Optimization Settings

The `OnTester()` function is used to set optimization parameters for backtesting.

## Product Description

The ON Trade Shepherd Numerology Levels is a forex trading strategy developed by the Forex Robot Easy Team. It utilizes the Shepherd Numerology Levels Indicator to identify potential support and resistance levels in the market. The strategy aims to execute trades based on these identified levels.

This code provides a sample implementation of the strategy and can be used as a reference. ForexRobotEasy is not the official developer of this product. To find the official developer and obtain detailed reviews and trading results, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/trade-shepherd-review-unveil-forex-patterns-with-numerology/).

Please note that the effectiveness of this strategy may vary depending on market conditions and individual trading preferences. It is recommended to conduct thorough testing and analysis before using it in live trading.
