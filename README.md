# SMS Transaction Parser

A professional Android application that automatically reads bKash and Nagad transaction SMS messages, parses transaction data, and uploads to a PHP/MySQL backend.

## 🌟 Features

- **Auto SMS Reading**: Automatically reads and processes bKash and Nagad transaction messages
- **Smart Parsing**: Extracts Amount, Phone Number, Transaction ID, Balance, and DateTime
- **Foreground Service**: Runs reliably in the background with auto-start capability
- **Masking Management**: Add, remove, enable/disable custom SMS sender IDs
- **Real-time Logging**: Color-coded console for tracking all operations
- **Secure API**: API key authentication for secure data transmission
- **Modern UI**: Material Design 3 with Dark Mode support

## 📋 Requirements

### Android App
- **Minimum Android Version**: Android 12 (API 31)
- **Maximum**: Latest Android Version
- **Language**: Kotlin
- **Permissions**: SMS Read, Foreground Service, Boot Completed

### Backend
- **PHP**: 7.4 or higher
- **MySQL**: 5.7 or higher
- **Web Server**: Apache/Nginx with mod_rewrite

## 🚀 Quick Start

### Android App Setup

1. Open the `android` folder in Android Studio
2. Sync Gradle dependencies
3. Build and run on your device
4. Grant SMS and notification permissions
5. Configure API settings in Settings tab

### PHP Backend Setup

1. Copy `backend` folder to your web server
2. Import `database/sms_transactions.sql` to MySQL
3. Configure database credentials in `config.php`
4. Update `API_KEY` in `config.php`
5. Test API using the demo test button in the app

## 📱 App Structure

### Tab 1 - Start/Stop
- START/STOP button for service control
- Real-time counters (Received, Uploaded, Failed)
- Auto-start on app open

### Tab 2 - Masking Management
- Add/Remove custom sender IDs
- Enable/Disable maskings
- Default: bKash, NAGAD

### Tab 3 - Console/Logs
- Real-time operation logs
- Color-coded messages (Green=Success, Red=Failed, Blue=Processing)

### Tab 4 - Settings
- API Configuration (URL, Key)
- Database connection details (optional)
- Test connection button
- Local storage for settings

## 🔒 Security Features

- API Key authentication
- SQL injection protection
- Input validation
- Prepared statements
- Secure credential storage

## 📊 Database Schema

```sql
sms_transactions (
    id, masking_name, phone_number, transaction_id,
    amount, balance, received_time, created_at
)
```

## 🔍 Search Functionality

Search by phone number returns:
- Phone Number
- Transaction ID
- Balance
- Date & Time

## 👨‍💻 Developer

**MD ALAMIN**  
SHOBHAN AUTO, JESSORE

📧 aaminjsr@gmail.com  
📱 +8801711844085 (WhatsApp)

## 📄 License

This project is open source and available for everyone.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

## ⭐ Support

If you like this project, please give it a star on GitHub!
