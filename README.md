# Smart Resume Builder with AI Suggestions

A professional resume builder web application that creates beautiful resumes with AI-powered improvement suggestions.

## Features

- **Interactive Resume Builder**: Real-time form with instant preview
- **Multiple Templates**: Modern, Classic, and Minimal designs
- **AI-Powered Suggestions**: Get smart recommendations for improving your resume
- **PDF Export**: Download your resume as a professional PDF
- **Print Support**: Optimized print styling for direct printing
- **Auto-Save**: Automatic local storage of your work
- **Responsive Design**: Works perfectly on desktop and mobile devices

## Live Demo

Visit the live application: [GitHub Pages URL will be here after deployment]

## How to Use

1. **Fill in Your Information**: Enter your personal details, work experience, education, and skills
2. **Choose a Template**: Select from Modern, Classic, or Minimal designs
3. **Get AI Suggestions**: Click the AI suggestion buttons to get personalized recommendations
4. **Preview in Real-Time**: See your resume update instantly as you type
5. **Export or Print**: Download as PDF or print directly from your browser

## AI Suggestions

The app provides intelligent suggestions for:
- **Overall Resume**: Structure and completeness recommendations
- **Professional Summary**: Writing tips for compelling summaries
- **Work Experience**: Advice on quantifying achievements and using action verbs
- **Skills**: Suggestions for relevant technical and soft skills

## Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **UI Framework**: Bootstrap 5.3.0
- **Icons**: Font Awesome 6.4.0
- **PDF Generation**: jsPDF
- **AI Integration**: OpenAI GPT-3.5 Turbo
- **Backend**: Flask (Python) for AI API

## GitHub Pages Deployment

This application is designed to work as a static website on GitHub Pages. The AI suggestions feature requires a backend server, but the core resume building functionality works entirely in the browser.

### For Full Functionality (with AI)
1. Deploy the Flask backend to a service like Heroku, Railway, or Render
2. Update the API endpoint in `script.js`
3. Set your OpenAI API key in the backend environment

### For Static GitHub Pages (without AI)
The resume builder works perfectly without the AI features, providing all core functionality including:
- Resume building and editing
- Template switching
- PDF export
- Print support
- Local storage

## Installation

1. Clone this repository
2. For local development with AI features:
   ```bash
   pip install -r requirements.txt
   export OPENAI_API_KEY=your_api_key_here
   python app.py
   ```
3. For static deployment: Simply upload the HTML, CSS, and JS files to any web server

## Browser Support

- Chrome/Chromium 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## License

MIT License - feel free to use this project for personal or commercial purposes.

## Contributing

Pull requests are welcome! Please ensure your code follows the existing style and includes appropriate tests.