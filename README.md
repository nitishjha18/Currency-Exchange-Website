# 💱 Currency Exchange Website

A modern, responsive currency converter web application that provides real-time exchange rates for over 150+ currencies worldwide. Convert currencies instantly with an intuitive interface and beautiful UI.

## ✨ Features

- **Real-Time Exchange Rates** – Fetches live currency data from the Free Currency API
- **150+ Currencies** – Support for major and minor world currencies
- **Flag Display** – Visual currency flags using the FlagsAPI
- **Responsive Design** – Works seamlessly on desktop, tablet, and mobile devices
- **Instant Conversion** – Get exchange rates with a single click
- **User-Friendly Interface** – Clean and intuitive design for easy navigation
- **Error Handling** – Graceful error messages for failed API requests
- **Default Values** – USD to INR conversion on page load

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|----------|
| **HTML5** | Structure and markup |
| **CSS3** | Styling and responsive design |
| **JavaScript (Vanilla)** | Core functionality and API integration |
| **Free Currency API** | Real-time exchange rate data |
| **FlagsAPI** | Country flag images |
| **Font Awesome** | Icon library |

## 📦 Project Structure

```
Currency-Exchange-Website/
├── index.html          # Main HTML structure
├── app.js              # Core application logic
├── codes.js            # Currency codes and country mapping
├── style.css           # Styling and layout
└── README.md           # Documentation
```

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection (for API calls)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/nitishjha18/Currency-Exchange-Website.git
   cd Currency-Exchange-Website
   ```

2. **Open in browser**
   ```bash
   # On Windows
   start index.html
   
   # On macOS
   open index.html
   
   # On Linux
   xdg-open index.html
   ```

3. **Or use a local server** (recommended)
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (with http-server)
   npx http-server
   ```

## 💻 Usage

1. **Enter Amount** – Type the amount you want to convert in the input field
2. **Select From Currency** – Choose the source currency from the first dropdown
3. **Select To Currency** – Choose the target currency from the second dropdown
4. **View Exchange Rate** – The conversion rate displays automatically
5. **Click "Get Exchange Rate"** – Button updates the conversion with live rates

### Example
```
Input: 100 USD
Select: From = USD, To = INR
Output: 100 USD = 8300 INR (or current rate)
```

## 📋 Key Components

### HTML Structure
- **Header**: Currency Converter title
- **Amount Input**: Text field for entering conversion amount
- **Currency Dropdowns**: Dual select menus with flag icons
- **Exchange Rate Display**: Shows the conversion result
- **Submit Button**: Triggers the conversion

### JavaScript Functions

#### `updateExchangeRate()`
Fetches real-time exchange rate from the API and calculates the conversion amount.

```javascript
const updateExchangeRate = async () => {
  // Validates input amount
  // Constructs API URL with currencies
  // Fetches data and updates UI
};
```

#### `updateFlag(element)`
Updates the flag image based on selected currency code.

```javascript
const updateFlag = (element) => {
  // Gets currency code from selection
  // Fetches corresponding flag image
  // Updates display
};
```

## 🔌 API Integration

### Free Currency API
- **Endpoint**: `https://api.freecurrencyapi.com/v1/latest`
- **Features**: Real-time rates, 150+ currencies
- **Auth**: API key required

### FlagsAPI
- **Endpoint**: `https://flagsapi.com/{countryCode}/flat/64.png`
- **Usage**: Displays country flags for visual reference

## 🎨 Design Features

- **Color Scheme**: Steel blue (#4682b4) background with white container
- **Responsive Layout**: Flexbox-based design
- **Interactive Elements**: Hover effects on button, smooth transitions
- **Accessibility**: Semantic HTML, clear labels

## ⚠️ Important Notes

### API Key Security
The API key is currently exposed in the frontend code. For production use:

```javascript
// Store API key in environment variables
const BASE_URL = `https://api.freecurrencyapi.com/v1/latest?apikey=${process.env.API_KEY}`;
```

Or use a backend server to proxy API requests.

### Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 🐛 Known Issues & Solutions

| Issue | Solution |
|-------|----------|
| API rate limiting | Free tier has request limits; consider upgrade |
| Network errors | Check internet connection and browser console |
| Missing flags | Ensure FlagsAPI is accessible |
| CORS errors | May occur with certain VPNs or corporate networks |

## 🔮 Future Enhancements

- [ ] Add historical exchange rate charts
- [ ] Implement currency favorites/bookmarks
- [ ] Add offline mode with cached rates
- [ ] Dark mode toggle
- [ ] Multi-currency conversion
- [ ] Export conversion history as PDF/CSV
- [ ] Add cryptocurrency support
- [ ] Mobile app version
- [ ] Backend server for API key security

## 🤝 Contributing

Contributions are welcome! Follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit changes (`git commit -m 'Add YourFeature'`)
4. Push to branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

**Nitish Jha**
- GitHub: [@nitishjha18](https://github.com/nitishjha18)
- Repository: [Currency-Exchange-Website](https://github.com/nitishjha18/Currency-Exchange-Website)

## 🙏 Acknowledgments

- **Free Currency API** – For providing reliable exchange rate data
- **FlagsAPI** – For country flag imagery
- **Font Awesome** – For icon resources

## 📞 Support

For issues, questions, or suggestions:
- **GitHub Issues**: [Open an issue](https://github.com/nitishjha18/Currency-Exchange-Website/issues)

---

**Last Updated**: December 29, 2025

Made with ❤️ by [Nitish Jha](https://github.com/nitishjha18)