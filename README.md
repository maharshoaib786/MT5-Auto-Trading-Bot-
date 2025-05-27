# MT5-Auto-Trading-Bot-
Auto Trading Boy by © MAHAR SHOAIB ©

"""
Grid-Martingale bot for MetaTrader 5 with phased Fibonacci and dynamic multipliers.
Uses LIMIT ORDERS for grid entries, with a configurable max number of pending grid orders per side.
Resets a side (cancels pending, resets Fib sequence) when any position on that side closes.
Console logging set to INFO. MT5 comments simplified.
Strict price validation for placing limit orders (buy below ask, sell above bid) has been REMOVED.
Orders will be placed at calculated levels; broker handles execution if price is already met.

• Phased lot sizing.
• Grid steps in pips.
• Grid entries via Limit Orders.
• Max Pending Grid Orders.
• Reset on Closure.
• Dynamic profit pips.
• Delay between entries.
• Auto-hedge (market orders).
• Profit Target (market orders).
• Proactive TP Sync.
• Configurable via .env.
"""
