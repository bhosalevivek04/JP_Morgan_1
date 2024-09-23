# JP_Morgan_1

## Overview

This repository contains a Java class, `RewardValue`, that represents a monetary reward that can be either in cash or miles.

## Usage

### Create a RewardValue object

You can create a `RewardValue` object using one of two constructors:

* `RewardValue(double cashValue)`: Creates a `RewardValue` object with the specified cash value.
* `RewardValue(double milesValue)`: Creates a `RewardValue` object with the specified miles value.

### Get the cash value

To get the cash value of a `RewardValue` object, use the `getCashValue()` method.

### Get the miles value

To get the miles value of a `RewardValue` object, use the `getMilesValue()` method.

### Convert miles to cash

You can convert the miles value of a `RewardValue` object to cash using the `convertMilesToCash()` method. This method uses a conversion rate of 0.0035, meaning that 1 mile is worth $0.0035.

## Example

The following code shows how to use the `RewardValue` class:

```java
// Create a RewardValue object with a cash value of $100.
RewardValue rewardValue = new RewardValue(100.0);

// Get the cash value of the RewardValue object.
double cashValue = rewardValue.getCashValue();

// Print the cash value.
System.out.println(cashValue); // Output: 100.0

// Create a RewardValue object with a miles value of 1000.
RewardValue rewardValue = new RewardValue(1000.0);

// Get the miles value of the RewardValue object.
double milesValue = rewardValue.getMilesValue();

// Print the miles value.
System.out.println(milesValue); // Output: 1000.0

// Convert the miles value of the RewardValue object to cash.
double cashValue = rewardValue.convertMilesToCash();

// Print the cash value.
System.out.println(cashValue); // Output: 35.0
```