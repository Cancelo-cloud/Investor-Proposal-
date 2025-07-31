<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wealth Inc. (WIC) - Investment Profile</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 15px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            overflow: hidden;
        }
        
        .header {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: white;
            padding: 30px;
            text-align: center;
            position: relative;
        }
        
        .header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            font-weight: bold;
        }
        
        .targets-box {
            position: absolute;
            top: 20px;
            right: 20px;
            background: rgba(255,255,255,0.1);
            padding: 15px;
            border-radius: 10px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
            font-size: 0.9em;
        }
        
        .targets-box h4 {
            color: #ffd700;
            margin-bottom: 8px;
        }
        
        .bio {
            background: rgba(255,255,255,0.1);
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
        }
        
        .bio p {
            line-height: 1.6;
            font-size: 1.1em;
        }
        
        .highlight {
            color: #ffd700;
            font-weight: bold;
        }
        
        .divider {
            height: 3px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            margin: 0;
        }
        
        .main-content {
            padding: 30px;
        }
        
        .investment-grid {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 30px;
            margin-bottom: 40px;
        }
        
        .investment-column {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            color: white;
        }
        
        .investment-column.etfs {
            background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
        }
        
        .investment-column.crypto {
            background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);
        }
        
        .investment-column h3 {
            font-size: 1.5em;
            margin-bottom: 20px;
            text-align: center;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }
        
        .asset-list {
            list-style: none;
        }
        
        .asset-list li {
            background: rgba(255,255,255,0.2);
            margin: 8px 0;
            padding: 10px 15px;
            border-radius: 25px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.3);
            transition: transform 0.3s ease;
        }
        
        .asset-list li:hover {
            transform: translateY(-2px);
            background: rgba(255,255,255,0.3);
        }
        
        .bottom-section {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 30px;
            margin-top: 30px;
        }
        
        .info-box {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 25px;
            border-radius: 15px;
            color: white;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }
        
        .info-box h3 {
            color: #ffd700;
            margin-bottom: 15px;
            font-size: 1.3em;
        }
        
        .info-box ul {
            list-style: none;
        }
        
        .info-box li {
            margin: 8px 0;
            padding: 8px 0;
            border-bottom: 1px solid rgba(255,255,255,0.2);
        }
        
        .info-box li:last-child {
            border-bottom: none;
        }
        
        .frequency {
            color: #ffd700;
            font-weight: bold;
        }
        
        .tools-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }
        
        .tool-category {
            background: rgba(255,255,255,0.1);
            padding: 15px;
            border-radius: 10px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
        }
        
        .policy-link {
            background: rgba(255,255,255,0.1);
            padding: 10px 15px;
            border-radius: 8px;
            margin: 5px 0;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
            transition: all 0.3s ease;
        }
        
        .policy-link:hover {
            background: rgba(255,255,255,0.2);
            transform: translateX(5px);
        }
        
        @media (max-width: 768px) {
            .investment-grid,
            .bottom-section {
                grid-template-columns: 1fr;
            }
            
            .targets-box {
                position: static;
                margin-top: 15px;
            }
            
            .header h1 {
                font-size: 2em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Wealth Inc. (WIC)</h1>
            <div class="targets-box">
                <h4>🎯 Targets & Risk Management</h4>
                <div>Target: Min <strong>4% annually</strong></div>
                <div>Risk Limits: <strong>2% / 10% / 15%</strong></div>
                <div style="font-size: 0.8em; margin-top: 5px;">(Investor dependent)</div>
            </div>
            
            <div class="bio">
                <p><strong class="highlight">Wealth Inc. (WIC)</strong> is a 5-year investment company centered around one insight: <strong class="highlight">Follow human movement.</strong></p>
                <p>From the networks that fuel our connections to the vehicles that carry us forward, from the platforms that bridge distances to the technologies that chart our course — we invest in the <strong class="highlight">engines of human flow</strong> and the <strong class="highlight">innovations that pull us forward</strong>.</p>
                <p>Grounded in portfolio management and supercharged by AI, WIC turns this philosophy into performance — building capital by riding the currents of human flow and technological progress.</p>
            </div>
        </div>
        
        <div class="divider"></div>
        
        <div class="main-content">
            <div class="investment-grid">
                <div class="investment-column companies">
                    <h3>🏢 Companies</h3>
                    <ul class="asset-list">
                        <li>• Coinbase</li>
                        <li>• Realty Income</li>
                        <li>• JetBlue</li>
                        <li>• Tesla</li>
                        <li>• Uber</li>
                        <li>• Google</li>
                        <li>• YUM Brands</li>
                    </ul>
                </div>
                
                <div class="investment-column etfs">
                    <h3>📊 ETFs</h3>
                    <ul class="asset-list">
                        <li>• ARKK</li>
                        <li>• SOXX</li>
                        <li>• LIT</li>
                        <li>• IDNV</li>
                        <li>• IYN</li>
                        <li>• SPDR</li>
                    </ul>
                </div>
                
                <div class="investment-column crypto">
                    <h3>₿ Crypto</h3>
                    <ul class="asset-list">
                        <li>• ETH</li>
                        <li>• ECID</li>
                        <li>• (Additional assets TBD)</li>
                    </ul>
                </div>
            </div>
            
            <div class="bottom-section">
                <div class="info-box">
                    <h3>📈 Reporting Schedule</h3>
                    <ul>
                        <li><span class="frequency">Weekly:</span> Big decisions - New investments or selling positions (48hr intervention window)</li>
                        <li><span class="frequency">Monthly:</span> General portfolio updates and market analysis</li>
                        <li><span class="frequency">Quarterly:</span> Portfolio status, strategic changes, performance review</li>
                        <li><span class="frequency">Yearly:</span> Annual targets, comprehensive review, strategy adjustment</li>
                    </ul>
                </div>
                
                <div class="info-box">
                    <h3>🔧 Technical & Fundamental Tools</h3>
                    <div class="tools-grid">
                        <div class="tool-category">
                            <strong>Technical Analysis:</strong>
                            <div>• Moving Averages</div>
                            <div>• RSI & MACD</div>
                            <div>• Support/Resistance</div>
                            <div>• Volume Analysis</div>
                        </div>
                        <div class="tool-category">
                            <strong>Fundamental Analysis:</strong>
                            <div>• P/E Ratios</div>
                            <div>• Revenue Growth</div>
                            <div>• Market Position</div>
                            <div>• AI-Enhanced Screening</div>
                        </div>
                    </div>
                </div>
                
                <div class="info-box">
                    <h3>📋 Policies & Documentation</h3>
                    <div class="policy-link">📄 Quarterly Pay Structure</div>
                    <div class="policy-link">💰 Fee Schedule & Transparency</div>
                    <div class="policy-link">⚖️ Risk Management Framework</div>
                    <div class="policy-link">📊 Performance Benchmarks</div>
                    <div class="policy-link">🔒 Asset Protection Policy</div>
                    <div class="policy-link">📞 Investor Communication Protocol</div>
                    <div class="policy-link">🎯 Investment Philosophy & Strategy</div>
                    <div class="policy-link">📈 Exit Strategy Guidelines</div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
