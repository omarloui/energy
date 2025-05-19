# Data Pattern for Cyprus Energy Knowledge Document

**Version:** 1.1

## Electricity Tariffs in Cyprus

Residential three-time-period (effective April 1, 2025) from KIB-TEK:

| Period               | Hours       | Rate (TL/kWh) |
| -------------------- | ----------- | ------------- |
| **Day** (Puant)      | 07:00–17:00 | 13.7116       |
| **Peak**             | 17:00–23:00 | 13.7116       |
| **Night** (Off-Peak) | 23:00–07:00 | 9.9115        |

*Source: KIBRIS TÜRK ELEKTRİK KURUMU, Tariff tables (April 1, 2025)*

---

## Schema

* **question**

  * **Type:** string
  * **Description:** A user question regarding energy forecasting for a smart home in Cyprus.
* **answer**

  * **Type:** string
  * **Description:** The corresponding answer containing energy consumption and solar generation predictions along with calculated metrics.

## Required Fields

* question
* answer

---

## Detailed Kyrenia, Cyprus Weather Summary

Kyrenia exhibits a typical Mediterranean climate characterized by hot, dry summers and mild, wet winters. Below is a detailed summary based on historical records:

| Month     | Avg High (°C) | Avg Low (°C) | Precipitation (mm) | Sunshine Hours (approx.) | Relative Humidity (%) |
| --------- | ------------- | ------------ | ------------------ | ------------------------ | --------------------- |
| January   | 16            | 8            | 70                 | 150                      | 80                    |
| February  | 17            | 8            | 60                 | 160                      | 78                    |
| March     | 19            | 10           | 50                 | 180                      | 75                    |
| April     | 22            | 12           | 30                 | 210                      | 70                    |
| May       | 26            | 16           | 10                 | 250                      | 65                    |
| June      | 30            | 20           | 0                  | 280                      | 60                    |
| July      | 33            | 23           | 0                  | 300                      | 55                    |
| August    | 33            | 23           | 0                  | 300                      | 55                    |
| September | 31            | 21           | 10                 | 250                      | 60                    |
| October   | 27            | 17           | 30                 | 200                      | 65                    |
| November  | 22            | 12           | 50                 | 160                      | 75                    |
| December  | 18            | 10           | 70                 | 140                      | 80                    |

**Annual Summary:**

* **Average Temperature:** Approximately 18°C
* **Total Annual Precipitation:** \~400 mm
* **Sunshine:** Approximately 2,800 hours per year
* **Relative Humidity:** Around 70%

---

## Cloud Coverage Data Summary

Based on the provided cloud coverage CSV data (dataexport\_20250320T125219.csv), the average monthly cloud coverage in Kyrenia is estimated as follows:

| Month     | Average Cloud Coverage (%) |
| --------- | -------------------------- |
| January   | 80                         |
| February  | 75                         |
| March     | 65                         |
| April     | 55                         |
| May       | 40                         |
| June      | 30                         |
| July      | 25                         |
| August    | 25                         |
| September | 35                         |
| October   | 50                         |
| November  | 70                         |
| December  | 80                         |

**Summary:**
Kyrenia experiences high cloud coverage during the winter months (around 70–80%), which can limit solar generation during that period. Conversely, summer months show low cloud coverage (25–30%), supporting higher solar panel output. These cloud metrics, combined with the temperature and sunshine data, help in accurately forecasting both energy consumption (e.g., increased cooling needs during cloudy, humid periods) and the efficiency of solar generation.

---

## Smart Home Appliance Energy Consumption and Solar Generation Data

This section provides typical energy consumption values for common smart home appliances, as well as estimated solar panel generation for a 6kW installation in Cyprus.

### Appliance Energy Consumption

| Appliance       | Average Consumption        | Notes                                            |
| --------------- | -------------------------- | ------------------------------------------------ |
| Refrigerator    | 1.0 - 1.5 kWh per day      | Energy-efficient models use less power           |
| LED Lighting    | \~0.1 kWh per bulb per day | Total consumption depends on the number of bulbs |
| Washing Machine | 0.5 - 2 kWh per load       | Varies by model and cycle length                 |
| Air Conditioner | 1.5 - 2.5 kWh per hour     | Higher usage during peak summer                  |
| Television      | 0.1 - 0.3 kWh per hour     | Depends on screen size and usage                 |
| Laptop          | \~0.05 - 0.1 kWh per hour  | Typical usage during work hours                  |
| Dishwasher      | 1 - 2 kWh per cycle        | Energy use depends on cycle and efficiency       |

### Solar Panel Generation

For a typical 6kW solar panel system in Cyprus:

* **Monthly Generation:** Varies seasonally—from about 372 kWh in January to approximately 900–1,054 kWh in July.
* **Daily Generation:** On a sunny day, a 6kW system may produce between 12 and 20 kWh, depending on weather conditions.

### How This Data is Utilized

* **Energy Forecasting:**
  The weather and cloud coverage data combined with appliance consumption metrics help predict overall energy demand in a smart home.

* **Solar Generation Estimation:**
  Historical solar and cloud data inform the expected output from a 6kW system, which can then be compared against consumption values.

* **Cost and Efficiency Calculations:**
  Understanding appliance consumption and solar generation allows the computation of net energy costs, self-sufficiency ratios, and potential savings. For example, if solar generation covers a significant portion of your daily appliance usage, your dependence on grid power decreases, leading to cost savings.
