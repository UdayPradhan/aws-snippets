
# Lambda Arithmetic Expression Evaluator

This AWS CloudFormation template creates a Lambda function that evaluates arithmetic expressions provided as strings and outputs the result in the stack outputs.

## Overview

The template deploys a Lambda function written in Python that can parse and evaluate basic arithmetic expressions. It demonstrates how to use AWS Lambda for simple computational tasks and how to integrate it with CloudFormation outputs.

## Features

- Evaluates arithmetic expressions containing addition, subtraction, multiplication, and division
- Handles parentheses for expression grouping
- Returns the result through CloudFormation outputs

## Usage

1. Deploy the CloudFormation template in your AWS account.
2. Once the stack is created, you can find the Lambda function in the AWS Lambda console.
3. The arithmetic expression to be evaluated is set as an environment variable for the Lambda function.
4. The result of the evaluation will be available in the CloudFormation stack outputs.

## Parameters

- `ArithmeticExpression`: The arithmetic expression to evaluate (e.g., "2 + 3 * (4 - 1)")

## Outputs

- `LambdaReturnValue`: The result of evaluating the provided arithmetic expression

## Limitations

- The Lambda function supports basic arithmetic operations (+, -, *, /) and parentheses.
- It does not handle more complex mathematical functions or operations.
- The expression must be valid and well-formed to avoid errors.

## Security

Ensure that you review and adjust the IAM roles and permissions as needed for your specific use case and security requirements.

## Customization

You can modify the Lambda function code to add more operations or enhance the expression evaluation capabilities as needed.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
