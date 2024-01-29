The 128 64 32 16 8 4 2 1 chart is a common method used to convert decimal numbers to binary². Here's how you can use it:

1. Write down the numbers 128, 64, 32, 16, 8, 4, 2, and 1 in a row.
2. Start from the left (128) and proceed to the right, asking if your decimal number is greater than or equal to each number in the row.
3. If it is, write down a `1` under that number and subtract that number from your decimal number.
4. If it isn't, write down a `0` under that number.
5. Repeat this process until you reach the end of the row.

For example, let's convert the decimal number 13 to binary:

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|-----|----|----|----|---|---|---|---|
| 0   | 0  | 0  | 0  | 1 | 1 | 0 | 1 |

Here, 13 is less than 128, 64, 32, and 16, so we write `0` under these numbers. 13 is greater than 8, so we write `1` under 8 and subtract 8 from 13, leaving us with 5. 5 is greater than 4, so we write `1` under 4 and subtract 4 from 5, leaving us with 1. 1 is less than 2, so we write `0` under 2. Finally, 1 is equal to 1, so we write `1` under 1. The binary equivalent of 13 is therefore `00001101`.

Please note that this method works for decimal numbers up to 255. For larger numbers, you would need to extend the chart with larger powers of 2².