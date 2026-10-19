# Forex Scanner Android App (source project)

This is a native Android Studio project starter for the manual-only multi-pair forex scanner.

## Important
- This package is Android source code, **not an installable APK**.
- Build it with Android Studio (Build > Build APK(s)) to produce an APK.
- The scanner is manual-only; it does not connect to Exness or place trades.
- Market data comes from Yahoo Finance public reference candles, not broker bid/ask quotes.
- TP/SL are reference levels of 60 pips; confirm pip conventions and actual prices in your broker's MT5 app.

## Build
1. Open this folder in Android Studio.
2. Let Gradle sync.
3. Build > Build APK(s).
4. The debug APK will be under `app/build/outputs/apk/debug/`.

The app fetches 1-minute and 5-minute candles for 28 common FX pairs, applies EMA/RSI/momentum filters, and displays BUY/SELL/WAIT. Public endpoints can rate-limit or fail; unavailable pairs are shown as such.
