# How lmaas.io Differs from Other Options

Last checked: 2026-11-12 (Japanese original)

There are several ways to use generative AI at work. This page organizes the differences in approach. It does not evaluate the performance or features of any specific company's service. Company names and trademarks belong to their respective owners.

## Options compared

| | General-purpose AI chat services (ChatGPT, Gemini, etc.) | Running open models on your own GPU servers | lmaas.io |
|---|---|---|---|
| General questions and writing | ◎ | Depends on the model | ○ (depends on the model) |
| Searching and referring to internal documents | △ | Build it yourself | ◎ (RAG included in every plan) |
| Adapting to your wording and terminology | △ | Build your own training setup | ◎ (additional training and versioning) |
| Not sending data to external AI services | Sent | Not sent | Not sent (except when you set up external connections) |
| Preparing and maintaining GPU servers | Not needed | Needed | Not needed |
| Choice of AI models | Models provided by the service | Free choice | Choose from over 1,000 (each plan has a size limit) |
| Managing users and connections | Depends on the service's plan | Build it yourself | Administrators manage users and connections |
| Cost structure | Often priced by number of users or usage | Hardware, electricity and maintenance staff | Fixed monthly price (plus an initial fee) |

The table is a rough guide to the approaches. ◎, ○ and △ do not indicate the superiority or inferiority of any service's performance.

## Reasons customers tend to choose lmaas.io

- They do not want to send internal documents or customer information to external AI services
- They want to use open models but do not want to prepare and maintain GPU servers
- They want to grow an AI for their company by combining internal document reference and additional training
- They want predictable costs with a fixed monthly price

## When other options may fit better

- If the performance of the latest and largest general-purpose AI is your top priority, a general-purpose AI chat service is a better fit
- If you want complete freedom over model size and configuration, or want to run it only inside your internal network, preparing your own GPU servers is a better fit (lmaas.io is a cloud service)
- For a small team handling information that is not confidential, a general-purpose AI chat service may be cheaper

## Choosing between lmaas.io plans

| Deciding factor | How to choose |
|---|---|
| Model size you want to use | 4B class → Personal, 8B class → Starter / Starter Plus, 24B class → Business, 32B class → Business Plus |
| Response speed | If you need consistent speed, a dedicated GPU (Starter Plus, Business Plus) |
| Number of users | Personal 1, Starter 3, Starter Plus / Business up to 10 |
| Administrator review of conversations | Business and Business Plus only |
| Training frequency | If you train often, a dedicated-GPU plan, which offers training-only mode |
