# SECURE TRADE FINANCE EXPLORER FOR TRANSACTION TRANSPARENCY AND COMPLIANCE INSIGHTS

# Setup Instructions

1. Backend Setup
Go to the backend folder:

cd TradeFinanceMain/backend
Create and activate a virtual environment:

python -m venv venv
venv\Scripts\activate
Install Python dependencies:

pip install -r requirements.txt
Create a .env file in the backend folder and configure values such as:

DATABASE_URL=postgresql+asyncpg://postgres:password@localhost:5432/tradedb
SECRET_KEY=change-this-secret
REFRESH_SECRET_KEY=change-this-refresh-secret
REDIS_URL=redis://localhost:6379/0
AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_REGION=us-east-1
S3_BUCKET_NAME=trade-finance-docs
GEMINI_API_KEY=
Run database migrations:

alembic upgrade head
Start the backend server:

python run_local.py
The backend will run at:

http://127.0.0.1:8000
API documentation is available at:

http://127.0.0.1:8000/docs

2. Frontend Setup
Go to the frontend folder:

cd TradeFinanceMain/frontend
Install Node dependencies:

npm install
Start the frontend development server:

npm start
The frontend will run at:

http://localhost:3000

3. Redis Setup
Start Redis before using cache-dependent features.

If using the included Windows Redis folder, run the Redis server executable from:

Redis-x64-5.0.14.1/redis-server.exe


# Usage Details
Open the frontend in the browser:
http://localhost:3000
Register or log in with a valid user account.

Use the dashboard to view trade finance activity, compliance insights, and transaction summaries.

Create and manage trade transactions from the Transactions section.

Upload and review documents connected to trade transactions.

Review transaction history and ledger details for transparency.

Check risk scores and alerts to identify suspicious or high-risk transactions.

Generate compliance reports and analytics from the reporting sections.

