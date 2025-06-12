# Gemini-Binance-Live-Crypto-Price-Fetcher

A Python-based project that integrates Google Gemini (LLM) with the Binance API to fetch and display live cryptocurrency prices like Bitcoin (BTC) and Ethereum (ETH).

## 📌 Project Overview

This project demonstrates how to:
- Connect to Google Gemini (Generative AI) via API.
- Use the Binance REST API to fetch real-time cryptocurrency prices.
- Combine LLM-generated queries with external tool functions (like live price fetchers).
- Simulate function calling by Gemini to answer natural language questions with live data.

## ✅ Features

- 🔐 API key handling with `.env` and `python-dotenv`
- 🪙 Fetches live price data for any crypto symbol (e.g., BTCUSDT, ETHUSDT)
- 💬 Gemini model responds to price-related prompts
- 🔧 Function registered for future tool calling use
- 📡 Uses `requests` to call Binance’s ticker endpoint

---

## 📦 Technologies Used

| Tool/Library      | Purpose                              |
|------------------|--------------------------------------|
| `google.generativeai` | Gemini model integration       |
| `requests`        | Call Binance API                    |
| `dotenv`          | Securely store API keys             |
| `Binance API`     | Live cryptocurrency price data      |
| `Python`          | Main programming language           |

---

## 🚀 How It Works

1. Load Gemini API key from `.env`.
2. Connect to the `gemini-2.0-flash` model.
3. Create a `get_crypto_price(symbol)` function to fetch live prices from Binance.
4. Simulate Gemini's response using both:
   - LLM (for natural language)
   - Real price (from Binance)
5. Prepare for Gemini tool-calling by registering the function.

