    # Biggest Atlantic Hurricanes 🌪️  

This project contains data on the most significant hurricanes in the Atlantic, including their category, damage, and maximum wind speeds.  

## 📊 Data Overview  

The dataset includes:  
- **Hurricane Name**  
- **Start Date**  
- **Damage (USD Millions)**  
- **Category (Saffir-Simpson Scale)**  
- **Max Wind Speed**  
![Screen Shot 2025-02-20 at 13 13 37](https://github.com/user-attachments/assets/99bd7229-6600-4b5b-b69a-19d5572d1c70)

### 🌀 Hurricane Categories  

The Saffir-Simpson Hurricane Wind Scale is used to categorize hurricanes based on wind speeds:  

| Category | Max Wind Speed (mph) |
|----------|----------------------|
| 5        | 157 and over         |
| 4        | 156                  |
| 3        | 129                  |
| 2        | 110                  |
| 1        | 95                   |

## 🛠️ Excel Switch Formula  

To categorize hurricanes automatically in Excel, the following `SWITCH` function can be used:  

```excel
=SWITCH(TRUE,  
    A2>=157, "Category 5 - Catastrophic",  
    A2>=130, "Category 4 - Extreme",  
    A2>=111, "Category 3 - Severe",  
    A2>=96, "Category 2 - Moderate",  
    A2>=74, "Category 1 - Weak",  
    "Not a Hurricane"
)
Replace A2 with the cell reference containing the wind speed.
    This formula assigns a hurricane category based on wind speed.

🚀 How to Use

    Open the Excel file.
    Add wind speed data in column A.
    Copy and paste the formula into column B to categorize hurricanes automatically.

