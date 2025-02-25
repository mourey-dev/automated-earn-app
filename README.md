# Automated Earn App

The "Automated Earn App" is a web application that integrates with the Gmail API to automate the process of checking for specific promotional emails and performing actions based on their content. The app is designed to help users quickly identify and interact with promotional emails that contain specific keywords or phrases, such as "Did You Win".

## Key Features

- **Google Authentication**: Securely sign in with your Google account using Google's OAuth 2.0.
- **Token Management**: Handles access tokens and refresh tokens to maintain user sessions and refresh access tokens when they expire.
- **Email Filtering**: Lists all messages in the user's inbox under the "CATEGORY_PROMOTIONS" label and filters messages based on specific keywords in the subject line.
- **Message Display**: Displays the full content of the message, including any links that match a specific structure.
- **Automated Actions**: Triggers actions such as clicking on links within the email and deleting the email after the action is performed.
- **User Interface**: Provides a simple user interface with buttons to authorize and sign out, and a content area to display messages and results.

## How It Works

1. **Authorization**: Users click the "Authorize" button to sign in with their Google account. The app requests access to the user's Gmail account with the necessary scopes.
2. **Token Handling**: The app saves the access token and refresh token to local storage. If the access token expires, the app uses the refresh token to obtain a new access token.
3. **Listing Messages**: The app lists messages in the user's inbox under the "CATEGORY_PROMOTIONS" label and checks each message's subject for the keyword "Did You Win".
4. **Displaying Messages**: If a matching message is found, the app displays the full content of the message, including any links that match a specific structure.
5. **Automated Actions**: The app can trigger actions such as clicking on links within the email and deleting the email after the action is performed.
6. **Sign Out**: Users can click the "Sign Out" button to revoke the access token and clear the session.
