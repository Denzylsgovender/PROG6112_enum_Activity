# 🏦 Java Enum Activity: Bank Account Type Selector

## 📘 Overview

In this activity, you'll build a **bank account registration system** using the Java `enum` type. This will help you learn how to:

✅ Declare and use enums  
✅ Store enum values in classes  
✅ Use `switch` statements with enums  
✅ Apply enum methods 
✅ Add descriptions to enum constants (Bonus)

---

## 🌍 Real-World Scenario

You're developing a system for a **bank** where users can open different types of accounts. The system must only allow predefined account types:

- **SAVINGS**
- **CURRENT**
- **FIXED_DEPOSIT**

These account types are stored using the `enum` type for safety, readability, and consistency.

---

## 🎯 Learning Outcomes

By completing this task, you’ll be able to:

| Objective                                      | Outcome                                 |
|-----------------------------------------------|------------------------------------------|
| ✅ Use `enum` in Java                          | Store constant values like account types |
| ✅ Use enum in a class                         | Use `AccountType` inside `BankAccount`   |
| ✅ Use `.name()`, `.ordinal()`, `.values()`    | Display info and loop through enum values |
| ✅ Use enums in a `switch` statement           | Perform actions based on enum selection |
| ✅ Add fields and methods to enums *(Bonus)*   | Attach descriptions to each constant     |

---

## 🧱 Step-by-Step Instructions

### 🔹 Step 1: Create the `enum` AccountType

```java
enum AccountType {
    SAVINGS, CURRENT, FIXED_DEPOSIT
}
---

### 🔹 Step 2: Create the BankAccount Class
```java

class BankAccount {
    String holderName;
    AccountType accountType;

    public BankAccount(String holderName, AccountType accountType) {
        this.holderName = holderName;
        this.accountType = accountType;
    }

    public void displayDetails() {
        System.out.println("Account Holder: " + holderName);
        System.out.println("Account Type: " + accountType.name());
    }
}

