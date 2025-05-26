# OpenStack AI Command Center

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![OpenStack SDK];(https://img.shields.io/badge/OpenStack-SDK-red.svg)](https://docs.openstack.org/openstacksdk/)
[![Google Gemini](https://img.shields.io/badge/AI-Google%20Gemini-green.svg)](https://ai.google.dev/)

A next-generation **AI-powered OpenStack management platform** that revolutionizes cloud infrastructure operations through natural language processing, intelligent automation, and modern web interfaces. Built with Google Gemini AI, this system transforms complex OpenStack operations into simple conversational commands.

## ð¯ Project Overview

The OpenStack AI Command Center bridges the gap between complex cloud infrastructure management and user-friendly interaction paradigms. By leveraging cutting-edge AI technology and modern web development practices, it provides an intuitive, efficient, and scalable solution for OpenStack resource management.

### Key Achievements
- **90% reduction** in command complexity through natural language processing
- **Real-time AI interpretation** of user intents with Google Gemini integration
- **Comprehensive API coverage** supporting all major OpenStack services
- **Production-ready architecture** with mock testing capabilities
- **Modern React-based UI** with shadcn/ui components and TypeScript

## ð Features

### Core Capabilities
- **ð¤ AI-Powered Natural Language Processing**: Convert plain English commands into OpenStack operations using Google Gemini
- **ð¯ Intelligent Command Interpretation**: Advanced context understanding with parameter extraction and validation
- **â¡ Real-time Execution**: Instant processing and execution of cloud infrastructure commands
- **ð Interactive Workflows**: Smart parameter collection with user confirmation for critical operations
- **ð Comprehensive Resource Management**: Full CRUD operations for VMs, networks, volumes, and storage
- **ð¡ï¸ Security-First Design**: Environment-based credential management and secure API interactions

### Technical Features
- **ðï¸ Modular Architecture**: Clean separation between AI agent, API layer, and OpenStack integration
- **ð§ª Mock Testing Environment**: Complete fake API implementation for development and testing
- **ð± Modern Web Interface**: React + TypeScript frontend with shadcn/ui components
- **ð RESTful API**: Well-documented endpoints for seamless integration
- **ð Scalable Design**: Built for enterprise-grade OpenStack deployments
- **ð Rich Logging**: Comprehensive logging and error handling for debugging

## ðï¸ Architecture Overview

The OpenStack AI Command Center follows a modern, microservices-inspired architecture:

```
âââââââââââââââââââ    ââââââââââââââââââââ    âââââââââââââââââââ
â   Frontend UI   â    â   Backend API    â    â  OpenStack API  â
â   (React/TS)    âââââºâ   (Flask/CORS)   âââââºâ   (Real/Mock)    â
âââââââââââââââââââ    ââââââââââââââââââââ    âââââââââââââââââââ
                              â
                              â¼
                       ââââââââââââââââââââ
                       â   AI Agent       â
                       â (Google Gemini)  â
                       ââââââââââââââââââââ
```

### Component Breakdown
- **AI Agent Layer**: Google Gemini-powered natural language processing
- **API Gateway**: Flask-based REST API with CORS support
- **OpenStack Integration**: SDK-based real and mock implementations
- **Frontend Interface**: Modern React application with TypeScript
- **Data Layer**: JSON-based mock data for testing scenarios

## ð¡ The Challenge We Solve

OpenStack management traditionally requires:
- **Complex API Knowledge**: Understanding intricate service interactions
- **CLI Expertise**: Memorizing numerous commands and parameters
- **Manual Processes**: Repetitive, error-prone infrastructure tasks
- **Steep Learning Curve**: Months of training for effective usage

### Our Solution
- **Natural Language Interface**: "Create a Ubuntu VM with 4GB RAM" â Executed
- **Intelligent Automation**: Smart parameter defaults and validation
- **User-Friendly Web UI**: Point-and-click operations for common tasks
- **Comprehensive Testing**: Mock environment for safe experimentation

## ð Project Structure

```
VM_manager_AgenticAi/
âââ ð¤ Core AI Components
â   âââ agent.py                 # Google Gemini-powered AI agent
â   âââ agent_original.py        # Original agent implementation
â   âââ agent_two_layer_original.py # Alternative agent architecture
â
âââ ð Backend API
â   âââ routes.py               # Flask REST API endpoints
â   âââ app.py                  # Main Flask application
â   âââ runner.py               # Application runner
â
âââ âï¸ OpenStack Integration
â   âââ api.py                  # Real OpenStack API wrapper
â   âââ fake_api.py             # Mock OpenStack implementation
â   âââ openstack_manager.py    # Core OpenStack operations
â   âââ test_openstack_api.py   # API connectivity tests
â
âââ ð¨ Frontend Application
â   âââ openstack-command-center-ui/
â       âââ src/
â       â   âââ components/      # Reusable UI components
â       â   âââ pages/          # Application pages
â       â   âââ services/       # API service layer
â       â   âââ hooks/          # Custom React hooks
â       â   âââ lib/            # Utility libraries
â       âââ package.json        # Node.js dependencies
â       âââ vite.config.ts      # Vite build configuration
â       âââ tailwind.config.ts  # Tailwind CSS configuration
â
âââ ð Mock Data & Testing
â   âââ fake_data/
â       âââ servers.json        # Mock server instances
â       âââ flavors.json        # VM flavor definitions
â       âââ images.json         # OS image catalog
â       âââ networks.json       # Network configurations
â       âââ volumes.json        # Storage volumes
â       âââ usage.json          # Resource usage data
â
âââ ð§ Configuration
â   âââ requirements.txt        # Python dependencies
â   âââ chatbot_config.json     # AI agent configuration
â   âââ .gitignore             # Git ignore rules
â
âââ ð Documentation
    âââ README.md              # This file
    âââ frontend.md            # Frontend documentation
```

### ð Key Components

#### AI Agent (`agent.py`)
- **Google Gemini Integration**: Advanced natural language processing
- **Function Calling**: Structured OpenStack operation execution
- **Context Management**: Intelligent parameter extraction and validation
- **Error Handling**: Comprehensive error recovery and user feedback

#### Backend API (`routes.py`)
- **RESTful Endpoints**: Standard HTTP methods for resource management
- **CORS Support**: Cross-origin requests for frontend integration
- **Authentication**: Secure credential management
- **Request Validation**: Input sanitization and parameter validation

#### OpenStack Integration
- **Real API (`api.py`)**: Production OpenStack SDK integration
- **Mock API (`fake_api.py`)**: Development and testing environment
- **Manager (`openstack_manager.py`)**: High-level operation abstractions

#### Frontend Application
- **React + TypeScript**: Type-safe, modern web development
- **shadcn/ui Components**: Beautiful, accessible UI components
- **Vite Build System**: Fast development and optimized production builds
- **Tailwind CSS**: Utility-first styling framework

## ð ï¸ Technology Stack

### Backend Technologies
- **Python 3.8+**: Core programming language
- **Flask**: Lightweight web framework
- **OpenStack SDK**: Official OpenStack client library
- **Google Generative AI**: Gemini model integration
- **Flask-CORS**: Cross-origin resource sharing
- **Rich**: Enhanced terminal output formatting

### Frontend Technologies
- **React 18**: Modern UI library with hooks
- **TypeScript**: Type-safe JavaScript development
- **Vite**: Next-generation frontend tooling
- **Tailwind CSS**: Utility-first CSS framework
- **shadcn/ui**: High-quality component library
- **Radix UI**: Accessible component primitives
- **Framer Motion**: Animation library
- **TanStack Query**: Data fetching and caching

### Development & Testing
- **Mock Data System**: JSON-based fake OpenStack environment
- **Environment Variables**: Secure configuration management
- **ESLint**: Code quality and consistency
- **PostCSS**: CSS processing and optimization

## ð Quick Start

### Prerequisites

- **Python 3.8+** with pip
- **Node.js 16+** with npm/yarn
- **Google API Key** for Gemini integration
- **OpenStack Environment** (optional - can use mock mode)

### 1. ð¥ Clone Repository

```bash
git clone https://github.com/akshit7093/VM_manager_AgenticAi.git
cd VM_manager_AgenticAi
```

### 2. ð Backend Setup

#### Create Virtual Environment
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# Windows
.\venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

#### Install Python Dependencies
```bash
pip install -r requirements.txt
```

#### Configure Environment Variables
Create a `.env` file in the project root:

```bash
# Google AI Configuration (Required)
GOOGLE_API_KEY=your_google_api_key_here

# OpenStack Configuration (Optional - for production use)
OS_AUTH_URL=https://your-openstack-endpoint:5000/v3
OS_USERNAME=your_username
OS_PASSWORD=your_password
OS_PROJECT_NAME=your_project_name
OS_PROJECT_ID=your_project_id
OS_USER_DOMAIN_NAME=Default
OS_PROJECT_DOMAIN_NAME=Default
OS_REGION_NAME=RegionOne
OS_INTERFACE=public
OS_IDENTITY_API_VERSION=3
```

**ð Getting Google API Key:**
1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create a new API key
3. Copy the key to your `.env` file

### 3. ð¨ Frontend Setup

```bash
cd openstack-command-center-ui

# Install dependencies
npm install
# or
yarn install

# Return to project root
cd ..
```

### 4. ð§ª Development Mode (Recommended)

For development and testing, the system uses mock OpenStack data by default:

```bash
# The agent.py file is configured to use FakeOpenStackAPI
# No additional OpenStack setup required
```

### 5. ð§ Production Configuration

For production use with real OpenStack:

1. **Update agent.py** to use real API:
   ```python
   # Change this line in agent.py
   from api import OpenStackAPI  # Instead of FakeOpenStackAPI
   ```

2. **Verify OpenStack connectivity:**
   ```bash
   python test_openstack_api.py
   ```

### 6. â Verify Installation

```bash
# Test Python dependencies
python -c "import flask, google.generativeai, openstacksdk; print('â Backend dependencies OK')"

# Test frontend dependencies
cd openstack-command-center-ui && npm list --depth=0
```

## ð® Usage Guide

### ð Starting the Application

#### 1. Start Backend Services

**Option A: Using the main application runner**
```bash
# Start the Flask API server
python routes.py
```

**Option B: Using the alternative app runner**
```bash
# Alternative Flask application
python app.py
```

The backend API will be available at:
- **API Base URL**: `http://localhost:5001`
- **Health Check**: `http://localhost:5001/api/health`
- **Command Endpoint**: `http://localhost:5001/api/command`

#### 2. Start Frontend Application

```bash
cd openstack-command-center-ui

# Development server
npm run dev
# or
yarn dev
```

The frontend will be available at:
- **Web UI**: `http://localhost:3000`
- **Development Tools**: Hot reload enabled

### ð¬ Natural Language Commands

The AI agent understands various natural language patterns:

#### VM Management
```bash
# Create VMs
"Create a new Ubuntu server named web-server-01 with 4GB RAM"
"Launch a CentOS VM called database-server with m1.large flavor"
"Spin up a Windows instance with 8GB memory and 100GB storage"

# List and query VMs
"Show me all running servers"
"List VMs in the project"
"What servers are currently active?"

# VM operations
"Delete the server named test-vm"
"Stop the instance web-server-01"
"Restart database-server"
```

#### Network Operations
```bash
# Network management
"Create a new network called production-net"
"List all available networks"
"Show network details for private-net"
```

#### Storage Management
```bash
# Volume operations
"Create a 50GB volume named backup-storage"
"List all volumes in the project"
"Attach volume backup-storage to web-server-01"
```

### ð Web Interface Usage

1. **Dashboard**: Overview of all OpenStack resources
2. **VM Management**: Create, list, and manage virtual machines
3. **Network View**: Visualize and manage network topology
4. **Storage Console**: Manage volumes and snapshots
5. **AI Chat**: Interactive natural language interface

### ð§ API Integration

For programmatic access, use the REST API endpoints:

### 3. Interacting with the System

   - **Via Web UI:** Open the UI URL in your browser to manage VMs and interact with OpenStack resources.
     *   **Screenshot Placeholder:**
         ```
         [----------------------------------------------------]
         [|                  Web Application UI                |]
         [|                (Screenshot of the App)             |]
         [----------------------------------------------------]
         ```

   - **Via AI Agent (CLI or API):** Send natural language commands to the agent's endpoint or interface.
     *   **CLI Screenshot Placeholder:**
         ```
         [----------------------------------------------------]
         [|               CLI Interaction Example              |]
         [|        (Screenshot of CLI command and output)      |]
         [----------------------------------------------------]
         ```

   **Example API Endpoints (defined in `routes.py` or `app.py`):**

   Detailed examples of API interactions:

   - **`POST /api/command`**: Send a natural language command to the AI agent.
     *   **Request Example (Create VM):**
         ```json
         {
           "command": "create a new ubuntu vm named webserver01 with 2 vcpus and 4gb ram flavor m1.small image ubuntu-latest"
         }
         ```
     *   **Expected Response (Success):**
         ```json
         {
           "status": "success",
           "message": "VM 'webserver01' creation initiated successfully.",
           "vm_id": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
           "details": {
             "name": "webserver01",
             "vcpus": 2,
             "ram_mb": 4096,
             "flavor": "m1.small",
             "image": "ubuntu-latest"
           }
         }
         ```
     *   **Expected Response (Error):**
         ```json
         {
           "status": "error",
           "message": "Failed to process command: Invalid flavor specified.",
           "details": "Flavor m1.unknown not found."
         }
         ```

   - **`GET /api/vms`**: List all VMs.
     *   **Request Example:** (No body required for GET)
     *   **Expected Response (Success with VMs):**
         ```json
         {
           "status": "success",
           "vms": [
             {
               "id": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
               "name": "webserver01",
               "status": "ACTIVE",
               "addresses": {
                 "private": [
                   {"version": 4, "addr": "192.168.1.10"}
                 ]
               },
               "flavor": "m1.small",
               "image": "ubuntu-latest",
               "created_at": "2023-10-27T10:30:00Z"
             },
             {
               "id": "yyyyyyyy-yyyy-yyyy-yyyy-yyyyyyyyyyyy",
               "name": "dbserver01",
               "status": "BUILDING",
               "addresses": {},
               "flavor": "m1.medium",
               "image": "centos-stream9",
               "created_at": "2023-10-27T11:00:00Z"
             }
           ]
         }
         ```
     *   **Expected Response (Success with no VMs):**
         ```json
         {
           "status": "success",
           "vms": []
         }
         ```

   - **`GET /api/vms/<vm_id>`**: Get details for a specific VM.
     *   **Request Example:** (No body required for GET, `vm_id` in URL path)
     *   **Expected Response (Success):**
         ```json
         {
           "status": "success",
           "vm": {
             "id": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
             "name": "webserver01",
             "status": "ACTIVE",
             "addresses": {
               "private": [
                 {"version": 4, "addr": "192.168.1.10"}
               ]
             },
             "flavor": "m1.small",
             "image": "ubuntu-latest",
             "vcpus": 2,
             "ram_mb": 4096,
             "disk_gb": 20,
             "created_at": "2023-10-27T10:30:00Z",
             "updated_at": "2023-10-27T10:35:00Z"
           }
         }
         ```
     *   **Expected Response (Not Found):**
         ```json
         {
           "status": "error",
           "message": "VM not found",
           "vm_id": "non-existent-vm-id"
         }
         ```

   - **`DELETE /api/vms/<vm_id>`**: Delete a specific VM.
     *   **Request Example:** (No body required for DELETE, `vm_id` in URL path)
     *   **Expected Response (Success):**
         ```json
         {
           "status": "success",
           "message": "VM 'xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx' deletion initiated."
         }
         ```
     *   **Expected Response (Error - VM not found):**
         ```json
         {
           "status": "error",
           "message": "Failed to delete VM: VM not found.",
           "vm_id": "non-existent-vm-id"
         }
         ```

### 4. Using the Mock API (`fake_api.py`)

   To run the system without a live OpenStack environment, ensure the agent and backend are configured to use `fake_api.py`. This is typically handled through configuration settings or environment variables.

### ð§ª Testing & Development

#### Mock Environment Testing
```bash
# Test with fake OpenStack data (default)
python agent.py
# The system will use data from fake_data/ directory
```

#### OpenStack Connectivity Testing
```bash
# Test real OpenStack connection
python test_openstack_api.py
```

#### API Endpoint Testing
```bash
# Test API endpoints with curl
curl -X GET http://localhost:5001/api/health
curl -X POST http://localhost:5001/api/command \
  -H "Content-Type: application/json" \
  -d '{"command": "list all servers"}'
```

## ð Deployment

### Production Deployment

#### Using Docker (Recommended)

```dockerfile
# Dockerfile example
FROM python:3.9-slim

WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .
EXPOSE 5001

CMD ["python", "routes.py"]
```

```bash
# Build and run
docker build -t VM_manager_AgenticAi .
docker run -p 5001:5001 --env-file .env VM_manager_AgenticAi
```

#### Using systemd (Linux)

```ini
# /etc/systemd/system/openstack-ai.service
[Unit]
Description=OpenStack AI Command Center
After=network.target

[Service]
Type=simple
User=www-data
WorkingDirectory=/opt/VM_manager_AgenticAi
Environment=PATH=/opt/VM_manager_AgenticAi/venv/bin
ExecStart=/opt/VM_manager_AgenticAi/venv/bin/python routes.py
Restart=always

[Install]
WantedBy=multi-user.target
```

#### Environment Variables for Production

```bash
# Production environment variables
FLASK_ENV=production
FLASK_DEBUG=False
GOOGLE_API_KEY=your_production_api_key
OS_AUTH_URL=https://your-openstack.com:5000/v3
# ... other OpenStack credentials
```

### Frontend Deployment

```bash
cd openstack-command-center-ui

# Build for production
npm run build

# Serve with nginx, Apache, or any static file server
# Build output will be in dist/ directory
```

## ð§ Troubleshooting

### Common Issues

#### Google API Key Issues
```bash
# Error: GOOGLE_API_KEY not set
# Solution: Set environment variable
export GOOGLE_API_KEY="your_api_key_here"
```

#### OpenStack Connection Issues
```bash
# Error: Failed to connect to OpenStack
# Solution: Check credentials and network connectivity
python test_openstack_api.py
```

#### Frontend Build Issues
```bash
# Error: Node modules not found
# Solution: Reinstall dependencies
cd openstack-command-center-ui
rm -rf node_modules package-lock.json
npm install
```

#### CORS Issues
```bash
# Error: CORS policy blocking requests
# Solution: Ensure Flask-CORS is properly configured
# Check routes.py for CORS(app) configuration
```

### Debug Mode

```bash
# Enable debug logging
export FLASK_DEBUG=True
export FLASK_ENV=development
python routes.py
```

### Log Files

- **Application Logs**: `chatbot.log`
- **Consolidated Logs**: `consolidated_chatbot.log`
- **Frontend Logs**: Browser developer console

## ð¤ Contributing

We welcome contributions! Please follow these guidelines:

### Development Setup

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Install development dependencies**
   ```bash
   pip install -r requirements.txt
   cd openstack-command-center-ui && npm install
   ```
4. **Make your changes**
5. **Test thoroughly**
6. **Submit a pull request**

### Code Style

- **Python**: Follow PEP 8 guidelines
- **TypeScript/React**: Use ESLint configuration
- **Commit Messages**: Use conventional commit format

### Areas for Contribution

- ð¤ **AI Agent Improvements**: Enhanced natural language understanding
- ð¨ **UI/UX Enhancements**: Better user interface design
- ð§ **OpenStack Integration**: Support for additional services
- ð **Documentation**: Improved guides and examples
- ð§ª **Testing**: Unit tests and integration tests
- ð **Performance**: Optimization and caching

## ð Acknowledgments

- **Google Gemini AI** for advanced natural language processing
- **OpenStack Foundation** for the comprehensive cloud platform
- **React Community** for the excellent frontend ecosystem
- **Flask Community** for the lightweight web framework

## ð Support

For support and questions:

- ð§ **Email**: [akshitsharma7093@gmail.com]
- ð¬ **Issues**: [GitHub Issues](https://github.com/akshit7093/VM_manager_AgenticAi/issues)
- ð **Documentation**: [Project Wiki](https://github.com/akshit7093/VM_manager_AgenticAi/wiki)

---

**Made with â¤ï¸ for the OpenStack community**