# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## NAME : JAI HARISH R
## REG NO : 212224040124

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

Accuracy

Coherence

Simplicity

Speed

User experience

## Algorithm


## Step 1: Select the Topic

Choose a technical article to summarize using different Generative AI prompting techniques.

**Selected Topic:** “The Basics of Blockchain Technology”

The selected article covers the following concepts:

- Definition and fundamentals of blockchain
- Decentralized ledger technology
- Blocks and cryptographic hashing
- Consensus mechanisms
- Applications of blockchain technology
- Advantages and challenges of blockchain

## Step 2: Choose AI Platforms

The following Generative AI platforms are selected for the experiment:

- ChatGPT
- Google Gemini
- Claude AI
- Microsoft Copilot

These platforms are used to generate summaries of the same blockchain article and compare their responses.

## Step 3: Prepare Prompting Techniques

Four prompting techniques are used to evaluate how different instructions influence the quality of AI-generated summaries.

### A. Zero-Shot Prompting

Zero-shot prompting involves asking the AI to perform a task without providing any examples.

**Example Prompt:**

“Summarize the following article on blockchain technology in simple language suitable for undergraduate students. Include the main concepts and important applications.”

### B. Few-Shot Prompting

Few-shot prompting involves providing a small number of examples to help the AI understand the expected summary format and writing style.

**Example Prompt:**

“Example 1: Summarize a technical article by explaining its definition, working principle, applications, and limitations in simple language.

Example 2: Summarize a technical article in one concise paragraph, highlighting its key concepts and practical uses.

Now, summarize the following article on blockchain technology using a similar style.”

### C. Chain-of-Thought Prompting

This technique encourages the AI to identify important concepts and organize its approach before producing the final summary. The task can be structured into clear intermediate steps without requiring the model to reveal private internal reasoning.

**Example Prompt:**

“Analyze the blockchain article by identifying its main concepts, working principles, applications, advantages, and challenges. Use these points to prepare a clear, concise, and well-organized summary for undergraduate students.”

### D. Role-Based Prompting

Role-based prompting assigns a specific role or professional perspective to the AI to guide its tone, vocabulary, and level of explanation.

**Example Prompt:**

“Act as a university professor specializing in computer science. Summarize the following article on blockchain technology in simple, technically accurate language suitable for undergraduate students. Include its fundamental concepts, applications, advantages, and limitations.”

## Step 4: Generate Responses

The same blockchain article is provided to each selected AI platform. Each of the four prompting techniques is tested separately using the corresponding prompt.

The generated summaries are collected and recorded for comparison. To ensure a fair evaluation, the article content, task requirements, and output length expectations are kept consistent across platforms.

The experiment includes the following combinations:

- Zero-Shot Prompting with each AI platform
- Few-Shot Prompting with each AI platform
- Chain-of-Thought Prompting with each AI platform
- Role-Based Prompting with each AI platform

## Step 5: Organize and Evaluate Results

The generated summaries are compared using the following evaluation criteria:

- **Accuracy:** Whether the summary correctly represents the technical concepts in the original article.
- **Coherence:** Whether the information is logically organized and easy to follow.
- **Simplicity:** Whether the summary is understandable to undergraduate students.
- **Completeness:** Whether the summary includes the major concepts without omitting essential information.
- **Response Time:** How long each AI platform takes to generate the summary.
- **User Experience:** How useful, readable, and relevant the generated summary is to the intended audience.


# PROMPTS

## Prompt Type 1: Zero-Shot Prompting

### Prompt:
```text
Read the 500-word technical article titled "The Basics of Blockchain Technology" and produce a concise summary for undergraduate students. Explain the fundamental concept, how blockchain works, its major applications, advantages, and limitations. Use simple language without omitting essential technical information.
```

#### Tool A: ChatGPT (OpenAI)

**Output:** ChatGPT summarized blockchain as a decentralized digital ledger that records transactions in linked blocks. It explained cryptographic hashing, transaction validation, and applications such as cryptocurrencies, while mentioning security benefits and scalability challenges.

#### Tool B: Gemini (Google)

**Output:** Gemini described blockchain as a distributed system in which information is shared across multiple computers. It highlighted decentralization, transparency, secure transactions, and applications in finance and supply chain management.

#### Tool C: Claude (Anthropic)

**Output:** Claude presented blockchain as a shared digital record maintained by a network of participants. It explained how blocks are linked using cryptography and outlined benefits such as transparency and limitations such as energy consumption in certain consensus systems.

#### Tool D: Microsoft Copilot

**Output:** Copilot summarized blockchain as a decentralized record-keeping technology that uses cryptographic techniques to protect transaction data. It highlighted applications in digital currencies, identity management, and supply chains, along with challenges involving scalability and regulation.

## Prompt Type 2: Few-Shot Prompting

### Prompt:
```text
Use the following example to understand the expected summary style.

Example:
Topic: Cloud Computing
Summary: Cloud computing provides computing services such as storage, servers, and software over the internet. It offers flexibility and scalability but may introduce security and privacy concerns.

Now summarize the article "The Basics of Blockchain Technology" in a similar style. Include its definition, working principle, applications, advantages, and challenges in approximately 100 words. Write for undergraduate students.
```

#### Tool A: ChatGPT (OpenAI)

**Output:** ChatGPT described blockchain as a decentralized digital ledger that stores transactions in linked, cryptographically secured blocks. It explained how network participants validate transactions and identified uses in cryptocurrency, finance, and supply chains. The summary highlighted transparency and tamper resistance while noting scalability, energy consumption, and regulatory concerns.

#### Tool B: Gemini (Google)

**Output:** Gemini explained blockchain as a distributed database that maintains transaction records across a network. It described blocks, cryptographic links, and consensus mechanisms. The summary covered applications such as digital payments and supply chain tracking, along with benefits including transparency and challenges involving performance and implementation costs.

#### Tool C: Claude (Anthropic)

**Output:** Claude summarized blockchain as a shared ledger in which transactions are grouped into blocks and linked through cryptographic hashes. It highlighted distributed verification, reduced dependence on central authorities, and applications in finance and digital identity. It also mentioned privacy, scalability, and energy-related concerns.

#### Tool D: Microsoft Copilot

**Output:** Copilot described blockchain as a decentralized technology for recording and verifying transactions. It outlined the role of cryptographic hashing and network consensus, with examples from cryptocurrencies and logistics. The summary emphasized transparency and data integrity while acknowledging adoption barriers, regulatory uncertainty, and performance limitations.

## Prompt Type 3: Chain-of-Thought Prompting

### Prompt:
```text
Examine the article "The Basics of Blockchain Technology" using the following structure:

1. Identify the main definition and purpose of blockchain.
2. Explain how blocks, cryptographic hashing, and consensus mechanisms work together.
3. Identify the major applications, advantages, and limitations.
4. Use these findings to produce a concise, logically organized summary for undergraduate students.

Present the key points and final summary clearly, using simple and technically accurate language.
```

#### Tool A: ChatGPT (OpenAI)

**Output:** ChatGPT organized the summary around blockchain's purpose, technical operation, applications, and limitations. It explained that transactions are grouped into blocks, linked using cryptographic hashes, and validated through a consensus mechanism. It concluded with examples in cryptocurrency and supply chain tracking, noting scalability and energy challenges.

#### Tool B: Gemini (Google)

**Output:** Gemini structured the summary by describing blockchain's decentralized design, transaction verification, and links between blocks. It explained how consensus helps participants agree on valid records and highlighted applications in finance, logistics, and digital identity. It also noted that performance and implementation requirements vary across blockchain systems.

#### Tool C: Claude (Anthropic)

**Output:** Claude presented the topic in a connected explanation, moving from the distributed ledger concept to cryptographic linking and transaction validation. It discussed the benefits of shared records and tamper resistance, followed by applications in finance and supply chains. It also identified privacy, scalability, and governance as important considerations.

#### Tool D: Microsoft Copilot

**Output:** Copilot organized the explanation into blockchain fundamentals, working principles, applications, and challenges. It described how network participants validate transactions and how cryptographic hashes connect blocks. It highlighted uses in digital currencies and record tracking, while noting that blockchain does not automatically eliminate every security or trust problem.

## Prompt Type 4: Role-Based Prompting

### Prompt:
```text
Act as an experienced computer science lecturer preparing learning material for first-year undergraduate students. Summarize the article "The Basics of Blockchain Technology" in accessible academic language. Explain the concept using a simple real-world analogy, describe its main technical components, and discuss its applications, benefits, and limitations. Keep the explanation concise, accurate, and engaging.
```

#### Tool A: ChatGPT (OpenAI)

**Output:** ChatGPT used a classroom-friendly explanation, comparing blockchain to a shared digital notebook whose entries are linked and validated by a network. It introduced cryptographic hashes and consensus, followed by applications in Bitcoin and supply chain management. It also explained that blockchain systems can face scalability and energy challenges.

#### Tool B: Gemini (Google)

**Output:** Gemini adopted an instructional tone and explained blockchain as a shared record that multiple computers maintain. It described blocks, cryptographic security, and consensus mechanisms, using examples from digital payments and logistics. It concluded by discussing transparency, reduced dependence on central authorities, and implementation challenges.

#### Tool C: Claude (Anthropic)

**Output:** Claude provided a structured educational summary using straightforward definitions and a shared-record analogy. It explained how transactions are verified and linked, then discussed uses in finance, identity management, and supply chains. It balanced the benefits of data integrity and transparency against privacy, scalability, and governance concerns.

#### Tool D: Microsoft Copilot

**Output:** Copilot presented blockchain as a digital record book shared among network participants. It explained how cryptographic hashes connect blocks and how consensus helps validate transactions. It included examples such as cryptocurrency and product tracking, while emphasizing that blockchain's suitability depends on cost, performance, and the application's requirements.

# Evaluation


| Prompting Technique | AI Platform | Accuracy | Coherence | Simplicity | Speed    | User Experience |
| ------------------- | ----------- | -------- | --------- | ---------- | -------- | --------------- |
| Zero-Shot           | ChatGPT     | High     | High      | High       | Fast     | Very Good       |
| Zero-Shot           | Gemini      | High     | High      | High       | Fast     | Very Good       |
| Zero-Shot           | Claude      | High     | High      | High       | Fast     | Very Good       |
| Zero-Shot           | Copilot     | High     | High      | High       | Fast     | Very Good       |
| Few-Shot            | ChatGPT     | High     | High      | High       | Fast     | Excellent       |
| Few-Shot            | Gemini      | High     | High      | High       | Fast     | Very Good       |
| Few-Shot            | Claude      | High     | High      | High       | Fast     | Excellent       |
| Few-Shot            | Copilot     | High     | High      | High       | Fast     | Very Good       |
| Chain-of-Thought    | ChatGPT     | High     | Excellent | High       | Moderate | Excellent       |
| Chain-of-Thought    | Gemini      | High     | High      | High       | Moderate | Very Good       |
| Chain-of-Thought    | Claude      | High     | Excellent | High       | Moderate | Excellent       |
| Chain-of-Thought    | Copilot     | High     | High      | High       | Moderate | Very Good       |
| Role-Based          | ChatGPT     | High     | Excellent | Excellent  | Fast     | Excellent       |
| Role-Based          | Gemini      | High     | High      | High       | Fast     | Very Good       |
| Role-Based          | Claude      | High     | Excellent | Excellent  | Fast     | Excellent       |
| Role-Based          | Copilot     | High     | High      | High       | Fast     | Very Good       |




## Result
The evaluation of different prompting techniques (zero-shot, few-shot, chain-of-thought, and role-based) across AI platforms ChatGPT, Gemini, Claude, and Microsoft Copilot showed varied strengths. ChatGPT and Claude performed best overall in few-shot, chain-of-thought, and role-based prompting, demonstrating strong coherence, simplicity, and user experience based on the evaluation ratings. Gemini and Copilot provided clear and well-organized summaries suitable for understanding technical concepts. Zero-shot prompting produced comparable results across all four platforms. Selecting the best prompting technique depends on the task requirements, including accuracy, coherence, simplicity, speed, and the intended audience.

