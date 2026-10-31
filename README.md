# Waroeng Batman - Bitcoin Grocery Store (LNbits TPoS Blueprint)

A practical blueprint for local grocery stores (UMKM/Warung in Indonesia) to accept Bitcoin via Lightning Network using the **LNbits TPoS (Touch Point of Sale)** extension.

## Key Features & Practical Solutions
* **Wholesale & Retail Categorization:** Clean product separation between bulk (*Sembako Borongan*) and retail (*Sembako Eceran*) items.
* **Volatility Buffer Pricing:** Product prices include a 5%–10% buffer over normal fiat (IDR) prices to protect low-margin grocery merchants from short-term Bitcoin volatility and swap fees.
* **Dynamic Shipping Trick (`Per Rp 1,000` Multiplier):** Since LNbits TPoS does not natively calculate courier rates, we created a base shipping unit (`Ongkir Per Rp 1.000`). Customers check shipping rates via WhatsApp, and add the multiplier accordingly (e.g., click `+` 15 times for Rp 15,000 shipping) to pay everything in a single Lightning invoice.

## How Other Merchants Can Copy This Setup
1. Open your **LNbits** dashboard and enable the **TPoS** extension.
2. Create a new TPoS and set currency to your local fiat (e.g., `IDR`).
3. Download our CSV file from this repository, click **IMPORT/EXPORT** inside your TPoS item list, and import the file to see our exact structure.
4. Share the watch-only TPoS link with your cashier or customers!
