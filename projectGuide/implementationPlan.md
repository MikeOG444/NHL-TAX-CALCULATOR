Great! Let’s start by setting up the project in Visual Studio Code step by step. Since you’re on a MacBook and have the VS Code and terminal extensions enabled, we will use the terminal for the setup.

⸻

1. Project Setup

We’ll create a new project using Node.js with Express for the backend and React with TypeScript for the frontend. This will allow us to build a scalable and maintainable web application.

Step 1: Open Terminal in VS Code
	1.	Open VS Code.
	2.	Open the terminal:
	•	Use shortcut Ctrl + ` (backtick) or
	•	Click Terminal > New Terminal.

⸻

Step 2: Create Project Directory

Run the following command in the terminal to create and navigate into a new project folder:

mkdir nhl-tax-calculator
cd nhl-tax-calculator



⸻

Step 3: Initialize Git (Optional but Recommended)

This will set up version control:

git init



⸻

Step 4: Set Up Backend (Node.js & Express)
	1.	Initialize a Node.js project:

mkdir backend
cd backend
npm init -y


	2.	Install Express.js and other dependencies:

npm install express cors dotenv


	3.	Install development dependencies (TypeScript, nodemon, etc.):

npm install -D typescript ts-node nodemon @types/node @types/express


	4.	Initialize TypeScript config:

npx tsc --init


	5.	Create an entry point file:

touch src/index.ts
mkdir src



⸻

Step 5: Set Up Frontend (React with TypeScript)

Navigate back to the root folder and create the React project:

cd ..
npx create-react-app frontend --template typescript



⸻

Step 6: Setup Project Guide Folder

Since we want to document the implementation plan, let’s create a projectGuide folder and an initial plan file.
	1.	Navigate to the root project directory:

cd nhl-tax-calculator


	2.	Create the projectGuide folder and plan file:

mkdir projectGuide
touch projectGuide/implementationPlan.md


	3.	Open the file in VS Code:

code projectGuide/implementationPlan.md



⸻

2. Write the Initial Implementation Plan

Now, in projectGuide/implementationPlan.md, add the following initial implementation plan:

⸻

NHL Tax Calculator - Implementation Plan

Phase 1: Project Setup (✅ Done)
	•	Create project folder nhl-tax-calculator
	•	Initialize Git repository
	•	Setup backend with Node.js, Express, TypeScript
	•	Setup frontend with React, TypeScript
	•	Create projectGuide folder and add this implementation plan

⸻

Phase 2: Backend Development
	•	Setup Express server
	•	Create API endpoints for tax calculations and contract data retrieval
	•	Integrate Free NHL API to fetch player contracts
	•	Implement Tax Calculation Logic
	•	Federal tax
	•	State & local tax
	•	Jock tax based on NHL schedule
	•	Store tax data (state & city rates)
	•	Use MongoDB/PostgreSQL or JSON for initial version

⸻

Phase 3: Frontend Development
	•	Create UI to enter contract details
	•	Show tax calculations & comparisons
	•	Table format: Gross salary, taxes, net pay
	•	Charts & graphs for visualization
	•	Display assumptions page & tooltips
	•	Inline tax assumption tooltips
	•	Full “Assumptions” page with all details

⸻

Phase 4: Testing & Debugging
	•	Write unit tests for tax calculations
	•	Validate data with real-world NHL contracts
	•	Optimize performance

⸻

Phase 5: Deployment
	•	Deploy backend (Node.js API) on Render/Vercel/AWS
	•	Deploy frontend (React) on Netlify/Vercel
	•	Make the tool publicly accessible
	•	Announce on Reddit/Twitter/Hockey Forums

⸻
