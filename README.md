# 📁 Telegram Drive

Web-based file manager for Telegram bots. Manage and organize files stored in your Telegram chats with a beautiful, modern interface.

## 🌟 Live Demo
**[https://foxxw0lf.github.io/telegram-drive/](https://foxxw0lf.github.io/telegram-drive/)**
**[https://telegram-drive-iota.vercel.app/](https://telegram-drive-iota.vercel.app/)**

## ✨ Features

### 🤖 Telegram Integration
- Connect to any Telegram bot using Bot Token and Chat ID
- Automatically fetch and display files from Telegram chats
- Support for all file types (documents, images, videos, audio, archives)

### 📂 File Management
- **View**: Browse all files with thumbnails and metadata
- **Download**: Direct download from Telegram servers
- **Share**: Generate share links for files
- **Categorize**: Auto-sort files into Documents, Images, Videos, Others

### 🎨 Modern Interface
- Clean, responsive design that works on desktop and mobile
- File grid with icons and detailed information
- Category-based filtering and navigation
- Upload guide with step-by-step instructions

### 🔄 Demo Mode
- Automatic fallback when Telegram API is unavailable
- Sample files for testing and demonstration
- No setup required to try the interface

## 🚀 Getting Started

### 1. Create a Telegram Bot
1. Open Telegram and search for `@BotFather`
2. Send `/newbot` command
3. Follow the instructions to create your bot
4. Copy the **Bot Token** (format: `123456789:ABCdefGHIjklMNOpqrsTUVwxyz`)

### 2. Get Chat ID
**Option A: Use your bot**
1. Send a message to your bot
2. Visit: `https://api.telegram.org/bot<YOUR_BOT_TOKEN>/getUpdates`
3. Find `"chat":{"id":` in the response

**Option B: Use @userinfobot**
1. Send any message to `@userinfobot`
2. It will reply with your Chat ID

**Option C: For groups/channels**
1. Add your bot to the group/channel
2. Send a message mentioning the bot
3. Use the getUpdates method above

### 3. Connect Your Bot
1. Open the [Telegram Drive application](https://foxxw0lf.github.io/telegram-drive/)
2. Enter your **Bot Token** and **Chat ID**
3. Click **"Hubungkan"** (Connect)
4. Start uploading files to your Telegram chat!
5. Bot Token and Chat ID is saved on localstorage

## 📱 How to Upload Files

1. Open your Telegram app
2. Go to the chat with your bot
3. Send files by:
   - Drag & drop files into the chat
   - Click attachment button and select files
   - Forward files from other chats
4. Return to Telegram Drive and click **"Refresh"**
5. Your files will appear in the interface!

## 🔧 Technical Features

- **CORS Handling**: Graceful fallback to demo mode when API calls fail
- **Local Storage**: Remembers your bot configuration
- **File Type Detection**: Automatic categorization based on file extensions
- **Error Handling**: User-friendly error messages and recovery
- **Responsive Design**: Optimized for all screen sizes
- **Keyboard Shortcuts**: 
  - `ESC` - Close modals
  - `F5` - Refresh files
  - `Ctrl+R` - Refresh files

## 🛡️ Privacy & Security

- All data processing happens in your browser
- Bot tokens are stored locally in your browser only
- No server-side storage or processing
- Direct communication with Telegram API
- Open source - you can review all code

## 🎯 Supported File Types

### 📄 Documents
- PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX

### 🖼️ Images  
- JPG, JPEG, PNG, GIF, BMP, SVG

### 🎥 Videos
- MP4, AVI, MOV, WMV, FLV

### 🎵 Audio
- MP3, WAV, FLAC, AAC

### 📦 Archives
- ZIP, RAR, 7Z, TAR, GZ

## 🌐 Browser Support

- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features  
- Submit pull requests
- Improve documentation

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Links

- **Live Application**: [https://foxxw0lf.github.io/telegram-drive/](https://foxxw0lf.github.io/telegram-drive/)
- **Repository**: [https://github.com/foxxw0lf/telegram-drive](https://github.com/foxxw0lf/telegram-drive)
- **Telegram Bot API**: [https://core.telegram.org/bots/api](https://core.telegram.org/bots/api)

---

**Made with ❤️ for the Telegram community**
