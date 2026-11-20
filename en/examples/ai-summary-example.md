# Example: Answers and Summaries Based on Internal Documents

> A hypothetical example written to explain how the features are used. The company name and rules are fictional. The AI's actual output varies with the model you choose and the documents you register.

## Situation

- The general affairs department of Company B (fictional) keeps receiving the same questions about travel expense claims
- Company B has registered its "Travel Expense Rules" (PDF) in lmaas.io and lets RAG refer to them

## Example question and answer

**User's question**

```
Do I get a daily allowance for a day trip?
```

**AI's answer (example)**

```
According to Article 8 of the Travel Expense Rules, a daily allowance is
paid for day trips as well, if the one-way travel distance is 100 km or more.
It is not paid for trips under 100 km. Please see the table attached to
that article for the amount.
(Reference: Travel_Expense_Rules.pdf)
```

* The articles and figures in these rules are fictional.

## Example summary

**User's request**

```
Summarize the Travel Expense Rules in 5 lines for new employees.
```

**AI's answer (example)**

```
1. Get your manager's approval before a business trip and apply in advance.
2. Transportation is reimbursed at actual cost, in principle via the most economical route.
3. Accommodation is reimbursed at actual cost, up to the limit for your position.
4. A daily allowance is paid for trips over a certain distance.
5. Submit your claim by the deadline after the trip ends.
```

## Tips for using it this way

- When the rules are revised, you can update only the RAG reference data. You can also go back to the previous version
- If you want consistent answer formats (for example, always citing the source), additional training (LoRA) with example answers can be effective
- AI answers can be wrong. Check important decisions against the original rules
