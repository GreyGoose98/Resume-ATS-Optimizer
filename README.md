# Resume ATS Optimizer Pro 📄

A powerful Streamlit application that helps job seekers optimize their resumes for Applicant Tracking Systems (ATS) using Google's Gemini AI. This tool analyzes, enhances, and creates professional resumes to improve your chances of getting past ATS filters.

## Features 🚀

### Core Functionality
- **Resume Analysis**: Comprehensive ATS compatibility scoring (0-100) with detailed feedback
- **Resume Optimization**: AI-powered resume enhancement based on job descriptions
- **Custom Updates**: Personalized resume modifications with custom instructions
- **Resume Creation**: Build professional resumes from scratch using a form-based interface

### File Support
- **Input Formats**: PDF, DOCX, TXT, TEX files
- **Output Formats**: Markdown, HTML, DOCX downloads
- **Text Extraction**: Advanced parsing for multiple document types

### User Experience
- **Modern UI**: Clean, responsive interface with professional styling
- **Visual Scoring**: Circular progress indicators for ATS scores
- **Tabbed Interface**: Organized workflow across multiple tabs
- **Real-time Processing**: Instant feedback and results

## Installation 🛠️

### Prerequisites
- Python 3.7 or higher
- Google Gemini API key (optional but recommended)

### Required Dependencies
```bash
pip install streamlit
pip install google-generativeai
pip install python-docx
pip install PyPDF2
pip install pdfminer.six
pip install python-docx
pip install markdown
```

### Optional Dependencies
For enhanced functionality:
```bash
pip install phi-agent  # For advanced agent functionality
pip install mammoth    # For better DOCX formatting
```

## Setup 📋

1. **Clone or download** the application files
2. **Install dependencies** using the requirements above
3. **Configure Gemini API** (optional):
   - Uncomment the API key line in the `GeminiModel` class
   - Replace `"YOUR_GEMINI_API_KEY"` with your actual API key
4. **Add logo** (optional):
   - Place `inventify_logo.png` in the same directory as the script

## Usage 🎯

### Running the Application
```bash
streamlit run app.py
```

### Workflow

#### 1. Upload & Analyze Tab
- **Upload Resume**: Support for PDF, DOCX, TXT, TEX files
- **Add Job Description**: Upload file or paste text directly
- **Analyze**: Get comprehensive ATS compatibility score
- **Boost**: Automatically optimize resume based on analysis

#### 2. Custom Update Tab
- Upload any resume file
- Provide custom instructions for modifications
- Get personalized resume updates

#### 3. Create New Resume Tab
- Fill out comprehensive form with personal details
- Include education, experience, skills, and optional sections
- Generate professional resume from scratch

#### 4. Results & Downloads Tab
- View analysis reports and ATS scores
- Download optimized resumes in multiple formats
- Compare before/after scores

## Technical Architecture 🏗️

### AI Models
- **Google Gemini 1.5 Flash**: Primary AI model for all text processing
- **Custom Agents**: Specialized agents for different tasks:
  - Analysis Agent: Resume analysis and scoring
  - Boost Agent: Resume optimization
  - Custom Agent: Custom modifications
  - Create Agent: New resume generation

### File Processing
- **PDF Extraction**: Using pdfminer.six and PyPDF2
- **DOCX Processing**: python-docx with optional mammoth for better formatting
- **Text Processing**: Advanced cleaning and placeholder removal

### Scoring Algorithm
The ATS scoring system evaluates:
1. **Resume Parsing**: Text extraction and formatting preservation
2. **Job Description Analysis**: Keyword and requirement extraction
3. **Keyword Matching**: Frequency and context analysis
4. **Contextual Evaluation**: Relevance and appropriate placement
5. **Formatting Assessment**: ATS-friendly structure validation
6. **Scoring Aggregation**: Weighted component scoring

## Customization 🎨

### Styling
The application uses custom CSS for:
- Modern gradient backgrounds
- Circular progress indicators
- Responsive button designs
- Professional typography

### Agents Configuration
Each AI agent can be customized with:
- Different model versions
- Custom instructions
- Specific parameters
- Tool configurations

## Troubleshooting 🔧

### Common Issues

1. **PDF Text Extraction Errors**
   - Ensure PDF is not password-protected
   - Try converting to DOCX or TXT format

2. **API Key Issues**
   - Verify Gemini API key is correct
   - Check API quota and billing status

3. **File Upload Problems**
   - Verify file format is supported
   - Check file size limitations

4. **Missing Dependencies**
   - Install all required packages
   - Use virtual environment for isolation

### Performance Optimization
- Use smaller resume files for faster processing
- Limit job description length for better analysis
- Consider using Gemini Pro for complex documents

## File Structure 📁

```
resume-ats-optimizer/
├── app.py                  # Main application file
├── inventify_logo.png      # Optional logo file
├── README.md              # This file
└── requirements.txt       # Dependencies list
```

## API Integration 🔌

### Google Gemini Configuration
```python
# Configure in the GeminiModel class
genai.configure(api_key="YOUR_GEMINI_API_KEY")
```

### Custom Model Integration
The application supports custom AI models by:
1. Implementing the model interface
2. Updating agent configurations
3. Modifying prompt templates

## Contributing 🤝

### Areas for Contribution
- Additional file format support
- Enhanced scoring algorithms
- UI/UX improvements
- Performance optimizations
- Multi-language support

### Development Setup
1. Fork the repository
2. Create feature branch
3. Implement changes
4. Test thoroughly
5. Submit pull request

## License 📜

This project is open-source and available under standard terms. Please respect the usage guidelines and API terms of service.

## Support 💬

For issues, questions, or suggestions:
- Check the troubleshooting section
- Review common issues in the codebase
- Consider API documentation for Gemini integration

## Roadmap 🗺️

### Planned Features
- [ ] LinkedIn profile integration
- [ ] Industry-specific resume templates
- [ ] Batch processing capabilities
- [ ] Advanced analytics dashboard
- [ ] Resume comparison tools
- [ ] Interview preparation suggestions

### Recent Updates
- ✅ Multi-format file support
- ✅ Custom update functionality
- ✅ Form-based resume creation
- ✅ Enhanced UI/UX design
- ✅ DOCX export capability

---

**Resume ATS Optimizer Pro** - Empowering job seekers with AI-driven resume optimization tools.
