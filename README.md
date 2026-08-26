# Lambda-project4
# 🚀 Project 4 – The Serverless Logic

## AWS Lambda – Cost Calculator

### 📌 Project Overview

This project demonstrates the implementation of a serverless backend using AWS Lambda.

A Python-based Lambda function is created to accept two numbers through a JSON event, calculate their sum, and return the result as a JSON response.

The project also demonstrates Lambda testing and execution monitoring using Amazon CloudWatch Logs.

---

## 🎯 Objectives

- Create a serverless function using AWS Lambda
- Configure a Python runtime
- Accept input through a JSON event
- Perform a calculation using Python
- Return the result in JSON format
- Test the Lambda function with different inputs
- Monitor Lambda execution using CloudWatch

---

## 🛠️ Technologies Used

- AWS Lambda
- Python 3
- Amazon CloudWatch
- JSON
- AWS Management Console

---

## ⚙️ Lambda Function

**Function Name:** `CostCalculator`

**Runtime:** Python 3.x

The Lambda function receives two numbers, `num1` and `num2`, from the event and calculates their sum.

### Python Code

python
def lambda_handler(event, context):
    num1 = event.get("num1")
    num2 = event.get("num2")
    total = num1 + num2
    return {
        "Sum": total
    }




🧪 Test Case 1

Input:

{
  "num1": 15,
  "num2": 25
}

Output:

{
  "Sum": 40
}

Status: ✅ Successful


---

🧪 Test Case 2

Input:

{
  "num1": 100,
  "num2": 250
}

Output:

{
  "Sum": 350
}

Status: ✅ Successful


---

☁️ CloudWatch Monitoring

Amazon CloudWatch Logs were used to verify the execution of the Lambda function.

The execution logs provide information such as:

1) START request

2) END request

3) REPORT information

4) Execution duration

5) Billed duration

6) Memory usage


This confirms that the Lambda function was successfully invoked and executed.


---

📊 Project Results

Test	Input	Expected Output Status

Test 1	15 + 25	Sum =  40  ✅ Successful

Test 2	100 + 250	Sum = 350	✅ Successful



---

🎓 Learning Outcomes

Through this project, I learned:

How to create and configure an AWS Lambda function

How to write serverless logic using Python

How to work with JSON events

How to test Lambda functions

How to verify function outputs

How to monitor Lambda executions using CloudWatch

How serverless computing works without managing a traditional server



---

✅ Conclusion

The CostCalculator Lambda function was successfully created and tested.

Both test cases returned the expected results, and the Lambda execution was verified using Amazon CloudWatch Logs.

Project 4 – The Serverless Logic successfully completed. 🚀
