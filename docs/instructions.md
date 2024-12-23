# Instructions for Real-Time Chat Application 
## Overview
This project involves developing a real-time chat application using the Plasmic's Next.js framework. The application integrates with Supabase for authentication, storage, and real-time subscriptions to provide a seamless and responsive user experience.
## Requirements:
1. User Authentication
- Implement user authentication using Supabase Auth.
- Ensure secure login and registration functionalities. 
2. Real-Time Chat Functionality
- Integrate real-time subscriptions using Supabase.
- Enable users to send and receive messages instantly.
- Display chat history and ensure new messages appear in real-time.
3.Storage
- Utilize Supabase storage for handling user-uploaded files (e.g images, documents).
- Ensure efficient upload, retrieval, and display of stored files within the chat application.
4.User Interface
- Design an intuitive and user-friendly interface using Next.js, Tailwind CSS and ShadCN UI.
- Ensure the application is responsive and works well on different devices (desktop, tablet, mobile).
UI/UX Design Brief for Real-Time Chat Application:
We are developing a real-time chat application using the Plasmic's Next.js framework. The design should be user-friendly, visually appealing, and responsive across different devices. The integration of Supabase will be used for authentication, storage, and real-time messaging.
Key Components:
    1. Login & Registration Screens:
A welcoming splash screen with the app logo and name (NextChat).
Simple and intuitive forms for user login and registration.
With username, email and password. 
    2. Home Screen:
A clean and modern dashboard displaying recent chats and notifications.
A navigation menu allowing access to profile settings, contact list, and chat history.
Search functionality to quickly find contacts or chats.
    3. Chat Interface:
An easy-to-navigate chat layout with a list of contacts on the left and the chat window on the right.
Clear timestamps for messages.
Options for sending text messages, emojis, images, and files.
Indicate when users are typing.
A scrollable chat history.
    4. User Profile:
A profile section where users can update their information, change their profile picture, and set status messages.
Settings for notification preferences and privacy options.
    5. File Storage & Management:
A section within the chat for viewing and managing shared files.
Preview functionality for images and documents.
Option to download files.
    6. Notifications:
Real-time notifications for new messages, friend requests, and other important events.
A non-intrusive, consistent notification system across different devices.
Design Elements:
#Color Scheme: Choose a modern and calming color palette that promotes a sense of trust and security. Consider using shades of blue, green, or pastel colors.
#Typography: Use clear and legible fonts. Maintain consistency in font styles and sizes across the application.
#Icons & Illustrations: Use simple and intuitive icons to enhance usability. Consider adding illustrations for onboarding screens and empty states. Use framer motion for animations
#Accessibility: Ensure the design is accessible to all users. Follow best practices for color contrast, font size, and keyboard navigation.
#Responsiveness:
The application should be fully responsive and work seamlessly on desktops, tablets, and mobile.
5.Performance and Security
- Optimize the application for performance to handle high traffic and real-time updates efficiently.
- Implement security best practices to protect user data and prevent unauthorized access.
6.Testing and Deployment
- Conduct thorough testing to ensure all features work as expected.
- Prepare the application for deployment and provide documentation for maintenance and future updates.
7. Best Practices
- Follow best practices in coding to ensure code readability and maintainability.
- Provide detailed documentation for each component.

Backend & Database Setup:
##Supabase Integration
Supabase will be used as the backend service for this real-time chat application. It will handle authentication, storage, and real-time subscriptions, providing a scalable and efficient backend infrastructure.
Database Configuration
    1. Database Schema: I have already set up the database schema in Supabase.
#Authentication
User Authentication: Implement user authentication using Supabase Auth to manage secure login, registration functionalities.
Session Management: Ensure sessions are securely managed, allowing users to stay logged in across different devices.
#Real-Time Functionality
Real-Time Subscriptions: Utilize Supabase real-time subscriptions to ensure chat messages and updates are delivered instantly to all participants.
Event Listeners: Set up event listeners to handle real-time updates such as new messages, user status changes, and typing indicators.
#Storage
File Storage: Use Supabase storage for handling user-uploaded files like images and documents. Ensure efficient upload, retrieval, and display of files within the chat application.
#Security: I have also set up RLS policies on the table schema.


## Plasmic set-up guide 

    1. Initialization 
    2. import { initPlasmicLoader } from "@plasmicapp/loader-nextjs";
    3. export const PLASMIC = initPlasmicLoader({
    4.   projects: [
    5.     {
    6.       id: "PROJECTID",  // ID of a project you are using
    7.       token: "APITOKEN"  // API token for that project
    8.     }
    9.   ],
    10.   // Fetches the latest revisions, whether or not they were unpublished!
    11.   // Disable for production to ensure you render only published changes.
    12.   preview: true,
    13. })

  