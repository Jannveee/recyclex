# ReCycleX

ReCycleX is a MERN stack application architected to facilitate transactions between waste generators and recycling entities within a digital marketplace framework.

## Live Links
Frontend Environment: https://recyclex-puce.vercel.app/
Backend Environment: https://recyclex-mxjj.onrender.com/

## System Features
- Waste Categorization Module: Interface integrating AI-assisted parameters for waste identification and classification.
- Transaction Platform: Bidirectional marketplace supporting buy/sell operations for waste materials.
- Analytics Engine: Data visualization module outputting metrics for Waste Diverted and Active User Base.
- Incentive Tracking: System calculating and displaying numeric values corresponding to user transaction history.
- Frontend Interface: Component-based dashboard engineered with React, Vite, and Tailwind CSS.

## Technical Specifications
- Frontend Framework: React.js, Vite, Tailwind CSS, Lucide Icons
- Server Environment: Node.js, Express.js
- Data Storage: MongoDB (NoSQL)
- Infrastructure: Vercel (Frontend), Render (Backend)

## Application Architecture & Data Flow
1. Client Execution: The React.js frontend initializes state and renders the DOM. User input events trigger local state mutations.
2. Network Transmission: The client constructs and dispatches asynchronous HTTP requests. Payloads and JWT authorization headers are transmitted to REST API endpoints.
3. Server Processing: The Node.js/Express.js backend intercepts requests, executes JWT validation algorithms, and routes payloads to specified controller functions for logic execution.
4. Database Operations: The server initiates persistent connections to the MongoDB cluster to execute necessary CRUD operations.
5. State Reconciliation: The database returns query execution results to the server. The server formats the response as a JSON object and transmits it to the client.

## Repository Structure
The codebase utilizes a monorepo architecture:
- /client : Contains frontend application source code.
- /server : Contains backend API source code.

## Initialization Protocols

STEP 1: Repository Cloning
git clone https://github.com/Jannveee/recyclex.git
cd recyclex

STEP 2: Frontend Initialization
cd client
npm install
npm run dev

STEP 3: Backend Initialization
cd ../server
npm install
npm start

## Environment Configuration
Execution requires local .env file configuration in both root and client directories containing the following key-value pairs:

Server Configuration (create .env inside the /server folder)
MONGODB_URI=<Target_MongoDB_Connection_String>
JWT_SECRET=<Cryptographic_Key_For_Token_Generation>

Client Configuration (create .env inside the /client folder)
VITE_API_URL=<Target_Backend_Endpoint>
