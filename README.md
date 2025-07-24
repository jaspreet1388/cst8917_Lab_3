# CST8917 Lab 3: Implementing a Teams Chat Content Moderation Service

## Objective

In this lab, we will develop an **Microsoft Teams chat content moderation service** using **Azure Logic Apps**. The service will monitor Teams chat messages for inappropriate content and automatically trigger **email notifications** when a policy violation is detected. 



---

## About the Technologies

### Azure Logic Apps

Azure Logic Apps is a cloud-based service that allows you to automate workflows and integrate services without writing much code. It is ideal for building real-time systems triggered by services like Microsoft Teams, email, or HTTP endpoints.


---

## Tasks

### 1. Design the Moderation Workflow

- Create a **flowchart** that outlines how your moderation system works.
- Include components like Microsoft Teams trigger, Logic App flow, optional Azure Functions, optional Cognitive Services, and email notifications.
- <img width="1558" height="309" alt="image" src="https://github.com/user-attachments/assets/d2ee6c68-4f5f-4e91-9286-710a712c0b04" />

  

### 2. Build the Moderation Service

- Use **Azure Logic Apps** to set up a trigger that listens for new chat messages from **Microsoft Teams**.

### 3. Implement the Email Notification Logic

- Configure the Logic App to **send an email** to a specified administrator when inappropriate content is detected.
- Follow the format provided in the official alert template (if available).

### 4. Test the Workflow

- Simulate messages in Microsoft Teams and ensure:
  - Violations are detected correctly.
  - Email notifications are triggered.
  - Optional services (Functions, Cognitive Services) are working correctly.

### 5. Document Your Project

Include the following in your documentation:
- A screenshot or export of your workflow flowchart.
- Description of your Logic App setup.
- Optional: details about Azure Functions or Cognitive Services used.
- Explanation of how you tested the workflow.
- Challenges you encountered and how you resolved them.
- Recommendations for future improvement.

### 6. Record a Demo



---

## Deliverables

- Your completed Logic App workflow.
- A screenshot or exported image of your **moderation flowchart**.
- Your written **report** (as a separate file or included in `README.md`).
- A demo video uploaded to YouTube, linked in the `README.md`.

---




