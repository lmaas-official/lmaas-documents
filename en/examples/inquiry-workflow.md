# Example: Registering Summaries of Inquiries in an Internal System

> A hypothetical example written to explain how the features are used. The company name and contents are fictional. This is not a case study of a specific customer.

## Situation

- Parts manufacturer Company A (fictional) receives dozens of inquiries a day through the contact form on its website
- Staff read each message, categorize and summarize it, and enter it by hand into the internal case management system
- Inquiries include customers' company names, contact names and transaction details, so Company A does not want to send them to external AI services

## Flow

```
Contact form
      │ ① An inquiry arrives
      ▼
Company A's business system
      │ ② Sends the text to lmaas.io's API (authenticated with an API key)
      ▼
lmaas.io (an environment dedicated to Company A)
      │ ③ The AI returns a draft summary and category (with an AI-generated marker)
      ▼
Company A's business system
      │ ④ Registers the result in the case management system
      ▼
Staff check the content and respond
```

## Setup steps (overview)

1. An administrator chooses the AI model to use on lmaas.io
2. If needed, run additional training (LoRA) with past inquiries and example categories so the AI learns how Company A categorizes them
3. An administrator issues an API key
4. Add the code that calls the API to Company A's business system

## Example request to the AI

```
Summarize the following inquiry in this format:
- Type (quote / delivery date / defect / other)
- Key points (up to 3 lines)
- Whether it is urgent

Inquiry text:
(text here)
```

## Notes

- AI summaries and categories can be wrong. Staff should check them before responding
- If there are many inquiries or you need fast responses, a dedicated-GPU plan (Starter Plus, Business Plus) is a good fit
- Inquiry texts are processed inside the lmaas.io environment and are not sent to external AI services
