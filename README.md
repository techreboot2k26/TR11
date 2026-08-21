# TechReboot'26: Queue Management System (QMS)

**QueueCraft** is a comprehensive, multi-module queue management system designed to optimize student-staff interactions at educational institutions. It features a real-time dashboard for staff, mobile-friendly student queueing, and a robust admin interface for configuration and analytics.

## ✨ Features

### 👩‍🏫 Staff Module (Dashboard)
*   **Real-time Queue Management**: Instantly pull and serve the next token.
*   **Token Actions**: Complete, hold, or skip tokens with immediate feedback.
*   **Status Control**: Open or close the counter to control queue access.
*   **Live Metrics**: Track current serving token, wait times, and session statistics.
*   **Socket Sync**: Instant updates across all connected devices.

### 👨‍🎓 Student Module
*   **Get Token**: Request a ticket for a specific service (Printer, Librarian, etc.).
*   **Queue Tracking**: View real-time position in the queue.
*   **Service Details**: Check assigned service counter and operating hours.
*   **Responsive UI**: Seamless experience on mobile and desktop.

### 🛡️ Admin Module
*   **Service Configuration**: Define services and assign them to specific counters.
*   **Counter Management**: Add, edit, or delete service counters.
*   **Staff Management**: Onboard and manage staff users.
*   **User Control**: Manage both staff and student user accounts.

## 🚀 Getting Started

### Prerequisites
*   **Node.js**: v16.x or higher
*   **NPM**: v8.x or higher

### Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/karthik200805/TR11.git
    cd TR11
    ```

2.  Install dependencies:
    ```bash
    # Node.js dependencies
    npm install --ignore-scripts

    # Python dependencies (Optional / Python FastAPI backend)
    uv venv --python 3.13
    .\.venv\Scripts\activate
    uv pip install -r requirements.txt
    ```

### Running the Application

1. **Start Backend Server**:
   ```bash
   npm run server
   # Or for Python FastAPI backend:
   uvicorn app.main:app --reload --port 5001
   ```

2. **Start Frontend Client**:
   ```bash
   npm run dev
   ```

The application will be accessible at:
* **Frontend Application**: `http://localhost:5173`
  * **Student Portal**: `http://localhost:5173/`
  * **Staff Dashboard**: `http://localhost:5173/staff`
  * **Admin Portal**: `http://localhost:5173/admin`
* **Backend API**: `http://localhost:5001/api`

### Running Tests

* **Vitest (TypeScript / Express)**:
  ```bash
  npm test
  ```

* **Pytest (Python / FastAPI)**:
  ```bash
  pytest
  ```

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.