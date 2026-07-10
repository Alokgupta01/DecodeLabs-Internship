# Project 4 – AWS Lambda (Serverless Computing)

## 📌 Objective

Create an **AWS Lambda** function that accepts two numbers as input and returns their sum using **Python**. Verify the function execution through **Amazon CloudWatch Logs**.

## 🛠️ AWS Services Used

- AWS Lambda
- Amazon CloudWatch

## 💻 Programming Language

- Python 3.13

## 📝 Function Code

```python
def lambda_handler(event, context):
    num1 = event.get("num1", 0)
    num2 = event.get("num2", 0)

    total = num1 + num2

    return {
        "Sum": total
    }

## 📋 Steps Performed

1. Created an AWS Lambda function.
2. Selected **Python 3.13** as the runtime.
3. Wrote the Lambda function to calculate the sum of two numbers.
4. Created a test event with sample JSON input.
5. Invoked the Lambda function.
6. Verified the output returned by the function.
7. Monitored the execution logs using **Amazon CloudWatch Logs**.
   
## 💻 Technologies Used

- AWS Lambda
- Amazon CloudWatch
- Python 3.13
- AWS Management Console
  
## 🧪 Test Event

### Input

```json
{
  "num1": 15,
  "num2": 25
}

### Output

```json
{
  "Sum": 40
}

## 🚀 Features

- Serverless function execution
- No server management required
- Event-driven architecture
- Automatic scaling
- Execution logging with Amazon CloudWatch
  
## 📂 Project Structure

```text
project-4/
│── lambda_function.py
│── README.md
│── screenshots/
│   ├── lambda-function.png
│   ├── lambda-test-result.png
│   └── cloudwatch-logs.png
``
## ✅ Result

Successfully created and deployed an **AWS Lambda** function using **Python 3.13**. The function correctly calculated the sum of two input numbers and returned the expected output. The execution was successfully verified through **Amazon CloudWatch Logs**, confirming proper serverless function execution.
