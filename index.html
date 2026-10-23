Here is a complete HTML document for a derivative trading simulator. You can run it directly in your browser to practice trading with a virtual balance.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Deriv — trading simulator</title>
    <!-- Google Font & simple styling -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', system-ui, -apple-system, sans-serif;
            background: #0b0e14;
            color: #e9edf2;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 16px;
        }

        .app-container {
            max-width: 1280px;
            width: 100%;
            background: #131a24;
            border-radius: 32px;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.8);
            padding: 24px;
            border: 1px solid #2a3440;
        }

        /* header */
        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 16px;
            margin-bottom: 28px;
        }

        .logo-area {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo-icon {
            background: #00c6a7;
            width: 38px;
            height: 38px;
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            font-size: 22px;
            color: #0b0e14;
            box-shadow: 0 6px 12px rgba(0, 198, 167, 0.25);
        }

        .logo-text {
            font-size: 24px;
            font-weight: 700;
            letter-spacing: -0.5px;
            background: linear-gradient(135deg, #ffffff, #b0c4de);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .balance-card {
            background: #0f1620;
            border-radius: 100px;
            padding: 8px 20px 8px 24px;
            display: flex;
            align-items: center;
            gap: 16px;
            border: 1px solid #2e3b48;
            box-shadow: inset 0 2px 4px rgba(0,0,0,0.4);
        }

        .balance-label {
            font-size: 14px;
            color: #8f9eb0;
            font-weight: 500;
        }

        .balance-value {
            font-size: 22px;
            font-weight: 700;
            color: #00c6a7;
            letter-spacing: -0.3px;
        }

        .balance-value.usd::before {
            content: '$';
            margin-right: 2px;
            font-size: 18px;
            font-weight: 600;
            color: #b0c4de;
        }

        /* main grid */
        .trading-grid {
            display: grid;
            grid-template-columns: 1fr 360px;
            gap: 20px;
            margin-bottom: 20px;
        }

        @media (max-width: 800px) {
            .trading-grid {
                grid-template-columns: 1fr;
            }
            .app-container {
                padding: 16px;
            }
        }

        /* chart panel */
        .chart-panel {
            background: #0f1620;
            border-radius: 24px;
            padding: 18px 18px 12px 18px;
            border: 1px solid #25313e;
            box-shadow: inset 0 2px 8px rgba(0,0,0,0.5);
        }

        .chart-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 12px;
        }

        .pair-badge {
            background: #1e2a38;
            padding: 6px 14px;
            border-radius: 100px;
            font-weight: 600;
            font-size: 15px;
            border: 1px solid #31465a;
            letter-spacing: 0.3px;
        }

        .price-display {
            font-size: 26px;
            font-weight: 700;
            font-variant-numeric: tabular-nums;
            transition: color 0.2s;
        }

        .chart-container {
            width: 100%;
            height: 280px;
            position: relative;
        }

        #priceChart {
            width: 100%;
            height: 100%;
            display: block;
        }

        .chart-footer {
            display: flex;
            justify-content: space-between;
            margin-top: 10px;
            color: #8f9eb0;
            font-size: 13px;
            font-weight: 500;
        }

        /* trade panel */
        .trade-panel {
            background: #0f1620;
            border-radius: 24px;
            padding: 22px 20px;
            border: 1px solid #25313e;
            display: flex;
            flex-direction: column;
            gap: 22px;
        }

        .contract-type {
            display: flex;
            gap: 12px;
        }

        .btn-direction {
            flex: 1;
            padding: 14px 0;
            border-radius: 16px;
            font-weight: 700;
            font-size: 16px;
            border: none;
            cursor: pointer;
            transition: all 0.15s ease;
            background: #1b2532;
            color: #b0c4de;
            border: 1px solid #2e3b48;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }

        .btn-direction.active-buy {
            background: #00c6a7;
            color: #0b0e14;
            border-color: #00c6a7;
            box-shadow: 0 0 16px rgba(0, 198, 167, 0.3);
        }

        .btn-direction.active-sell {
            background: #f6465d;
            color: #ffffff;
            border-color: #f6465d;
            box-shadow: 0 0 16px rgba(246, 70, 93, 0.3);
        }

        .btn-direction:hover {
            filter: brightness(1.1);
        }

        .input-group {
            display: flex;
            flex-direction: column;
            gap: 8px;
        }

        .input-group label {
            font-size: 14px;
            color: #8f9eb0;
            font-weight: 500;
        }

        .input-wrapper {
            display: flex;
            align-items: center;
            background: #1b2532;
            border-radius: 16px;
            padding: 4px 8px 4px 18px;
            border: 1px solid #2e3b48;
            transition: border 0.15s;
        }

        .input-wrapper:focus-within {
            border-color: #00c6a7;
        }

        .input-wrapper input {
            background: transparent;
            border: none;
            color: #e9edf2;
            font-size: 18px;
            font-weight: 600;
            width: 100%;
            padding: 12px 0;
            outline: none;
            font-variant-numeric: tabular-nums;
        }

        .input-wrapper input::placeholder {
            color: #4e5f73;
            font-weight: 400;
        }

        .input-suffix {
            color: #8f9eb0;
            font-weight: 600;
            font-size: 16px;
            padding: 0 10px;
            background: #131a24;
            border-radius: 30px;
            line-height: 1;
            padding: 8px 14px;
            border: 1px solid #2a3440;
            cursor: pointer;
            transition: background 0.15s;
        }

        .input-suffix:hover {
            background: #1e2a38;
        }

        .quick-stakes {
            display: flex;
            gap: 8px;
            margin-top: 4px;
        }

        .quick-stake {
            background: #1b2532;
            border: 1px solid #2e3b48;
            color: #b0c4de;
            padding: 6px 12px;
            border-radius: 40px;
            font-size: 13px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.1s;
        }

        .quick-stake:hover {
            background: #253544;
            border-color: #3e5268;
        }

        .payout-info {
            background: #131e28;
            border-radius: 16px;
            padding: 14px 18px;
            display: flex;
            justify-content: space-between;
            font-size: 15px;
            border: 1px solid #25313e;
        }

        .payout-label {
            color: #8f9eb0;
        }

        .payout-value {
            font-weight: 700;
            color: #00c6a7;
        }

        .btn-trade {
            background: #00c6a7;
            border: none;
            padding: 18px;
            border-radius: 20px;
            font-size: 18px;
            font-weight: 700;
            color: #0b0e14;
            cursor: pointer;
            transition: all 0.15s;
            letter-spacing: 0.3px;
            box-shadow: 0 8px 18px rgba(0, 198, 167, 0.25);
            margin-top: 4px;
        }

        .btn-trade:hover {
            background: #00ddb9;
            transform: scale(1.01);
        }

        .btn-trade:disabled {
            background: #2a3a48;
            color: #6b7d91;
            box-shadow: none;
            cursor: not-allowed;
            transform: none;
        }

        /* history section */
        .history-section {
            background: #0f1620;
            border-radius: 24px;
            padding: 16px 20px;
            border: 1px solid #25313e;
            margin-top: 8px;
        }

        .history-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 12px;
            padding: 0 4px;
        }

        .history-title {
            font-weight: 600;
            color: #b0c4de;
            font-size: 16px;
            letter-spacing: 0.2px;
        }

        .history-count {
            background: #1e2a38;
            padding: 3px 10px;
            border-radius: 40px;
            font-size: 13px;
            color: #8f9eb0;
        }

        .history-list {
            max-height: 180px;
            overflow-y: auto;
            display: flex;
            flex-direction: column;
            gap: 8px;
            padding-right: 4px;
        }

        .history-list::-webkit-scrollbar {
            width: 5px;
        }

        .history-list::-webkit-scrollbar-thumb {
            background: #2e3b48;
            border-radius: 10px;
        }

        .history-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 14px;
            background: #131e28;
            border-radius: 14px;
            font-size: 14px;
            border-left: 4px solid #2e3b48;
            animation: fadeIn 0.2s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-4px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .history-item.buy-win { border-left-color: #00c6a7; }
        .history-item.sell-win { border-left-color: #f6465d; }
        .history-item.loss { border-left-color: #4e5f73; }

        .history-left {
            display: flex;
            gap: 14px;
            align-items: center;
        }

        .history-direction {
            font-weight: 700;
            font-size: 13px;
            padding: 2px 10px;
            border-radius: 40px;
            background: #1b2532;
            color: #b0c4de;
            text-transform: uppercase;
        }

        .history-direction.up {
            background: rgba(0, 198, 167, 0.15);
            color: #00c6a7;
        }

        .history-direction.down {
            background: rgba(246, 70, 93, 0.15);
            color: #f6465d;
        }

        .history-amount {
            font-weight: 600;
        }

        .history-result {
            font-weight: 700;
            font-variant-numeric: tabular-nums;
        }

        .profit { color: #00c6a7; }
        .loss-text { color: #f6465d; }

        .empty-history {
            color: #4e5f73;
            text-align: center;
            padding: 24px 0;
            font-style: italic;
            font-size: 14px;
        }
    </style>
</head>
<body>
<div class="app-container">
    <!-- header -->
    <div class="header">
        <div class="logo-area">
            <div class="logo-icon">D</div>
            <span class="logo-text">Deriv<span style="font-weight:400; color:#8f9eb0;">·sim</span></span>
        </div>
        <div class="balance-card">
            <span class="balance-label">BALANCE</span>
            <span class="balance-value usd" id="balanceDisplay">10,000.00</span>
        </div>
    </div>

    <!-- main trading area -->
    <div class="trading-grid">
        <!-- chart panel -->
        <div class="chart-panel">
            <div class="chart-header">
                <span class="pair-badge">📈 VOL 100 · 1s</span>
                <span class="price-display" id="currentPrice">1,245.32</span>
            </div>
            <div class="chart-container">
                <canvas id="priceChart" width="800" height="280"></canvas>
            </div>
            <div class="chart-footer">
                <span>⏱️ live simulation</span>
                <span id="chartChange">+0.00%</span>
            </div>
        </div>

        <!-- trade panel -->
        <div class="trade-panel">
            <div class="contract-type">
                <button class="btn-direction active-buy" id="btnBuy" data-dir="buy">
                    ▲ BUY / UP
                </button>
                <button class="btn-direction" id="btnSell" data-dir="sell">
                    ▼ SELL / DOWN
                </button>
            </div>

            <div class="input-group">
                <label>Stake amount</label>
                <div class="input-wrapper">
                    <input type="number" id="stakeInput" value="100" min="1" step="10" placeholder="0.00">
                    <span class="input-suffix" id="currencyLabel">USD</span>
                </div>
                <div class="quick-stakes">
                    <span class="quick-stake" data-stake="10">$10</span>
                    <span class="quick-stake" data-stake="50">$50</span>
                    <span class="quick-stake" data-stake="100">$100</span>
                    <span class="quick-stake" data-stake="500">$500</span>
                </div>
            </div>

            <div class="payout-info">
                <span class="payout-label">Payout (85%)</span>
                <span class="payout-value" id="payoutDisplay">$185.00</span>
            </div>

            <button class="btn-trade" id="tradeBtn">PLACE TRADE</button>
        </div>
    </div>

    <!-- trade history -->
    <div class="history-section">
        <div class="history-header">
            <span class="history-title">📋 Recent trades</span>
            <span class="history-count" id="historyCount">0</span>
        </div>
        <div class="history-list" id="historyList">
            <div class="empty-history">No trades yet — place your first derivative</div>
        </div>
    </div>
</div>

<script>
    (function() {
        // ---------- state ----------
        let balance = 10000.00;
        let currentPrice = 1245.32;
        let priceHistory = Array(80).fill(currentPrice); // for chart
        let selectedDirection = 'buy'; // 'buy' or 'sell'
        const PAYOUT_RATE = 0.85; // 85% profit on win (stake + profit returned)
        let trades = []; // { id, direction, stake, entryPrice, exitPrice, result, payout, timestamp }

        // canvas & context
        const canvas = document.getElementById('priceChart');
        const ctx = canvas.getContext('2d');

        // DOM elements
        const balanceDisplay = document.getElementById('balanceDisplay');
        const currentPriceEl = document.getElementById('currentPrice');
        const chartChangeEl = document.getElementById('chartChange');
        const stakeInput = document.getElementById('stakeInput');
        const payoutDisplay = document.getElementById('payoutDisplay');
        const tradeBtn = document.getElementById('tradeBtn');
        const btnBuy = document.getElementById('btnBuy');
        const btnSell = document.getElementById('btnSell');
        const historyList = document.getElementById('historyList');
        const historyCount = document.getElementById('historyCount');

        // ---------- helpers ----------
        function formatMoney(value) {
            return value.toFixed(2).replace(/\B(?=(\d{3})+(?!\d))/g, ',');
        }

        function updateBalanceUI() {
            balanceDisplay.textContent = formatMoney(balance);
        }

        function updatePayout() {
            const stake = parseFloat(stakeInput.value) || 0;
            const payout = stake * (1 + PAYOUT_RATE);
            payoutDisplay.textContent = `$${formatMoney(payout)}`;
        }

        // price tick (random walk)
        function generateNewPrice() {
            const change = (Math.random() - 0.48) * 4.5; // slight upward bias
            currentPrice = Math.max(800, currentPrice + change);
            // keep 2 decimals
            currentPrice = Math.round(currentPrice * 100) / 100;
            return currentPrice;
        }

        // update chart data & UI
        function updatePriceUI() {
            currentPriceEl.textContent = currentPrice.toFixed(2);
            // chart change (relative to first price in history)
            const firstPrice = priceHistory[0] || currentPrice;
            const changePercent = ((currentPrice - firstPrice) / firstPrice) * 100;
            chartChangeEl.textContent = (changePercent >= 0 ? '+' : '') + changePercent.toFixed(2) + '%';
            chartChangeEl.style.color = changePercent >= 0 ? '#00c6a7' : '#f6465d';
        }

        // draw chart
        function drawChart() {
            const w = canvas.width;
            const h = canvas.height;
            ctx.clearRect(0, 0, w, h);

            // background grid
            ctx.strokeStyle = '#1e2a38';
            ctx.lineWidth = 1;
            for (let i = 0; i < 5; i++) {
                const y = (i / 4) * h;
                ctx.beginPath();
                ctx.moveTo(0, y);
                ctx.lineTo(w, y);
                ctx.strokeStyle = '#1e2a38';
                ctx.stroke();
            }

            if (priceHistory.length < 2) return;

            const minPrice = Math.min(...priceHistory) * 0.995;
            const maxPrice = Math.max(...priceHistory) * 1.005;
            const range = maxPrice - minPrice || 1;

            // draw line
            ctx.beginPath();
            ctx.strokeStyle = '#00c6a7';
            ctx.lineWidth = 3;
            ctx.lineJoin = 'round';
            ctx.lineCap = 'round';

            const stepX = w / (priceHistory.length - 1);
            priceHistory.forEach((price, i) => {
                const x = i * stepX;
                const y = h - ((price - minPrice) / range) * h;
                if (i === 0) ctx.moveTo(x, y);
                else ctx.lineTo(x, y);
            });
            ctx.stroke();

            // gradient fill under line
            ctx.lineTo(w, h);
            ctx.lineTo(0, h);
            ctx.closePath();
            const gradient = ctx.createLinearGradient(0, 0, 0, h);
            gradient.addColorStop(0, 'rgba(0, 198, 167, 0.15)');
            gradient.addColorStop(1, 'rgba(0, 198, 167, 0.01)');
            ctx.fillStyle = gradient;
            ctx.fill();

            // current price dot
            const lastX = (priceHistory.length - 1) * stepX;
            const lastY = h - ((priceHistory[priceHistory.length - 1] - minPrice) / range) * h;
            ctx.beginPath();
            ctx.arc(lastX, lastY, 6, 0, 2 * Math.PI);
            ctx.fillStyle = '#00c6a7';
            ctx.shadowColor = '#00c6a7';
            ctx.shadowBlur = 14;
            ctx.fill();
            ctx.shadowBlur = 0;
        }

        // update chart history on new tick
        function pushPriceToHistory(newPrice) {
            priceHistory.push(newPrice);
            if (priceHistory.length > 80) priceHistory.shift();
            drawChart();
        }

        // ---------- trade logic ----------
        function placeTrade() {
            const stake = parseFloat(stakeInput.value);
            if (isNaN(stake) || stake <= 0) {
                alert('Please enter a valid stake amount.');
                return;
            }
            if (stake > balance) {
                alert('Insufficient balance. Please lower your stake.');
                return;
            }

            // capture entry price and direction
            const entryPrice = currentPrice;
            const direction = selectedDirection;

            // deduct stake from balance (temporarily)
            balance -= stake;
            updateBalanceUI();

            // simulate outcome with 50% win probability (market random)
            // but we can also make it slightly direction-biased for fun? keep fair
            const isWin = Math.random() < 0.5; // 50% chance

            // small random price movement for exit
            const movement = (Math.random() - 0.5) * 9;
            const exitPrice = Math.round((entryPrice + (direction === 'buy' ? movement : -movement)) * 100) / 100;
            // Update current price to exit price for realism
            currentPrice = Math.max(800, exitPrice);
            currentPrice = Math.round(currentPrice * 100) / 100;
            pushPriceToHistory(currentPrice);

            let profit = 0;
            let payout = 0;
            let resultType = 'loss';

            if (isWin) {
                profit = stake * PAYOUT_RATE;
                payout = stake + profit; // return stake + profit
                balance += payout;       // add back full payout
                resultType = direction === 'buy' ? 'buy-win' : 'sell-win';
            } else {
                // loss: stake already deducted, nothing to add back
                profit = -stake;
                payout = 0;
                resultType = 'loss';
            }

            // record trade
            const trade = {
                id: Date.now() + Math.random(),
                direction: direction,
                stake: stake,
                entryPrice: entryPrice,
                exitPrice: currentPrice,
                result: resultType,
                profit: profit,
                payout: payout,
                timestamp: new Date(),
            };
            trades.unshift(trade); // newest first
            if (trades.length > 30) trades.pop();

            // update UI
            updateBalanceUI();
            renderHistory();
            updatePriceUI();
            updatePayout();

            // reset stake input? keep for convenience but set to last stake
            // ensure input value not bigger than balance? not necessary
        }

        // render history list
        function renderHistory() {
            historyCount.textContent = trades.length;

            if (trades.length === 0) {
                historyList.innerHTML = '<div class="empty-history">No trades yet — place your first derivative</div>';
                return;
            }

            let html = '';
            trades.forEach((trade, index) => {
                const profitClass = trade.profit >= 0 ? 'profit' : 'loss-text';
                const sign = trade.profit >= 0 ? '+' : '';
                const directionLabel = trade.direction === 'buy' ? 'UP' : 'DOWN';
                const directionClass = trade.direction === 'buy' ? 'up' : 'down';
                const itemClass = trade.result === 'loss' ? 'loss' : (trade.direction === 'buy' ? 'buy-win' : 'sell-win');

                html += `
                    <div class="history-item ${itemClass}">
                        <div class="history-left">
                            <span class="history-direction ${directionClass}">${directionLabel}</span>
                            <span class="history-amount">$${formatMoney(trade.stake)}</span>
                        </div>
                        <span class="history-result ${profitClass}">${sign}$${formatMoney(Math.abs(trade.profit))}</span>
                    </div>
                `;
            });

            historyList.innerHTML = html;
        }

        // ---------- market simulation ----------
        function tickMarket() {
            // update price with random walk
            generateNewPrice();
            pushPriceToHistory(currentPrice);
            updatePriceUI();
        }

        // ---------- event listeners ----------
        function setDirection(dir) {
            selectedDirection = dir;
            if (dir === 'buy') {
                btnBuy.classList.add('active-buy');
                btnBuy.classList.remove('active-sell');
                btnSell.classList.remove('active-sell');
                btnSell.classList.add('active-sell'); // actually we need to style sell as inactive
                // fix: remove active classes from both then add
                btnBuy.classList.add('active-buy');
                btnSell.classList.remove('active-sell', 'active-buy');
                btnSell.style.background = '#1b2532';
                btnSell.style.color = '#b0c4de';
                btnSell.style.borderColor = '#2e3b48';
                btnSell.style.boxShadow = 'none';
            } else {
                btnSell.classList.add('active-sell');
                btnBuy.classList.remove('active-buy');
                btnBuy.style.background = '#1b2532';
                btnBuy.style.color = '#b0c4de';
                btnBuy.style.borderColor = '#2e3b48';
                btnBuy.style.boxShadow = 'none';
            }

            // easier: reset both and set active
            btnBuy.className = 'btn-direction';
            btnSell.className = 'btn-direction';
            if (dir === 'buy') {
                btnBuy.classList.add('active-buy');
            } else {
                btnSell.classList.add('active-sell');
            }
        }

        // rewrite clean setDirection
        function setDirectionClean(dir) {
            selectedDirection = dir;
            btnBuy.className = 'btn-direction';
            btnSell.className = 'btn-direction';
            if (dir === 'buy') {
                btnBuy.classList.add('active-buy');
            } else {
                btnSell.classList.add('active-sell');
            }
        }

        // ---------- initialize ----------
        function init() {
            // set initial price history with slight variation
            for (let i = 0; i < 80; i++) {
                const base = 1200 + i * 1.5 + (Math.random() - 0.5) * 20;
                priceHistory[i] = Math.round(base * 100) / 100;
            }
            currentPrice = priceHistory[priceHistory.length - 1];
            currentPriceEl.textContent = currentPrice.toFixed(2);
            drawChart();
            updatePriceUI();
            updateBalanceUI();
            updatePayout();

            // initial direction active
            setDirectionClean('buy');

            // listeners
            btnBuy.addEventListener('click', () => setDirectionClean('buy'));
            btnSell.addEventListener('click', () => setDirectionClean('sell'));

            stakeInput.addEventListener('input', () => {
                updatePayout();
            });

            document.querySelectorAll('.quick-stake').forEach(el => {
                el.addEventListener('click', () => {
                    const val = el.getAttribute('data-stake');
                    stakeInput.value = val;
                    updatePayout();
                });
            });

            tradeBtn.addEventListener('click', placeTrade);

            // market tick every 1.8 seconds
            setInterval(() => {
                tickMarket();
                // also update payout display occasionally
                updatePayout();
            }, 1800);

            // initial price push to history after slight delay
            setTimeout(() => {
                pushPriceToHistory(currentPrice);
                updatePriceUI();
            }, 100);
        }

        // start
        init();
    })();
</script>
</body>
</html>
```

Core Trading Mechanics

The page simulates a real-time trading environment where you can test strategies without financial risk. Here's how it works:

· Market Simulation: A price chart updates every 1.8 seconds with a random walk, giving you a live market feel.
· Placing Trades: You can choose to BUY (UP) or SELL (DOWN). Enter a stake amount (using quick buttons or a custom value), and the potential payout is calculated instantly.
· Trade Outcome: When you place a trade, the system randomly determines a win or loss. A winning trade returns your stake plus an 85% profit. Your balance and a detailed trade history update immediately.
