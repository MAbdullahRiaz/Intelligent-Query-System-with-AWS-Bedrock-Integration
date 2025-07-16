# Intelligent-Query-System-with-AWS-Bedrock-Integration
Architecture that uses Amazon Bedrock and other AWS services to process user queries, invoke foundation models, and return responses through an API endpoint. Designed for testing via Postman, with potential real-time interaction through a hosted API gateway.

# AWS Bedrock GenAI Use Case – API Gateway + Lambda + Cohere LLM

This project demonstrates how to build a serverless Generative AI application using:

- ✅ Amazon Bedrock (Cohere model)
- ✅ AWS Lambda for orchestration
- ✅ Amazon API Gateway to expose REST endpoint
- ✅ Input prompt + summarized response lifecycle

---

## 📊 Architecture

![Architecture Diagram](./architecture/Architecture_Diagram.png)

---

## 🚀 How it Works

1. The user sends a prompt via a REST API.
2. API Gateway routes the request to an AWS Lambda function.
3. The Lambda function invokes a foundational LLM hosted on Amazon Bedrock (e.g., Cohere or can be chosen).
4. The model responds with a summarized output, which is returned to the user.

---

## 🔧 Tech Stack

- **AWS Lambda**
- **Amazon Bedrock**
- **API Gateway**
- **Cohere Foundation Model**
- **Python (Boto3 SDK)**

---

## 🧪 Sample Prompt (test_prompts/sample_prompt.json)

```json
{
  "prompt": "Summarize the impact of generative AI on education."
}
