
# Chat Application in Power Apps 📱💬

Welcome to the Chat Application! This Power Apps-based chat solution is designed for efficient, user-friendly communication, with a SharePoint list serving as the data source. The app enables users to chat, reply, view chat history, and search for other users in a fully responsive design suitable for both mobile and desktop use.

---
![Intro](./localImages/chatApp.gif)


## Features

- **Chat and Reply**: Initiate chats with other users, send messages, and view replies in real-time.
- **User Search**: Easily search for and select users to start a new chat.
- **Chat History**: Keep a record of all conversations and refer back to previous messages.
- **Time & Date Tracking**: Messages are stored with timestamps, allowing you to see when each message was sent or received.
- **Responsive Design**: Optimized for use on both mobile and desktop devices.
- **Easy Configuration**: Simple to set up and use—just import the solution and configure your SharePoint list.

---

## Setup Instructions

### Step 1: Create a New SharePoint List

To get started, create a SharePoint list with the following columns:

| Column Name | Data Type          | Description                             |
|-------------|---------------------|-----------------------------------------|
| Title       | Single line of text | Stores the title of the message         |
| MessageTo   | Person or Group     | Identifies the user the message is sent to |

> **Note**: Make sure to set permissions on the SharePoint list according to your organization’s security policies.

### Step 2: Download and Import the Solution

1. **Download the ZIP File**: Click [here](link-to-zip-file) to download the Chat Application solution ZIP file.
2. **Import into Power Apps**:
   - Go to [Power Apps](https://make.powerapps.com) and navigate to **Solutions**.
   - Select **Import Solution** and upload the downloaded ZIP file.
   - Follow the prompts to complete the import process.

### Step 3: Configure the App (If Necessary)

- **Verify Data Connections**: Ensure that the app is properly connected to the newly created SharePoint list as its data source.
- **Set User Permissions**: Ensure that users have the necessary permissions to view and interact with the SharePoint list for a seamless chat experience.

---

## How to Use

1. **Start a Chat**: Use the search bar to find users and initiate a new chat with them.
2. **Reply to Messages**: Open an existing chat to view the conversation history and reply in real-time.
3. **View Chat History**: The app saves all chat messages, including timestamps for each message.
4. **Responsive Design**: Whether on mobile or desktop, the app automatically adjusts for the best viewing experience.

---

Thank you for choosing this Chat Application! 🎉 If you have any issues or need assistance, please reach out.

---

Enjoy chatting and collaborating with ease!
