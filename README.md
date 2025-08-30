Gyaan Deck: AI-Powered Presentation Generator

Effortlessly convert raw text into styled PowerPoint slides using your own templates. 

Gyaan Deck is a streamlined web application designed to instantly transform long-form text, such as markdown or notes, into a ready-to-use PowerPoint presentation. By uploading your own template, providing simple instructions, and using your personal LLM API key, the app produces a custom-styled deck.

✨ Core Features

Flexible Input: Accepts various text inputs, including lengthy documents, markdown, or simple prose.


AI Guidance: Direct the AI's output with brief instructions to define the presentation's tone or format (e.g., "create an investor pitch deck").


BYO API Key: Works with your personal API keys from providers like OpenAI, Anthropic, and Gemini. Keys are never logged or stored.


Custom Templates: Apply your branding by uploading existing .pptx or .potx files to set the style, fonts, and layouts.


Image Preservation: Preserves and reuses any images found within your uploaded template.


Direct Download: Generates a ready-to-download .pptx file immediately after processing.


Intelligent Content Splitting: Intelligently segments your source text into a logical number of slides.


Privacy-Focused: Built with privacy in mind; no user text, API keys, or files are ever saved.

🚀 Getting Started
1. Get the Source Code
Bash

git clone https://github.com/23f1000805/tds-bonus-project-Auto-PPT-Generator-GyaanSetu-Deck.git 
cd tds-bonus-project-Auto-PPT-Generator-GyaanSetu-Deck 
2. Install Dependencies
Bash

# Set up the backend environment
pip install -r requirements.txt 

# The frontend does not require a build step 
3. Run the App Locally
Bash

uvicorn app:app --reload 
Access the application at 

http://localhost:8000.

4. Deploy to the Cloud
The application is pre-configured for easy deployment on platforms like Railway, Render, Vercel, or Heroku.

🖥️ How to Use
Enter your source text or markdown content.

Provide an optional instruction to guide the AI, such as 

"make it a research summary".

Supply your API key from a supported LLM provider.

Select and upload your custom PowerPoint template.

Click 

Generate to create and download your presentation.

🛠️ System Architecture
Frontend:

A responsive interface using HTML and Tailwind UI.

Manages user inputs, file uploads, and downloads.

Features progress notifications and a history of past generations.

Backend (FastAPI):

Processes incoming text, guidance, API keys, and templates.

Intelligently divides content into slide sections.

Uses 

python-pptx to populate the provided template while preserving original styles, fonts, and images.

🌟 Potential Enhancements
Automatic generation of speaker notes for each slide.

A library of pre-set guidance options for common presentation types.

The ability to preview slides in the browser before downloading the final file.

Improved error handling and automatic retries for API requests.

📄 License
Distributed under the MIT License, which permits free usage, modification, and sharing.
