<p align="center">
  <img src="https://github.com/user-attachments/assets/fcf38350-e3a0-40d2-ada2-ba3ecead1b9f" 
       alt="FileFlow"
       width="60%" />
</p>


# ARPS Ultimate Signal Framework (USF)
**Originally created: August 21, 2020**
*(Note: This script was created in 2020 but is being shared on GitHub on 2025-04-25)*

---

# ARPS Ultimate Signal Framework (USF)

### By: Ali Rajabpour-Sanati | ali.poursanati@gmail.com

## Overview

The **ARPS Ultimate Signal Framework (USF)** is a powerful and advanced Pine Script indicator designed for intraday trading on the TradingView platform. It leverages a combination of trend analysis methodologies, adaptive oscillators, and signal generation mechanisms to provide highly insightful market indicators. The framework integrates multiple technical analysis tools, making it invaluable for traders seeking precise market entry and exit signals.

---

## Key Features

### 1. **Adaptive ATR-ADX Trend Analysis**
   - Utilizes **Average True Range (ATR)** and **Average Directional Index (ADX)** calculations to identify trends and reversals.
   - Adaptive multiplier adjusts dynamically based on ADX's rising or falling state, providing a reliable trend strength metric.
   - Can use **Heikin-Ashi candles** or regular price data for calculations.

### 2. **Oscillator Counter**
   - Tracks the state of multiple oscillators over time, dynamically incrementing or decrementing based on signal conditions across the framework.

### 3. **Ichimoku Cloud**
   - Includes the **Kumo Cloud**, **Tenkan Sen**, **Kijun Sen**, and **Chikou Span** to detect momentum shifts and support/resistance levels.
   - Signal generation based on specific crossovers among Ichimoku components.

### 4. **200 EMA Positioning**
   - Calculates positions relative to the **200 EMA** values across multiple intervals, including 30 minutes, 4 hours, and daily.
   - Visual indicators (up/down arrows) plotted directly on the chart to highlight price positioning.

### 5. **Stochastic RSI**
   - Combines RSI with stochastic calculations to identify overbought or oversold conditions.
   - Customizable length and smoothing inputs for precise tuning.

### 6. **Money Flow Index (MFI)**
   - Calculates the MFI based on positive and negative money flow, identifying oversold and overbought zones.
   - Customizable timeframe and sensitivity.

### 7. **Squeeze Momentum Indicator**
   - Identifies market conditions based on interactions between Bollinger Bands (BB) and Keltner Channels (KC).
   - Generates actionable "Go Long," "Go Short," "Exit Long," and "Exit Short" signals based on squeeze states.

### 8. **WaveTrend Oscillator**
   - Provides oversold and overbought conditions derived from price and volume.
   - Additional fine-tuning adjusts overbought/oversold signal levels for enhanced precision.

### 9. **Parabolic SAR**
   - Implements Parabolic SAR to track market momentum and identify reversal points.
   - Signal integration directly affects the oscillator counter.

### 10. **Candle Patterns Recognition**
   - Detects bullish and bearish candle patterns, including:
     - Morning Star, Shooting Star, Hammer, Harami, Engulfing, and Dark Cloud Cover.
   - Provides fractional adjustments to the oscillator counter for finer pattern-based predictions.

### 11. **Hull Moving Average (Hull MA)**
   - Incorporates **Hull MA** with crossovers against **T3 MA** to optimize trend-following analysis.
   - Integrated with WaveTrend thresholds for enhanced trading signals.

### 12. **Tillson MA (T3)**
   - A modified moving average that emphasizes smoother trend tracking.
   - Works in tandem with Hull MA and oscillator calculations.

---

## How It Works

1. **Calculation Modules**  
   Each technical indicator operates as a module within the script. Signal calculations and results are consolidated into an `osc_counter`, which tracks cumulative market sentiment.

2. **Visual Outputs**  
   The script plots key indicators such as trends, EMAs, Ichimoku crossovers, and Bollinger/Keltner channel states directly onto the TradingView chart. Arrows and labels provide actionable signals.

3. **Logic Flow**  
   Decisions are made based on predefined thresholds and conditions. For example:
   - If the price crosses below the Money Flow Index's oversold threshold, the `osc_counter` increments, signaling a potential buy condition.
   - A Hull MA crossover might trigger incremental adjustments to the oscillator, suggesting trend-related opportunities.

---

## Configuration Options

The framework allows users to customize the indicator's behavior using inputs directly within TradingView:

- **Trend Analysis Inputs**:
  - ATR Length and Multipliers
  - Use Heikin-Ashi or regular price data
- **Oscillators**:
  - Stochastic RSI length and smoothing
  - Money Flow Index length
- **Candle Patterns**:
  - Enable or disable specific patterns
- **WaveTrend Parameters**:
  - Oversold/Overbought threshold tuning
- **Moving Averages**:
  - Hull MA length, Tillson MA length

---

## Dependencies

The ARPS Ultimate Signal Framework is built entirely in Pine Script version 4. It is a standalone indicator that does not require external libraries or dependencies.

---

## Installation

1. Open TradingView and navigate to the Pine Editor.
2. Copy the code into the editor and save it as a custom script.
3. Add the indicator to your chart from the "My Scripts" section.

---

## Usage Instructions

- Use along with other indicators to validate signals.
- Customize input parameters to align with your trading strategy.
- Combine with additional market elements (e.g., volume-based analysis) for advanced setups.

---

## Future Improvements

- **Dynamic Risk Management Integration**: Incorporate stop-loss and take-profit levels based on oscillator signals.
- **Expanded Timeframe Support**: Additional customizable intervals for greater flexibility.
- **Advanced AI Analytics**: Leverage machine learning to dynamically adjust indicator sensitivity.

---

## License

This script is released under **MIT License**. You can use, modify, and share the code with appropriate attribution.

---

## Support

For feedback, questions, or issues, please contact **Ali Rajabpour-Sanati** at ali.poursanati@gmail.com.
