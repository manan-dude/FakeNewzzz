

# 📰 **News Authenticity Checker & Financial Fraud Detector**
![Screenshot (472)](https://github.com/user-attachments/assets/a9e20768-945d-439c-9af2-d73e4dafcfdd)


Welcome to the **News Authenticity Checker** and **Financial Fraud Detector** application! This app leverages Google Generative AI to help users determine the authenticity of news content and detect potential financial fraud. 

## 🚀 **Features**
- **News Authenticity Checking**: Analyze news headlines or content and receive a fake percentage score.
- **Financial Fraud Detection**: Assess whether a given prompt relates to financial fraud and get recommended measures.

## 🛠️ **Technologies Used**
- **Node.js**: JavaScript runtime for building the server.
- **Express**: Web framework for Node.js to handle HTTP requests.
- **CORS**: Middleware to enable Cross-Origin Resource Sharing.
- **Google Generative AI**: AI model for generating content.

## 📦 **Installation**

### Prerequisites
- Node.js (v14 or higher)
- npm (Node Package Manager)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/manan-dude/FakeNewzzz.git
   cd <repository-directory>
   ```

2. Install the dependencies:
   ```bash
   npm install
   ```

3. **Set Up Your Environment**
   - Create a `.env` file in the root directory of your project.
   - Add your Google Generative AI API key to the `.env` file:
     ```
     API_KEY=your_gemini_api_key
     ```

4. Start the server:
   ```bash
   npm start
   ```

5. Open your browser and visit:
   ```
   http://localhost:3001
   ```

## 📬 **API Endpoints**

### 1. **Generate Content for News Authenticity**
- **Endpoint**: `POST /generate`
- **Request Body**:
   ```json
   {
     "prompt": "Enter your news headline or content here..."
   }
   ```
- **Response**:
   ```json
   {
     "response": "AI generated response text",
     "percentage": "XX%"
   }
   ```

### 2. **Detect Financial Fraud**
- **Endpoint**: `POST /fraud-detect`
- **Request Body**:
   ```json
   {
     "prompt": "Enter the financial scenario to evaluate..."
   }
   ```
- **Response**:
   ```json
   {
     "response": "AI generated response text",
     "percentage": "XX%"
   }
   ```

## ⚠️ **Error Handling**
- If you receive a `400` error, ensure your request body includes a `prompt`.
- A `500` error indicates an internal server issue.

## 💻 **Example Usage**
You can use tools like **Postman** or **cURL** to test the API endpoints. Here’s a sample cURL request for generating news authenticity:
```bash
curl -X POST http://localhost:3001/generate \
-H "Content-Type: application/json" \
-d '{"prompt": "Is this news fake?"}'
```

## 🎉 **Contributing**
We welcome contributions! If you would like to contribute, please fork the repository and submit a pull request.

## 📄 **License**
This project is licensed under the MIT License.

---

Feel free to customize any sections according to your needs, including the repository URL and any additional instructions specific to your application!
