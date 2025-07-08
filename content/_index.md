---
# title: Automate and Share Your Trading Strategies
toc: false
description: Ready to turn your TradingView strategies into powerful trading bots? ClonQuant provides a fast, flexible solution to automate your strategies across forex, stocks, futures, and cryptocurrencies, while enabling social trading to follow and replicate top-performing strategies effortlessly.
---

<!-- {{< index/hero title="Automate Your Trades. Copy the Best. Share Your Edge." ref="/downloads/_index.md" image="cq-landing-page.png" >}} -->
{{< index/hero title="Automate Your Trades. Copy the Best. Share Your Edge." url="https://be.clonquant.com/newsletter" image="cq-landing-page.png" >}}


{{< index/how-it-works >}}
{{% index/how-it-works-left title="How It Works" %}}
You can automate, refine, and scale your trading strategies effortlessly.
<!-- {{< youtube dQw4w9WgXcQ >}} -->
<!-- [Docs ⇨]({{< ref "/docs/_index.md" >}}) -->
{{% /index/how-it-works-left %}}
{{% index/how-it-works-right title="How to Automate Your Trading in 4 Simple Steps" %}}

{{% steps %}}
<!-- ### Step 1: Choose a Strategy Creator
Browse verified traders with real performance data.
### Step 2: Set Your Risk Preferences
Choose your lot size, SL/TP, or let our smart scaling do it for you.
### Step 3: Mirror Trades Automatically
Trades are executed instantly—no manual action needed. -->
### Step 1: Register & Activate
Create your account and get access to the trading dashboard. Activate your copy trading profile to begin.
### Step 2: Install Required Apps (MT5 and Clonquant)
Download and install MetaTrader 5 and the ClonQuant Stand-alone Desktop App on your Windows PC.
### Step 3: Update Configurations (Optional)
Customize your trading preferences: set risk levels, stop-loss/take-profit rules, or lot size caps.
### Step 4: Connect & Auto-Trade
Launch ClonQuant, click 'Connect', and let the signals do the work. Sit back and watch the bot handle your trades automatically.
{{% /steps %}}
{{% /index/how-it-works-right %}}
{{< /index/how-it-works >}}

{{< index/section-gray  >}}
  {{< index/partners image="exness.png" >}}
  {{< index/partners image="xm.png" >}}
  {{< index/partners image="mt5.png" >}}
  {{< index/partners image="ftmo.png" >}}
  {{< index/partners image="fundednext.png" >}}
  {{< index/partners image="pepperstone.png" >}}
{{< /index/section-gray >}}

{{< index/features >}}

{{% index/feature-card title="Smart Risk Scaling — Adaptive Lot Sizing" icon="cube" %}}
Automatically adjusts trade sizes based on your balance/equity and selected risk level—ensuring every trade fits your portfolio without overexposure or overleveraging.

{{% /index/feature-card %}}

{{% index/feature-card title="Total Control — Manual Overrides" icon="user-circle" %}}
Pause, stop, or customize trades anytime. Set your own SL, TP, or lot sizes—even on automated strategies. You can also override, modify, or manually close trades in real time.
{{% /index/feature-card %}}

{{% index/feature-card title="Transparent Strategy Insights" icon="document-report" %}}
View real-time performance metrics like win rate, drawdown, PnL, average R:R, profit factor, sharpe ratio, average holding time and more—no more guessing who's worth following.
{{% /index/feature-card %}}

{{% index/feature-card title="Real-Time Trade Execution" icon="clock" %}}
Our low-latency mirror engine ensures instant trade synchronization across accounts and brokers, while actively monitoring broker latency and slippage so your trades stay accurate and consistent.
{{% /index/feature-card %}}

{{% index/feature-card title="Verified Strategy Creators" icon="badge-check" %}}
Gain confidence by copying from vetted and trusted trading experts. Every strategy creator on our platform goes through a rigorous verification process—evaluating their performance history, risk profile, and consistency over time.
{{% /index/feature-card %}}

{{% index/feature-card title="Profit Share & Rewards System" icon="currency-dollar" %}}
For copiers, it’s fair and results-driven. For traders, it’s a powerful incentive to stay sharp, optimize strategies, and maintain consistent performance. Plus, top-performing traders can unlock rewards, exclusive features, and increased visibility.
{{% /index/feature-card %}}

{{< /index/features >}}

{{< index/cta >}}
{{% index/cta-left title="Connect via WebSocket API" %}}
With ClonQuant's advanced features, you can connect via WebSocket API using your favorite programming language and receive trading signals at lightning speed.


<!-- [Docs ⇨]({{< ref "/docs/_index.md" >}}) -->
{{% /index/cta-left %}}
{{% index/cta-right title="Easy to use API" %}}
Subcribe to the websocket:

{{% steps %}}

### Step 1

Connect to wss://be.clonquant.com/ws/[token] 

### Step 2

Authenticate and Connect to WebSocket:
{{% /steps %}}

{{< tabs items="Python,Nodejs,Shell" >}}
  {{< tab >}}
    ```python
    import websocket

    def on_message(ws, message):
        print("Received:", message)

    ws = websocket.WebSocketApp("wss://be.clonquant.com/ws/<token>", on_message=on_message)
    ws.run_forever()
    ```
  {{< /tab >}}
  {{< tab >}}
    ```javascript
    const WebSocket = require('ws');

    const socket = new WebSocket('wss://be.clonquant.com/ws/<token>');

    socket.on('open', () => {
      console.log('Connected');
    });

    socket.on('message', (data) => {
      console.log('Received:', data);
    });

    ```
  {{< /tab >}}
  {{< tab >}}
    ```shell
    websocat wss://be.clonquant.com/ws/<token>  \
      -H 'Authorization: Bearer <YOUR_API_KEY>'
    ```
  {{< /tab >}}

{{< /tabs >}}



<!-- Get your API key from [Account](/docs/_index.md) page in the app. -->
<!-- Join the Waitlist, click [here](#hero) to join. -->
<!-- Join the Waitlist, click [here]("https://be.clonquant.com/newsletter) to join. -->

<!-- [Full API reference]({{< ref "/docs/_index.md" >}}) -->

{{% /index/cta-right %}}
{{< /index/cta >}}

<!-- {{< index/extra-links >}}
Terms | Privacy | Disclaimer
{{< /index/extra-links >}} -->


<!-- {{< index/section-dark >}}
{{% index/cta-left title="Get started quickly" %}}
With ClonQuant's advanced features, you can automate, refine, and scale your trading strategies effortlessly.


[Docs ⇨]({{< ref "/docs/_index.md" >}})
{{% /index/cta-left %}}
{{% index/cta-right title="Easy to use API" %}}
Create a new chat session:

{{% steps %}}

### Step 1

This is the first step.

### Step 2

This is the second step.

{{% /steps %}}

{{< tabs items="JSON,YAML,TOML" >}}
  {{< tab >}}**SHELL**: 
  ```shell
  curl https://app.tryhelix.ai/api/v1/sessions \
    -H 'Authorization: Bearer <YOUR_API_KEY>'
    -d "input=yo&mode=inference&type=text"
  ```
  {{< /tab >}}
  {{< tab >}}**Nodejs**: YAML is a human-readable data serialization language.{{< /tab >}}
  {{< tab >}}**Python**: TOML aims to be a minimal configuration file format that's easy to read due to obvious semantics.{{< /tab >}}

{{< /tabs >}}



Generate an image:

```shell
curl https://app.tryhelix.ai/api/v1/sessions \
  -H 'Authorization: Bearer <YOUR_API_KEY>'
  -d "input=flying fish&mode=inference&type=image"
```

Get your API key from [Account](https://app.tryhelix.ai/account) page in the app.

[Full API reference]({{< ref "/docs/_index.md" >}})
{{% /index/cta-right %}}
{{< /index/section-dark >}} -->

<!-- This is the landing page.

## Explore

{{< cards >}}
  {{< card link="docs" title="Docs" icon="book-open" >}}
  {{< card link="about" title="About" icon="user" >}} 
{{< /cards >}}-->

 <!-- {{< cards >}}
  {{< card link="/" title="Image Card" image="https://source.unsplash.com/featured/800x600?landscape" subtitle="Unsplash Landscape" >}}
  {{< card link="/" title="Local Image" image="/images/card-image-unprocessed.jpg" subtitle="Raw image under static directory." >}}
 {{< card link="/" title="Local Image" image="images/space.jpg" subtitle="Image under assets directory, processed by Hugo." method="Resize" options="600x q80 webp" >}}
{{< /cards >}} -->

<!-- {{% steps %}}

### Step 1

This is the first step.

### Step 2

This is the second step.

{{% /steps %}}

{{< tabs items="JSON,YAML,TOML" >}}

  {{< tab >}}**JSON**: JavaScript Object Notation (JSON) is a standard text-based format for representing structured data based on JavaScript object syntax.{{< /tab >}}
  {{< tab >}}**YAML**: YAML is a human-readable data serialization language.{{< /tab >}}
  {{< tab >}}**TOML**: TOML aims to be a minimal configuration file format that's easy to read due to obvious semantics.{{< /tab >}}

{{< /tabs >}}

## Documentation

For more information, visit [Hextra](https://imfing.github.io/hextra). -->
