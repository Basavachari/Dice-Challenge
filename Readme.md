

---

# Securin - The Doomed Dice Challenge

## Author: Basava Chari Boppudi

## Part A: Total Combinations and Probability Distribution

### Total Combinations Calculation:

For each die, there are 6 possibilities. Since there are 2 dice, the total combinations are calculated as follows:

Total Combinations = 6 * 6 = 36

### Probability Distribution:

Calculated and displayed the distribution of all possible combinations that can be obtained when rolling both Die A and Die B together. Here's the distribution matrix:

```
A/B  |   1     2     3     4     5     6
------------------------------------------
1    | (1,1) (1,2) (1,3) (1,4) (1,5) (1,6)
2    | (2,1) (2,2) (2,3) (2,4) (2,5) (2,6)
3    | (3,1) (3,2) (3,3) (3,4) (3,5) (3,6)
4    | (4,1) (4,2) (4,3) (4,4) (4,5) (4,6)
5    | (5,1) (5,2) (5,3) (5,4) (5,5) (5,6)
6    | (6,1) (6,2) (6,3) (6,4) (6,5) (6,6)
```

### Probability Calculation:

Calculated the probability of all possible sums occurring among the number of combinations. The probability distribution for sums 2 to 12 is as follows:

```
P(Sum = 2)  = 1/36
P(Sum = 3)  = 2/36
P(Sum = 4)  = 3/36
P(Sum = 5)  = 4/36
P(Sum = 6)  = 5/36
P(Sum = 7)  = 6/36
P(Sum = 8)  = 5/36
P(Sum = 9)  = 4/36
P(Sum = 10) = 3/36
P(Sum = 11) = 2/36
P(Sum = 12) = 1/36
```

## Part B: Reconstructing Face Values

### Problem Statement:

Reconstructed face values for two dice (Die A and Die B) after their spots have been removed. The constraints include Die A's faces not having more than 4 spots, Die A having repeated face values, Die B having values greater than 6, and the probability of each possible sum (2-12) remaining the same as with standard 6-sided dice.

### Solution Logic:

1. **Determine Possible Sum Range:**
   Identified the range of 2-12 based on the minimum and maximum face values.

2. **Fix Certain Values:**
   Placed 1 in both Die A and Die B to ensure sum 2 is possible. Placed 4 in Die A and 8 in Die B to ensure sum 12 is possible (due to Die A's maximum value is 4).

3. **Fill Remaining Spots:**
   - For Die A: Only 2 and 3 can be used to fill remaining spots to maintain probability constraints. The correct combination is 2, 2, 3, 3.
   - For Die B: Values must be less than 8 to avoid sums exceeding 12. The only combination that works is 6, 5, 4, 3.

4. **Final Assignments:**
   - Die A: {1, 4, 2, 2, 3, 3}
   - Die B: {1, 8, 6, 5, 4, 3}

### Final Sum Matrix:

The final sum matrix was generated, ensuring the frequency of each sum remains the same as before transformation.

```
A/B  | 1  2  2  3  3  4
------------------------
1    | 2  3  3  4  4  5
3    | 4  5  5  6  6  7
4    | 5  6  6  7  7  8
5    | 6  7  7  8  8  9
6    | 7  8  8  9  9  10
8    | 9  10 10 11 11 12
```



## Conclusion:

In this assignment, we successfully determined total combinations, calculated probability distributions, and reconstructed face values for two dice while maintaining the same probability constraints. The code is available in the [GitHub repository](https://github.com/Basavachari/Dice-Challenge) for reference.

---

Feel free to modify this template according to your assignment details, and include additional sections or details as needed.