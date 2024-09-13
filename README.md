# Credit Card Fraud Detection

## Introduction
This project focuses on detecting fraudulent credit card transactions using a dataset that contains transaction, card usage, and customer details. The goal is to explore transaction patterns and build a machine learning model to predict fraud.

## Dataset Overview
- **Format**: JSON (saved as text file)
- **Rows**: 786,363
- **Columns**: 29
- **Source**: kaggle

## Column Descriptions
| Column Name               | Description                                                 |
|---------------------------|-------------------------------------------------------------|
| `accountNumber`            | Unique ID for the credit card account                       |
| `customerId`               | Unique customer identifier                                  |
| `creditLimit`              | Maximum credit limit available for the account              |
| `availableMoney`           | Remaining balance of credit after transactions              |
| `transactionDateTime`      | Timestamp of the transaction (YYYY-MM-DDTHH:MM:SS)          |
| `transactionAmount`        | Amount spent in the transaction                             |
| `merchantName`             | Merchant where the transaction occurred                     |
| `acqCountry`               | Country of the acquiring bank                               |
| `merchantCountryCode`      | Merchant's country code                                     |
| `posEntryMode`             | Mode of card entry (e.g., swipe, chip)                      |
| `posConditionCode`         | Condition of the transaction (e.g., in-store, online)       |
| `merchantCategoryCode`     | Type of merchant (e.g., rideshare, restaurant)              |
| `currentExpDate`           | Card expiration date (MM/YYYY)                              |
| `accountOpenDate`          | Date when the account was opened                            |
| `dateOfLastAddressChange`  | Date of the last address update on the account              |
| `cardCVV`                  | Security CVV code of the card                               |
| `enteredCVV`               | CVV code entered during the transaction                     |
| `cardLast4Digits`          | Last four digits of the credit card                         |
| `transactionType`          | Type of transaction (e.g., purchase, refund)               |
| `currentBalance`           | Current balance on the credit card account                  |
| `merchantCity`             | Merchant's city location                                    |
| `merchantState`            | Merchant's state location                                   |
| `merchantZip`              | Merchant's ZIP/postal code                                  |
| `cardPresent`              | Whether the card was physically present during the transaction |
| `posOnPremises`            | Whether the transaction occurred on the merchant's premises |
| `recurringAuthInd`         | Indicates if the transaction is a recurring authorization   |
| `expirationDateKeyInMatch` | Whether the entered expiration date matched the actual card |
| `isFraud`                  | Whether the transaction is flagged as fraud                 |


## Data Cleaning
The data needs to be cleaned before performing any analysis or building a model. The following steps outline the data-cleaning process:

1. **Remove Missing or Invalid Data**
2. **Handle Duplicates**
3. **Fix Columns Types**
4. **Outlier Detection**
5. **Normalize/Scale Data**

## Exploratory Data Analysis (EDA)
This project aims to uncover the following insights:
- Patterns in transaction amounts (e.g., large or unusual purchases)
- Multiple card swipes in short timeframes
- Amount reversals or chargebacks
- Fraud trends based on transaction time, location, and card usage

## Modeling
We will use various machine learning techniques (e.g., logistic regression, decision trees, random forests) to predict fraudulent transactions. Performance metrics such as accuracy, precision, recall, and F1 score will be used to evaluate the models.

## Installation/Usage

### Prerequisites
- Python 3.x
- Install dependencies via pip:
    ```bash
    pip install -r requirements.txt
    ```

### Run EDA
1. To perform exploratory data analysis:
    ```bash
    python eda.py
    ```

### Train Model
2. To train the machine learning model:
    ```bash
    python train_model.py
    ```

## License
This project is licensed under the MIT License.
