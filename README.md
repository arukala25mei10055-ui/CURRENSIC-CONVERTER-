# CURRENSIC-CONVERTER-
SIMPLE COURRENSIC  CONVERTER IN PYTHON
  Currency Converter

A simple and fast Currency Converter application that converts one currency to another using live exchange rates.  
This project fetches real-time values from the *exchangerate.host* API (free, no API key needed).

---

##  Features
- Convert any currency to another
- Real-time exchange rates
- Clean and simple UI
- Supports all major world currencies
- Swap currency option
- Works in any browser
- No backend needed

---

##  Project Structure
## How to Use
1. Enter the amount you want to convert  
2. Select the *From Currency*  
3. Select the *To Currency*  
4. Click *Convert*  
5. View the result instantly

---

##  Live Demo (GitHub Pages)
You can host this project for free using *GitHub Pages*:
# Simple Offline Currency Converter (Basic Python)

rates = {
    "USD": 1.0,        # base currency
    "INR": 83.20,
    "EUR": 0.94,
    "GBP": 0.82,
    "AED": 3.67,
    "JPY": 157.12
}

def convert(amount, from_curr, to_curr):
    if from_curr not in rates or to_curr not in rates:
        return None
    # Convert to USD → then to target currency
    usd_value = amount / rates[from_curr]
    return usd_value * rates[to_curr]


print("=== Currency Converter ===")

amount = float(input("Enter amount: "))
from_currency = input("From currency (USD, INR, EUR, GBP, AED, JPY): ").upper()
to_currency = input("To currency (USD, INR, EUR, GBP, AED, JPY): ").upper()

result = convert(amount, from_currency, to_currency)

if result is None:
    print("Invalid currency")
else:
    print(f"\n{amount} {from_currency} = {result:.2f} {to_currency}")

1. Go to *Settings → Pages*
2. Select branch: *main*
3. Folder: *root*
4. Click *Save*

Your project will be live at:
