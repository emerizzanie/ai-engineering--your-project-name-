# Project Audit — 3-Minute Presentation

## 1. Project Title
- My project is called **Project Audit: A RAG-Based Assistant for Reviewing Responsible AI Practices in Student Projects**.
- It focuses on Generative AI, Retrieval-Augmented Generation (RAG), and Responsible AI.
- The main idea is to help students review potential risks in their AI projects using reliable guidelines and references.

## 2. Problem Background and Motivation
- When students develop AI projects, they need to consider issues such as privacy, fairness, reliability, and the impact of AI on users.
- Guidelines about these issues are available from organisations such as NIST and UNESCO.
- However, the information can be spread across different documents, and students may find it difficult to identify which guidelines are relevant to their projects.
- I want to explore whether an AI assistant can make these guidelines easier to find and understand.

## 3. Problem Statement
- Students may need to manually search through several documents to understand the Responsible AI risks related to their projects.
- A general AI chatbot may also provide answers that are not properly supported by reliable sources.
- Therefore, this project will investigate how a RAG-based assistant can provide project-specific explanations supported by retrieved guidelines and references.

## 4. Proposed Solution
- I plan to develop a simple web application using Streamlit.
- Students will enter their project details through a form, including the project's purpose, target users, and data used.
- The system will retrieve relevant information from public Responsible AI documents.
- An LLM will use the retrieved information to generate a preliminary review containing potential risks, suggested actions, and source references.
- PDF upload may be added later if time allows.

## 5. Objectives
- **Objective 1:** Collect and organise publicly available Responsible AI guidelines and frameworks.
- **Objective 2:** Develop a RAG-based assistant that explains potential Responsible AI risks using retrieved sources.
- **Objective 3:** Evaluate the system based on retrieval relevance, answer accuracy, citation accuracy, and its handling of questions that cannot be answered from the available documents.

## 6. Expected Outcome
- The expected outcome is a working prototype that helps students understand potential Responsible AI issues in their projects.
- It will provide explanations and references so students can check the original guidelines.
- The system is intended for preliminary review and learning, not formal safety certification or compliance approval.


# Project Audit — System Requirements

## 1. Functional Requirements

Functional requirements describe what the system must do.

| ID | Requirement | Description |
|---|---|---|
| FR1 | Project Information Input | The system shall allow students to enter their AI project's details, including its purpose, target users, and data used. |
| FR2 | Retrieve Reference Documents | The system shall retrieve relevant information from public Responsible AI guidelines based on the student's project details. |
| FR3 | Generate Risk Review | The system shall identify potential Responsible AI risks and explain why they may be relevant to the student's project. |
| FR4 | Provide Source Citations | The system shall provide references to the guidelines used to support its explanations. |
| FR5 | Display Review Report | The system shall present potential risks, explanations, and suggested actions in an organised report. |

## 2. Non-Functional Requirements

Non-functional requirements describe how well the system should work.

| ID | Requirement | Description |
|---|---|---|
| NFR1 | Answer Reliability | The system should generate answers supported by retrieved documents and avoid presenting unsupported information as fact. |
| NFR2 | Usability | The interface should be simple and easy for university students to understand and use. |
| NFR3 | Performance | The system should generate a review within a reasonable response time. |
| NFR4 | Privacy | The system should minimise the collection of personal or confidential information and handle submitted project details appropriately. |

## 3. Requirement Priorities

The initial development should focus on the five functional requirements and four non-functional requirements listed above.

The main workflow is:

1. Students enter their project details.
2. The system retrieves relevant Responsible AI guidance.
3. The system generates a preliminary risk review.
4. The system provides source citations.
5. The system displays the review report.

PDF uploads, user accounts, and downloadable reports may be considered as future enhancements if time permits.

## 4. Evaluation Considerations

The system should be evaluated to determine whether it meets its requirements.

- **Answer reliability:** Check whether the generated answers are supported by the reference documents.
- **Usability:** Test whether students can use the system and understand its results.
- **Performance:** Measure the time required to generate a review.
- **Privacy:** Check whether the system avoids collecting unnecessary personal or confidential information.

Measurable performance targets will be defined during the system design and evaluation stages.

**Note:** Project Audit provides a preliminary Responsible AI review for learning purposes. It does not provide formal compliance approval or certify that an AI project is safe.
