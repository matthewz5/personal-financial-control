# Personal Financial Control Project

The objective of this project is to record, analyze, and monitor personal financial status, enabling effective expense management and cash flow tracking.

The records are divided into:

1. **INCOME** 💵 - Receipts from salaries and other transfers;
2. **EXPENSES** 💸 - Payments and spending made using credit or debit cards, such as PIX;
3. **BALANCE** ⚖️ - The temporal difference between recorded income and expenses.

---

## 📈 Income

Recorded data:

1. **Date** - Date - Date of receipt  
2. **Source** - String - Institution, company, or person of origin  
3. **Category** - String - Income category  
4. **Start_Date** - Date - Reference period (start)  
5. **End_Date** - Date - Reference period (end)  
6. **Amount** - Float - Amount of the income  

---

## 📉 Expenses

Recorded data:

1. **Date** - Date - Date of the expense  
2. **Time** - Hour - Time of the expense  
3. **Category** - String - Expense category for classification  
4. **Type** - String - Recurrence category, such as fixed, installment, or variable for any other  
5. **Source** - String - Credit or debit  
6. **Sub_Source** - String - Card or specific payment method  
7. **Location** - String - Place, store, or company where the expense was made  
8. **Item** - String - Product or service acquired or paid  
9. **Description** - String - Additional relevant information  
10. **Unit_Price** - Float - Unit price  
11. **Quantity** - Float - Quantity of product acquired or value with discount, for example  
12. **Total_Amount** - Float - Resulting value from Unit Price x Quantity  

---

## 💵 Balance

Resulting from the intersection of Income 📈 and Expenses 📉 data.

**Note**: Expenses with Credit Type in month X are usually paid in fact via Debit when the bill is paid in month X+1. In this case, the real balance analysis is done by accumulating expenses between the open bill dates, with payment on
