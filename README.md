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
<img width="1470" height="579" alt="image" src="https://github.com/user-attachments/assets/d9ebf131-aa76-4f2c-885d-68c489e7cec1" />


  

### 2. Build the Moderation Service

- Use **Azure Logic Apps** to set up a trigger that listens for new chat messages from **Microsoft Teams**.

### 3. Implement the Email Notification Logic

- Configure the Logic App to **send an email** to a specified administrator when inappropriate content is detected.
- Follow the format provided in the official alert template (if available).

### 4. Test the Workflow

- Workflow setup
  <img width="1470" height="579" alt="image" src="https://github.com/user-attachments/assets/ced20f31-c315-4605-9cae-3eae76dcdd6e" />


- Simulate messages in Microsoft Teams and ensure:
  - Violations are detected correctly.
    <img width="1389" height="514" alt="image" src="https://github.com/user-attachments/assets/26411290-01c0-42bb-b52d-57be332e50bd" />
    
    <img width="1200" height="514" alt="image" src="https://github.com/user-attachments/assets/5cd1076c-519c-412c-8d9c-0e1f75c39f16" />

  - Email notifications are triggered.
    

   <img width="1200" height="514" alt="image" src="https://github.com/user-attachments/assets/181346d7-748d-488e-a2aa-1204474c54b3" />








---
### 5. Challenges Encountered

- Microsoft Teams trigger only supports certain scopes (e.g., team/channel vs private chats).
- Cognitive Services misclassification in some cases (false positives).
- Permissions required to access Teams message data.
- Delay in Logic App triggering for private messages.


---

### 6. Recommendations

- Use **Azure Content Moderator** (deprecated but still functional) for better flagging in future.
- Extend functionality to store flagged messages in a database for audit.
- Add sentiment and toxicity scoring in notification email.
- Secure Logic App endpoints with authentication if HTTP inputs are used.


### Demo: https://youtu.be/fcZj_PoUoF8




