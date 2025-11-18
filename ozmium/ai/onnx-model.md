# ONNX Model

Market data models use PyTorch DirectML to train an ONNX model on price horizons using various Coinbase [WebSocket](https://docs.cdp.coinbase.com/coinbase-app/advanced-trade-apis/websocket/websocket-channels) feeds for assets listed on the exchange. The aggregated training datasets are derived from Pandas TA [studies](https://www.pandas-ta.dev/api/studies/) which can include several hundred indicators.&#x20;

While currently designed using these sources for obtaining TA input and output, the training setup it designed to handle any number of indicators, including custom indicators, so it is not entirely reliant upon Pantas TA or Coinbase WebSocket feeds.
