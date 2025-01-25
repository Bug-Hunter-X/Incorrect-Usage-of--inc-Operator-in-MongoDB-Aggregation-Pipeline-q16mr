# Incorrect Usage of $inc Operator in MongoDB Aggregation Pipeline
This repository demonstrates a common error when using the `$inc` operator within a MongoDB aggregation pipeline. The `$inc` operator is intended to increment a numeric field, but it's incorrectly used in this example.  The correct approach involves using the `$addFields` stage. 

## Problem
The provided `bug.js` demonstrates incorrect usage of `$inc` within the pipeline. This results in unexpected and incorrect counts.

## Solution
The `bugSolution.js` file shows the correct way to increment the count using the `$addFields` stage in the MongoDB aggregation pipeline.

## How to reproduce
1. Clone this repository.
2. Ensure you have a MongoDB instance running and a collection populated with some data.
3. Run `bug.js` and observe the incorrect output.
4. Run `bugSolution.js` and observe the correct output.