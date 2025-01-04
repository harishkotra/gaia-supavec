# Supavec + Gaia Integration

A powerful document question-answering system that combines Supavec's RAG capabilities with Gaia's language understanding. This system enables intelligent conversations with your documents through semantic search and natural language processing.

## Project Structure

The project is divided into two main parts:
1. **Backend**: Handles file uploads, text uploads, and communication with the Supavec and Gaia APIs.
2. **Frontend**: Provides a user interface for uploading files, listing uploaded files, and interacting with the chat interface.

## Key Components
- Frontend Layer: React application with real-time updates and file management
- Backend API: Express.js server handling request orchestration
- Document Processing: Supavec API for document chunking and embedding
- Language Model: Gaia API for contextual question answering
- Data Flow: Bidirectional communication with optimized response streaming

### API Endpoints

- `POST /api/upload`: Uploads a file to Supavec.
- `POST /api/upload-text`: Uploads text content to Supavec.
- `GET /api/files`: Retrieves a list of uploaded files.
- `POST /api/search`: Searches embeddings based on a query and file IDs.
- `POST /api/ask`: Asks a question about documents using Gaia.

## Getting Started

### Prerequisites

- Node.js and npm installed on your machine.
- Get your Supavec API key from the [dashboard](https://www.supavec.com/)
- Run your own local node using [Gaia](https://docs.gaianet.ai/node-guide/quick-start/)

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/gaia-supavec.git
   cd gaia-supavec
   ```
2. Install backend dependencies:
    ```sh
    cd backend
    npm install
    ```
3. Install frontend dependencies:
    ```sh
    cd ../frontend
    npm install
    ```

### Running the Project

1. Start the backend server:
    ```sh
    cd backend
    npm start
    ````
2. Start the frontend development server:
   ```sh
   cd ../frontend
   npm start
   ```
3. Open your browser and navigate to `http://localhost:3000` to access the application.

### Usage
1. *Upload Documents:* Use the file upload interface to upload PDF or text files.
2. *List Files:* View the list of uploaded files.
3. *Ask Questions:* Select files and ask questions about their content using the chat interface.

## Contributing

1. Fork the repository
2. Create your feature branch (git checkout -b feature/AmazingFeature)
3. Commit your changes (git commit -m 'Add some AmazingFeature')
4. Push to the branch (git push origin feature/AmazingFeature)
5. Open a Pull Request

## Acknowledgments

- [Supavec](https://www.supavec.com/) team for the RAG infrastructure
- [Gaia](https://www.gaianet.ai/) for the simple infra to launch local LLMs or use Public nodes.