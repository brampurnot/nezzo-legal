# Privacy Policy

**Last Updated:** January 17, 2026

At **Nezzo**, we take your privacy seriously. Because our platform executes autonomous agents and durable workflows, we process unique types of data (including Agent Instructions and Workflow State). This policy explains how we handle that data.

## 1. Information We Collect

### 1.1. Account Information
We collect your name, email address, and payment information when you sign up.

### 1.2. Workflow & Agent Data (Sensitive)
To provide the Service, we process:
* **Agent Definitions:** The system prompts, instructions, and tools you configure.
* **Execution Logs:** The step-by-step history of what your Agent thought and did.
* **Workflow State:** The input and output variables passed between steps in your workflows.
* **Integration Credentials:** API keys (e.g., for Slack, SAP, OpenAI) that you provide to allow your Agents to act. These are encrypted at rest.

### 1.3. Usage Data
We collect telemetry on how you use the "Agent Builder" and execution engine to improve performance and fix bugs.

## 2. How We Use Your Data

* **To Provide the Service:** We need to read your Agent Definitions to compile them into executable workflows.
* **To Maintain Durability:** We persist your "Workflow State" to our database after every step. This allows your agents to resume exactly where they left off in case of a crash.
* **To Debug Failures:** If a workflow crashes, our engineers may access the execution logs to identify the root cause (unless you opt-out of support access).

## 3. Data Sharing and Sub-Processors

### 3.1. LLM Providers
Our platform relies on Large Language Models (LLMs) to function.
* **Data Transfer:** When your Agent runs, we send its system prompt and current context window to third-party model providers (e.g., OpenAI, Anthropic, Google).
* **Zero-Retention Policy:** We configure these API calls with "Zero Retention" settings where available, meaning the providers should not train their models on your data. However, this is subject to *their* privacy policies.

### 3.2. Infrastructure Providers
We use cloud providers (e.g., AWS, Azure, Vercel) to host our database and execution engine.

## 4. Data Retention

* **Execution History:** We retain detailed execution logs for **90 days** to allow you to audit and debug your agents. After this period, logs are permanently deleted.
* **Account Deletion:** If you delete your account, we will purge your Agent Definitions and Credentials within 30 days.

## 5. Security

We use enterprise-grade encryption for:
* **Data at Rest:** All workflow state and databases are encrypted.
* **Secrets:** Your third-party API keys are encrypted using a dedicated Key Management Service (KMS) and are only decrypted inside the ephemeral execution environment.

## 6. Your Rights (GDPR / CCPA)
Depending on your location, you may have the right to:
* Access the personal data we hold about you.
* Request deletion of your execution history.
* Export your Agent Definitions in a portable format (JSON).

To exercise these rights, contact us at **info@nezzo.io**.

## 7. Changes to This Policy
We may update this policy as our platform evolves (e.g., adding new AI models). We will notify you of significant changes via email or dashboard notification.
