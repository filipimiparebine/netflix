# Netflix clone

Netflix clone using `react`, `redux`, `firebase` and `stripe`

![Homepage](https://github.com/filipblajiu/netflix/blob/main/src/img/demo.jpg?raw=true)

![Profile](https://github.com/filipblajiu/netflix/blob/main/src/img/demo2.jpg?raw=true)

## Functionality

1. Sign up with email using Firebase Auth
2. Get movies from The Movie Database (TMDB) API
3. Manage subscription plans with Firebase Firestore DB and Stripe

## Installation

1. Clone the project
2. Install dependencies using `yarn` or `npm i`
3. Create a firebase project
4. Add stripe/firestore-stripe-payments extension to the firebase project
5. Set up the extension after instalation (`https://console.firebase.google.com/u/0/project/[PROJECT-ID]/extensions/instances/firestore-stripe-payments?tab=details`)
6. Create subscription plan products in stripe dashboard

![Stripe subscription plan product example](https://github.com/filipblajiu/netflix/blob/main/src/img/demo3.jpg?raw=true)

7. Add firebaseRole=[plan_type] metadata to each product subscription plan to eliminate one extra query
8. Create a `.env` file and update the credentials (see `.env_example`)
9. Run the project using `yarn start` or `npm run start`
