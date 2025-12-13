# 🍷 Telegram Dating Bot

A full-featured, premium Dating Bot for Telegram built with Node.js, Telegraf, and MongoDB. This bot provides a seamless Tinder-like experience directly within Telegram, complete with profile creation, matching algorithms, monetization via Telegram Stars, and safety features.

---

## 📱 Demo

<div align="center">
  <img src="assets/Demo.gif" width="300" />
  <p><em>App demo video: profile creation and matching flow</em></p>
</div>

<br>

<table>
<tr>
<th>Profile Creation</th>
<th>Swiping & Matching</th>
<th>Premium Features</th>
</tr>
<tr>
<td><img src="assets/img1.jpg" width="180" /></td>
<td><img src="assets/img2.jpg" width="180" /></td>
<td><img src="assets/img3.jpg" width="180" /></td>
</tr>
<tr>
<td><em>Sending a message</em></td>
<td><em>Swiping and getting a match</em></td>
<td><em>Buying more swipes with Stars</em></td>
</tr>
</table>

<p align="center"><em>Swipe, match, and explore premium features</em></p>
<br>

---

## ✨ Features

### 👤 User Profiles
- **Comprehensive Setup**: Users can set their Name, Age, Gender, Bio, and upload 2-3 Photos.
- **Preferences**: Users specify who they are looking for (Men/Women) and their intention (Serious, Casual, Friendship, Exploring).
- **Profile Management**: Easy-to-use commands to View (`/profile`), Edit (`/edit`), or Delete (`/delete`) profiles.

### 💘 Matching System
- **Smart Queue**: Shows candidates based on gender preferences and excludes already seen profiles.
- **Bidirectional Matching**: A match is only created when both users like each other.
- **Direct Messaging**: Users can send a message directly to a candidate, which also counts as a "Like".
- **Notifications**: Instant notifications for Likes and Matches.

### 💰 Monetization (Telegram Stars)
- **Daily Limits**: Users get **20 free swipes** every day.
- **In-App Purchases**: Integrated with Telegram Stars for seamless payments.
    - **40 Swipes**: 4 Stars
    - **80 Swipes**: 10 Stars
- **Revenue Generation**: Ready-to-deploy monetization strategy.

### 🛡️ Safety & Moderation
- **Reporting System**: Users can report inappropriate profiles directly from the card view.
- **Privacy First**: Usernames are only revealed after a mutual match.
- **Block Handling**: Graceful handling of users who block the bot.

---

## 🛠️ Tech Stack

- **Runtime**: [Node.js](https://nodejs.org/)
- **Framework**: [Telegraf](https://telegraf.js.org/) (Telegram Bot API)
- **Database**: [MongoDB](https://www.mongodb.com/) (Atlas recommended)
- **Payments**: Telegram Stars (XTR)

---

## 🚀 Installation

### Prerequisites
- Node.js (v16 or higher)
- MongoDB Connection URI
- Telegram Bot Token (from [@BotFather](https://t.me/BotFather))

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/Eul45/telegram-connect-bot.git
   cd telegram-dating-bot
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Environment Variables**
   Create a `.env` file in the root directory and add your credentials:
   ```env
   # Telegram Bot Token from BotFather
   BOT_TOKEN=your_bot_token_here

   # MongoDB Connection String
   MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/datingbot
   ```

4. **Start the Bot**
   ```bash
   npm start
   ```

## 📖 Usage Commands

| Command | Description |
|:---|:---|
| `/start` | Initialize the bot and see the welcome message. |
| `/create` | Start the profile creation wizard. |
| `/match` | Start swiping and finding matches. |
| `/profile` | View your own profile as others see it. |
| `/edit` | Edit specific parts of your profile (Photos, Bio, etc.). |
| `/matches` | View your mutual matches and people who liked you. |
| `/delete` | Permanently delete your profile and data. |
| `/help` | View safety tips and information. |

## 📂 Project Structure

```
telegram-dating-bot/
├── index.js           # Main bot logic and entry point
├── package.json       # Dependencies and scripts
├── .env               # Environment variables
└── README.md          # Project documentation
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License.

