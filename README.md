# 📁 Telegram Drive

Web-based file manager for Telegram bots. Manage and organize files stored in your Telegram chats with a beautiful, modern interface.

## 🌟 Live Demo
**[https://foxxw0lf.github.io/telegram-drive/](https://foxxw0lf.github.io/telegram-drive/)**

## ✨ Features

### 🤖 Telegram Integration
- Connect to any Telegram bot using Bot Token and Chat ID
- Automatically fetch and display files from Telegram chats
- Support for all file types (documents, images, videos, audio, archives)

### 📂 File Management
- **View**: Browse all files with thumbnails and metadata
- **Download**: Direct download from Telegram servers
- **Share**: Generate share links for files
- **Delete**: Remove files from the interface
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

- **Enhanced CORS Handling**: Intelligent detection and graceful handling of browser CORS restrictions
- **Local Storage**: Remembers your bot configuration
- **File Type Detection**: Automatic categorization based on file extensions
- **Error Handling**: User-friendly error messages and recovery
- **Responsive Design**: Optimized for all screen sizes
- **Keyboard Shortcuts**: 
  - `ESC` - Close modals
  - `F5` - Refresh files
  - `Ctrl+R` - Refresh files

## ⚠️ CORS Limitations & Solutions

### The Problem
Web browsers block direct API calls to Telegram servers due to CORS (Cross-Origin Resource Sharing) security policies. This is a browser security feature, not a bug in the application.

### ✅ Recommended Solutions

#### 1. **Browser Extension (Easiest)**
- Install "CORS Unblock" or "Disable CORS" browser extension
- Enable it for this site only
- ⚠️ **Security Note**: Only use for testing/development

#### 2. **Local Development**
```bash
# Clone the repository
git clone https://github.com/foxxw0lf/telegram-drive.git
cd telegram-drive

# Run local server (choose one):
python -m http.server 8000        # Python
npx serve .                       # Node.js  
php -S localhost:8000            # PHP

# Open http://localhost:8000
```

#### 3. **Firefox Developer Edition**
- Firefox has more relaxed CORS policies for development
- Download Firefox Developer Edition
- Open the application in Firefox

#### 4. **Chrome with Disabled Security**
```bash
# Close all Chrome windows first
chrome --disable-web-security --user-data-dir=/tmp/chrome
```

### 🎭 Enhanced Demo Mode

If CORS blocks API access, the app automatically switches to **Demo Mode** with:
- ✅ Full interface functionality
- ✅ Sample files for testing all features
- ✅ File categorization and filtering
- ✅ All UI interactions work normally
- ❌ No real file downloads (demo only)

Click "Enhanced Demo" for more sample files!

## 🛡️ Privacy & Security

- All data processing happens in your browser
- Bot tokens are stored locally in your browser only
- No server-side storage or processing
- Direct communication with Telegram API (when CORS allows)
- Open source - you can review all code
- **Security Note**: CORS workarounds should only be used for development/testing

## 🆘 Troubleshooting

### "Failed to connect" or "Network Error"
- **Cause**: Browser CORS policy blocking Telegram API
- **Solution**: Use the CORS solutions listed above or try Demo Mode

### "Bot token invalid"
- **Cause**: Incorrect token format or expired token
- **Solution**: Get a new token from @BotFather

### "Chat ID not found"
- **Cause**: Bot doesn't have access to the chat
- **Solution**: Send a message to the bot first, or add bot to group

### Files not showing up
- **Cause**: Bot only sees new messages after being added
- **Solution**: Send new files after connecting the bot

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
