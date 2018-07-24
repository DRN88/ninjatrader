# HighlightMyDateTime Ninjatrader 8 Indicator

## 1. About
* This indicator helps you find correlations between instruments price movement using **Vertical Lines** (ES -> FDAX, NQ, YM). This works great with `CurrentDayOHL` and `PriorDayOHLC`, etc. important price locations as support/resistance levels.
* Master and Slave roles are defined
  * Master: Where you draw your vertical lines which you want to replicate to other instruments/charts.
  * Slave: Where the Master chart's vertical lines DateTime Anchor data is used to draw vertical lines automatically.
* Everything happens on `OnRender()` event, so it is fast.
* This indicator works with CSV files. CSV File is created here: `%TEMP%\HighlightMyDateTime_<GroupID>.csv`
* Compatible with NT8

## 2. Installation
* Download `HighlightMyDateTime.zip`
* Navigate to: `Tools -> Import -> NinjaScript Add-On...`
* Browse to `HighlightMyDateTime.zip`, then import

## 3. Using HighlightMyDateTime indicator
* Open some instruments, like ES and NQ on two separate charts.
* Apply `HighlightMyDateTime` indicator on both charts.
* Tick `MasterMode` parameter on ES chart and draw a few vertical lines.
* Set `GroupID` parameter if needed. They have to match on both charts.
* You should see vertical lines appearing on NQ at the same DateTime Anchor which you drew on the ES chart.
* Enjoy

## 4. License: Mozilla Public License, version 2.0
https://www.mozilla.org/en-US/MPL/2.0/
