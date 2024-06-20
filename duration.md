

## Finance & economics | [Buttonwood](https://www.economist.com/finance-and-economics/2024/06/19/think-nvidia-looks-dear-american-shares-could-get-pricier-still)

### Think Nvidia looks dear? American shares could get pricier still

**Investors are willing to follow whichever narrative paints the rosiest picture**

![](https://www.economist.com/cdn-cgi/image/width=1424,quality=80,format=auto/media-assets/image/20240622_FNP502.jpg)

**Jun 19th 2024**

---

**How can you tell it’s time to get out of the market?** In 1929 Joseph Kennedy, an American businessman and politician, supposedly realized the party was over upon hearing a shoe-shine boy dispensing stock tips. In 2000 the exit doors beckoned after 17 “dotcom” firms paid millions of dollars each for brief advertising slots during the Super Bowl, an American football extravaganza.

And so to a sell signal fit for 2024: Keith Gill is back on social media. Mr. Gill was an architect of the meme-stock frenzy of 2021, exhorting retail traders to buy shares in GameStop, a struggling chain of video-game shops. After a three-year absence he is posting once again, now apparently in possession of a stake in the firm worth a few hundred million dollars. GameStop’s share price has resumed a gut-churning rollercoaster ride and is up by more than 40% since Mr. Gill’s return; the ailing company has made use of the excitement to issue some $3bn-worth of new shares. If you are looking for signs of speculative excess in markets, this is Exhibit A.

America’s benchmark S&P 500 share index is hitting new highs every other week, fueled by enthusiasm about artificial intelligence (AI). On June 18th this made Nvidia, a chip designer, the world’s most valuable firm. The cyclically adjusted price-earnings ratio, popularized by Robert Shiller of Yale University, is at nearly 36. It has been higher only before the crashes of the early 2000s and 2022—and even then, not by much. That a correction will arrive at some point seems a racing certainty, but in the meantime there is a more worrying prospect still.

---

Certainly! To illustrate the concepts discussed in the article, such as the cyclically adjusted price-earnings (CAPE) ratio, stock price movements, and duration analysis in relation to interest rates, we can generate several plots using Python with Matplotlib and Pandas. Here’s the Python code to create these graphics:

```python
import matplotlib.pyplot as plt
import pandas as pd
import numpy as np

# Generate dummy data to simulate the key concepts
np.random.seed(42)
dates = pd.date_range(start='2020-01-01', periods=365*4, freq='D')

# Simulate S&P 500 index price data
sp500_prices = np.cumprod(1 + np.random.randn(len(dates)) * 0.001 + 0.0002) * 3000
sp500_prices = pd.Series(sp500_prices, index=dates)

# Simulate CAPE ratio data
cape_ratio = 30 + np.random.randn(len(dates)) * 2
cape_ratio = pd.Series(cape_ratio, index=dates)

# Simulate interest rate data
interest_rates = 2 + np.random.randn(len(dates)) * 0.1
interest_rates = pd.Series(interest_rates, index=dates)

# Plot S&P 500 index price data
plt.figure(figsize=(14, 7))
plt.plot(sp500_prices, label='S&P 500 Index')
plt.title('S&P 500 Index Price Over Time')
plt.xlabel('Date')
plt.ylabel('Price')
plt.legend()
plt.grid(True)
plt.show()

# Plot CAPE ratio data
plt.figure(figsize=(14, 7))
plt.plot(cape_ratio, label='CAPE Ratio', color='orange')
plt.title('Cyclically Adjusted Price-Earnings (CAPE) Ratio Over Time')
plt.xlabel('Date')
plt.ylabel('CAPE Ratio')
plt.legend()
plt.grid(True)
plt.show()

# Plot interest rates data
plt.figure(figsize=(14, 7))
plt.plot(interest_rates, label='Interest Rates', color='red')
plt.title('Interest Rates Over Time')
plt.xlabel('Date')
plt.ylabel('Interest Rate (%)')
plt.legend()
plt.grid(True)
plt.show()

# Plot S&P 500 index price with CAPE ratio and interest rates
fig, ax1 = plt.subplots(figsize=(14, 7))

ax1.set_xlabel('Date')
ax1.set_ylabel('S&P 500 Index Price', color='blue')
ax1.plot(sp500_prices, label='S&P 500 Index', color='blue')
ax1.tick_params(axis='y', labelcolor='blue')

ax2 = ax1.twinx()
ax2.set_ylabel('CAPE Ratio', color='orange')
ax2.plot(cape_ratio, label='CAPE Ratio', color='orange')
ax2.tick_params(axis='y', labelcolor='orange')

ax3 = ax1.twinx()
ax3.spines['right'].set_position(('outward', 60))
ax3.set_ylabel('Interest Rates (%)', color='red')
ax3.plot(interest_rates, label='Interest Rates', color='red')
ax3.tick_params(axis='y', labelcolor='red')

fig.tight_layout()
plt.title('S&P 500 Index Price, CAPE Ratio, and Interest Rates Over Time')
plt.grid(True)
plt.show()
```

### Explanation:
1. **S&P 500 Index Price Over Time**: This plot shows the simulated price of the S&P 500 index over time, illustrating the general trend and volatility.
2. **CAPE Ratio Over Time**: This plot illustrates the cyclically adjusted price-earnings ratio over the same period, indicating periods of high or low market valuations.
3. **Interest Rates Over Time**: This plot shows the movement of interest rates, which is crucial for understanding the duration analysis and its impact on stock prices.
4. **Combined Plot**: This combined plot overlays the S&P 500 index price, CAPE ratio, and interest rates to provide a comprehensive view of their interrelations.

These plots help to visually understand the relationships and trends described in the article, particularly the impact of interest rates on long-duration assets like high-valuation stocks and the implications for future market movements.
