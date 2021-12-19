<div align="center">
<h1>Auction Site (client side)</h1>

This is the frontend for an Auction site built in React.js, where people can create an auction for their items, and also they can bid on items they like, and the highest bidder wins the auction.

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)![Redux](https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white)

</div>

Deployment: https://Deployment

While running locally: http://localhost:3000

Trello: https://trello.com/b/GMe6Tyz1/mp-project-ibrahimalsaif

Slides: https://Slides

## ⚫ User Stories

- A guest can browse the site a see all the available auctions without the need for sign-in.
- A guest must have an account and log-in if they want to use the site features.
- A user can bid on an auction.
- A user can add auctions in his own watch list.
- A user can create auctions for people to start bidding on.
- A user has his own dashboard with all of his information and statistics.
- A user can edit his information from name, avatar, ... etc.
- A user can edit his auction information.
- A user with role `admin` has all the features of a regular user.
- A user with role `admin` can change any auction status.
- A user with role `admin` has a dashboard with all of the site information and statistics.
- A user can report a scammer to the admin so he can't bid or create an auction again.

### ■ Installing Dependencies

#### ▸ Node js

Follow instructions to install the latest version of Node js for your platform in the [Node js docs](https://nodejs.org/en/).

#### ▸ NPM Dependencies

Once you have the project in your local machine, install dependencies by running:

```bash
npm install
```

This will install all of the required packages.

#### ▸ Key Dependencies

- [React](https://reactjs.org/) A JavaScript library for building user interfaces.

- [firebase](https://www.npmjs.com/package/firebase) provides the tools and infrastructure you need to develop, grow, and earn money from your app.

- [axios](https://www.npmjs.com/package/axios) is a promise based HTTP client for the browser and node.js.

- [redux](https://www.npmjs.com/package/redux) is a predictable state container for JavaScript apps.

- [react-redux](https://www.npmjs.com/package/react-redux) is a React bindings for Redux.

- [redux-devtools-extension](https://www.npmjs.com/package/redux-devtools-extension) is a debugging platform for Redux apps.

- [react-icons](https://react-icons.github.io/react-icons/) Include popular icons in your React projects easily with react-icons.

- [material-ui](https://mui.com/) MUI provides a robust, customizable, and accessible library of foundational and advanced components, enabling you to build your own design system and develop React applications faster.

- [sweetalert2](https://sweetalert2.github.io/) A Beautiful, Responsive, Customizable, Accessible (Wai-aria) Replacement For Javascript's Popup Boxes.

- [popup-tools](https://www.npmjs.com/package/popup-tools) Several simple tools to handle popups with callbacks. Posting data to popups as well as receiving data from them.

## ⚫ Running the server

To run the server, execute:

```bash
npm start
```

## ⚫ Router Routes

| Path                   | Component          | Permissions | Behavior                                                    |
| ---------------------- | ------------------ | ----------- | ----------------------------------------------------------- |
| `/`                    | Home               | public      | Home page, show items, about, how it works                  |
| `/explore`             | Explore            | public      | Shows all auctions                                             |
| `/explore/:id`         | Auction               | public      | See an auction description, and also you can bid               |
| `/users/:id`           | Profile            | public      | See a user profile, with all of his auctions                |
| `/signup`              | Signup             | public      | Signup form, navigate to login after signup                 |
| `/login`               | Login              | public      | Login form, navigate to home after login                   |
| `/addItem`             | createAuction            | user only   | Create a new auction                                        |
| `/EditItem`            | EditAuction           | user only   | Edit an auction                                             |
| `/dashboard`           | Dashboard          | user only   | Shows all of the user info                                  |
| `/dashboard/myAccount` | DashboardMyAccount | user only   | Shows all of the user info, and he/she can edit any info    |
| `/dashboard/myItems`   | DashboardMyAuctions   | user only   | Shows all of the user auctions, and he/she can edit any auction   |
| `/dashboard/myBids`    | DashboardMyBids    | user only   | Shows all of the user bids                                  |
| `/dashboard/watchList`    | DashboardWatchList    | user only   | Shows the user watch list                                  |
| `/dashboard/items`     | DashboardAuctions     | admin only  | Shows all auctions in site                                  |
| `/dashboard/users`     | DashboardUsers     | admin only  | Shows all users in site                                  |
| `/dashboard/reports`   | DashboardReports   | admin only  | Shows reports in the site, and admin can change their status |
| `/verify_account/id`   | VerifyTheAccount   | user only   | A page enables the user to activate their account           |
| `/verify_from_email`   | VerifyFromEmail    | user only   | A wlecome page to a user after register                     |
| `/reset_password/id`   | ResetPassword      | user only   | A page to let a user change his password                    |

## ⚫ Components

- Home
- Explore
- Auction
- Profile
- Login
- Signup
- CreateAuction
- EditAuction
- Dashboard
- DashboardMyAccount
- DashboardMyAuctions
- DashboardWatchList
- DashboardMyBids
- DashboardAuctions
- DashboardUsers
- DashboardReports
- VerifyTheAccount
- VerifyFromEmail
- ResetPassword

## ⚫ UML Diagram

![masterpiece frontend UML](https://user-images.githubusercontent.com/92247874/146672674-67833d1b-51d5-452f-828b-f5eea7948574.jpg)


## ⚫ Wireframes

### ■ Home

![Home](https://user-images.githubusercontent.com/92247874/146651652-062c54f7-c315-457d-8439-67372b5867e2.png)

### ■ Explore

![Explore](https://user-images.githubusercontent.com/92247874/146651658-dd326c65-147b-4847-9e50-386704e6bc59.png)

### ■ Auction

![Item](https://user-images.githubusercontent.com/92247874/146651738-abe1ef8d-11ec-445c-b3d3-f5fce5b4152a.png)


### ■ Profile

![Profile](https://user-images.githubusercontent.com/92247874/146651744-7848b363-4842-4fc4-aa2b-d912e97a19f4.png)


### ■ Login

![Login](https://user-images.githubusercontent.com/92247874/146651749-787bf85a-004c-49db-a7d9-945f41755ded.png)


### ■ Signup

![Signup](https://user-images.githubusercontent.com/92247874/146651751-d5769588-358d-4a52-bbdb-227868d5766b.png)


### ■ CreateAuction

![add item](https://user-images.githubusercontent.com/92247874/146651752-dbc3bac2-d037-46bd-bcbc-7c4ed48ba150.png)


### ■ EditAuction

![edit item](https://user-images.githubusercontent.com/92247874/146651757-339daf02-430d-4ac3-8ae3-8aae70bee333.png)


### ■ DashboardMyAccount

![DashboardMyAccount](https://user-images.githubusercontent.com/92247874/146651770-591be60a-c07b-4f01-958d-1dbd4b988f56.png)


### ■ DashboardMyAuctions

![DashboardMyItems](https://user-images.githubusercontent.com/92247874/146651772-3171bb6e-81ac-422e-ae29-dcdfd4645ec8.png)


### ■ DashboardWatchList

![DashboardWatchList](https://user-images.githubusercontent.com/92247874/146651773-57703a8c-16c1-4db2-b50f-792b6b32ae07.png)


### ■ DashboardMyBids

![DashboardMyBids](https://user-images.githubusercontent.com/92247874/146651775-84fcff87-e9fe-491d-a9df-27b13e7c0f43.png)

### ■ DashboardAuctions

![DashboardItems](https://user-images.githubusercontent.com/92247874/146651778-2444978b-c7ee-48b4-80c8-7fca99ed7b86.png)

### ■ DashboardUsers

![DashboardUsers](https://user-images.githubusercontent.com/92247874/146651791-e705f3f1-dc6c-4533-a888-34afa39e95a0.png)


### ■ DashboardReports

![DashboardReports](https://user-images.githubusercontent.com/92247874/146651783-b540d31a-aba7-4094-8628-ea7e20dbc5bd.png)


