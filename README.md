# Mood2Tunes

> **Note:** The Mood2Tunes web application is currently under maintenance as it awaits approval from the Spotify team to extend its API quota. Thank you for your patience.

Mood2Tunes is a web application designed to provide users with personalized music recommendations based on their mood. Built using modern technologies and hosted on AWS, it delivers a seamless user experience while leveraging the Spotify API for music recommendations.

![u1](https://github.com/duttasah26/Mood2Tunes/blob/main/mainUI%231.jpg)
![ui2](https://github.com/duttasah26/Mood2Tunes/blob/main/mainUI%232.jpg)

---

## Demo 🎥

[Watch the Demo Video](https://www.youtube.com/watch?v=kwZRr_PhnzU)

---

## Features 🎵

- **Mood-based Music Recommendations**: Enter your mood and receive a curated list of 10 songs.
- **User Authentication**: Secure sign-up and sign-in powered by AWS Cognito.
- **Responsive Frontend**: Built with React.js and hosted on AWS Amplify for scalability and reliability.
- **Serverless Backend**: Node.js backend hosted on AWS Lambda, ensuring efficient processing.
- **Data Logging**: User mood and interaction logs are stored in Amazon DynamoDB for potential future analytics.

---

## Architecture Diagram 🛠️

![Architecture Diagram](https://github.com/duttasah26/Mood2Tunes/blob/main/architecture-diagram.png)

---

## Development Infrastructure

- **Frontend**: React.js for an interactive UI
- **Backend**: Node.js for logic processing
- **API Integration**: Spotify API for personalized music recommendations
- **Version Control**: GitHub for collaboration and code management

---

## Cloud Infrastructure 🌩️

- **Amazon Cognito**: Manages authentication and authorization.
- **Amazon Amplify**: Hosts the React frontend and serves static files.
- **Amazon API Gateway**: Routes requests between the frontend and backend.
- **AWS Lambda**: Processes user requests and interacts with the Spotify API.
- **Amazon DynamoDB**: Stores user mood data and timestamps for future insights.

---

## Deployment Process 🚀

1. **Frontend Deployment**:
   - Run `npm run build` on the React project to generate static files.
   - Upload the build files to AWS Amplify for hosting.

2. **Backend Deployment**:
   - Package the Node.js backend code as a Lambda function.
   - Modify the code to adhere to AWS Lambda's handler format.

3. **API Gateway Configuration**:
   - Configure routes to connect frontend requests to the appropriate Lambda functions.
   - Enable CORS to facilitate secure communication.

4. **Authentication Setup**:
   - Set up a Cognito User Pool with email-based authentication.
   - Integrate Cognito login and registration into the frontend.

5. **Database Configuration**:
   - Create a DynamoDB table to log user moods and interaction data.

---

## Cost Estimate 💰

| Service           | Monthly Cost | Usage                                    |
|-------------------|--------------|------------------------------------------|
| AWS Amplify       | $1.33        | Hosts static frontend files             |
| Amazon Cognito    | $114.25      | Manages authentication for 1,000 users |
| Amazon API Gateway| $10.00       | Handles 10,000 API requests per month   |
| AWS Lambda        | $0.00        | Processes backend logic (free tier)     |
| Amazon DynamoDB   | $26.39       | Stores user mood logs                   |

---


## Future Enhancements 🔮

- Email users their recommended playlists using Amazon SES.
- Sentiment Analysis to generate playlists according to user entering any prompt using AWS Comprehend.
- Add caching via a CDN for faster loading times.
- Explore additional user analytics using DynamoDB.

For any questions or issues, feel free to contact us : @sahildutta.work@gmail.com or babice@sheridancollege.ca
