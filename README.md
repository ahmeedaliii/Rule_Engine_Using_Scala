# Scala-Discounts-Real-Time-Rule-Engine

## Overview
This Scala project is designed to handle discounts for orders based on various qualifying rules. It reads order data from a CSV file, applies discounts according to predefined rules, calculates final prices, and inserts the processed data into a database. Additionally, it includes logging functionality to track the processing flow and outcomes.

## Function Programming Approach
The project is implemented using a functional programming approach to ensure modularity, composability, and immutability of code. Functional programming principles such as immutability, higher-order functions, and pure functions are employed to enhance code readability, maintainability, and scalability.

## Features
- **Order Processing**: Parses order data from a CSV file into Order objects.
- **Discount Calculation**: Applies discounts based on several qualifying rules such as expiry date, product category, quantity, channel, and payment method.
- **Logging**: Provides logging functionality to record processing events and outcomes, aiding in debugging and monitoring.
- **Database Interaction**: Inserts the processed order data into a database for further analysis and reporting.

## Qualifying Rules
The project implements the following qualifying rules for discounts:

1. **Expiry Date**: Discounts are applied if the expiry date is less than 30 days from the order date.
2. **Product Category**: Discounts are applied to products categorized as "Cheese" or "Wine".
3. **Order Date**: Discounts are applied if the order date falls on the 23rd of March.
4. **Quantity**: Discounts are applied based on the quantity of products ordered.
5. **Channel**: Additional discounts are offered for orders made through the "App" channel.
6. **Payment Method**: Discounts are offered for orders paid with a "Visa" card.

