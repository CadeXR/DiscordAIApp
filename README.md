# Discord AI Bot - Setup and Usage Guide

Welcome to the Discord AI Bot! This guide will help you set up and use the application for the first time. 

## Prerequisites

Before you begin, ensure the following are installed on your Windows PC:

1. **Python**: Install from the [Microsoft Store](https://www.microsoft.com/store/productId/9NCVDN91XZQP?ocid=pdpshare). Make sure it is added to your system's PATH.
   
2. **.NET Framework**: The app will prompt an installation if it is not already installed.

3. **OpenAI API Key**: You will need an OpenAI API key. Follow [this guide](https://platform.openai.com/docs/quickstart) to get your key.

4. **Discord Bot Setup**: You need to create your own Discord bot with Privileged Gateway Intents enabled. Follow these steps:
   1. Go to the [Discord Developer Portal](https://discord.com/developers/applications).
   2. Click on **New Application**, give it a name, and create it.
   3. Navigate to the **Bot** section on the left sidebar.
   4. Click **Add Bot** to turn your application into a bot.
   5. Enable **Privileged Gateway Intents** under **Presence Intent**, **Server Members Intent**, and **Message Content Intent**.
   6. Copy the **Token** from the Bot section, as you’ll need it in the app.

---

## First Time Setup

1. **Open the Application**: After downloading and launching the application, you will be greeted with the main window.

2. **Setup Python Environment**: 
   - Click the `Setup Python Environment` button. 
   - This will automatically install the necessary Python packages for the bot to function.
   - This step must be done the first time you run the application.

---

## Configuration

### 1. **OpenAI API Key**
   - Paste your **OpenAI API Key** in the appropriate field in the app.

### 2. **Discord Bot Token**
   - Paste your **Discord Bot Token** into the field labeled **Discord Token**.

### 3. **Wake Word**
   - This is the word that will trigger the bot in your Discord server. Type the word you want to use.

### 4. **Choose OpenAI Model**
   - **GPT-3.5-turbo**: Fast and efficient, suitable for most applications. It is cheaper in token cost.
   - **GPT-4**: More powerful, but slower and consumes more tokens, making it ideal for more complex queries.
   - **GPT-4o**: Optimized version of GPT-4, balancing speed and power.

### 5. **Short Term Memory (Optional)**
   - If enabled, the bot will remember the context of previous interactions within a session.
   - **Pros**: Enhances context-based conversations.
   - **Cons**: Increases token consumption and may slow down responses slightly.

---

## Features

### 1. **Prompt File**
   - The bot uses a `prompt.txt` file located in the app's settings folder. You can open and modify this file to customize the bot's behavior and initial instructions.
   - Example of customization: You could instruct the bot to act like a teacher, a friend, or a specific persona by modifying the content of this file.

### 2. **Memory System**
   - The bot has a short-term memory feature. By default, it stores previous user interactions temporarily to provide more contextually relevant answers.
   - Memory is automatically cleared every 5 minutes, ensuring that only recent conversations are taken into account.
   - If memory is disabled, the bot will handle each user query as a new interaction, which speeds up the process and reduces token usage.

---

## Running the Bot

1. **Run the Bot**: 
   - After setting up your API keys, tokens, and other settings, click the `Run` button to start the bot.
   - The app will provide real-time feedback in the logs window about the bot’s activity.

2. **Stop the Bot**: 
   - Click the `Stop` button to safely shut down the bot.

---

## Additional Information

### Speed vs. Token Cost
   - **GPT-3.5-turbo** is faster and cheaper in terms of token usage but may not be as powerful for advanced tasks.
   - **GPT-4** consumes more tokens and is slower but handles more complex queries more effectively.

### Support
   - For any issues or questions regarding setup and usage, feel free to reach out via GitHub Issues or check out the OpenAI and Discord API documentation for additional support.
