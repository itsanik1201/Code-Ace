CODE-ACE: An Advanced LeetCode-Style Platform

CODE-ACE is a comprehensive coding platform that goes beyond traditional sites like LeetCode and HackerRank by integrating AI-driven tools, a gamified reward system, and a clean, modern user interface. It was built to solve the limitations of existing platforms by offering a more complete and interactive experience.

Key Features
AI-Powered Mock Interviews: Practice real-world interviews with an AI that generates questions, provides instant feedback, and scores your performance. This helps users, especially introverts, practice communicating their solutions under pressure.

"LeetCoin" Reward System: Earn LeetCoins by solving the daily Problem of the Day (POTD), scoring well in mock interviews, or ranking high in contests. These coins can be used to unlock premium problems without any payment.

Integrated AI Bot: Get instant, context-aware help while solving problems. This bot is specifically designed to answer questions about the current problem and avoids unrelated queries to keep you focused and reduce API costs.

Video Explanations with "Ask Me" Feature: Each problem has a video explanation with an AI-powered "Ask Me" feature. Using a vector database, it provides instant, relevant answers to your questions based only on the video's content, saving you time and money on API usage.
Real-time Contests: Participate in coding contests with a one-hour time limit to solve three random problems. Your performance is tracked on a leaderboard, and you are rewarded with LeetCoins.
Robust Problem Management: The platform provides a full-featured environment for solving Data Structures and Algorithms (DSA) problems, including a Monaco Editor for a VS Code-like experience, and the Judge0 API for code compilation and execution. You can easily filter, search, and paginate problems by difficulty and topic.

Tech Stack & Architecture

Frontend: Built with React.js for the user interface, styled with Tailwind CSS and DaisyUI. It also uses 

Redux for state management, WebRTC and WebSockets for real-time communication, and Zod with React Hook Form for validation.

Backend: Developed using Express.js with a microservices architecture. It uses 

JWT for authentication and authorization, and Redis for token blacklisting, rate limiting, and POTD tracking.

Databases:
MongoDB: The primary database for storing user data, problems, submissions, and contest information.
Redis: Used as an in-memory database for fast, temporary data like session management, rate limiting, and tracking daily challenges.
Supabase: Utilized as a vector database to store and semantically search video transcripts for the "Ask Me" feature.
Other Services: The project uses the Gemini API for AI-powered features, Cloudinary for media storage, and the Judge0 API for code compilation.
