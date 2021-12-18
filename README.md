# Social Media Website

This is the frontend for an Auction site built in React.js, where people can create an auction for their items, and also they can bid on items they like, and the highest bidder wins the auction.

While running locally: http://localhost:3000

## User Stories

- A user can browse the website a see all the available products without the need for sign-in.
- A user must have an account and log-in if they want to use website features.
- A logged-in user can bid on an item.
- A logged-in user can add items in his own watch list.
- A logged-in user can add items for people to start bidding on.
- A logged-in user has his own dashboard with all of his information and statistics.
- A logged-in user can edit his information from name, avatar, ... etc.
- A logged-in user can edit his bids information.
- A logged-in user can delete his bids.
- A logged-in user with role `admin` has all the features of a regular user.
- A logged-in user with role `admin` can delete any bid.
- A logged-in user with role `admin` has a dashboard with all of the website information and statistics.
- A user can report a scammer to the admin so he can't bid again.

## Getting Started

### Installing Dependencies

#### Node js

Follow instructions to install the latest version of Node js for your platform in the [Node js docs](https://nodejs.org/en/).

#### NPM Dependencies

Once you have the project in your local machine, install dependencies by running:

```bash
npm install
```

This will install all of the required packages.

##### Key Dependencies

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

## Running the server

To run the server, execute:

```bash
npm start
```

## Router Routes

| Path                   | Component          | Permissions | Behavior                                                    |
| ---------------------- | ------------------ | ----------- | ----------------------------------------------------------- |
| `/`                    | Home               | public      | Home page, show items, about, how it works                  |
| `/explore`             | Explore            | public      | Shows all items                                             |
| `/explore/:id`         | Item               | public      | See an Item description, and also you can bid               |
| `/users/:id`           | Profile            | public      | See a user profile, with all of his auctions                |
| `/signup`              | Signup             | public      | Signup form, navigate to login after signup                 |
| `/login`               | Login              | public      | Login form, navigate to todos after login                   |
| `/addItem`             | addItem            | user only   | Create a new auction                                        |
| `/EditItem`            | EditItem           | user only   | Edit an auction                                             |
| `/dashboard`           | Dashboard          | user only   | Shows all of the user info                                  |
| `/dashboard/myAccount` | DashboardMyAccount | user only   | Shows all of the user info, and he/she can edit any info    |
| `/dashboard/myItems`   | DashboardMyItems   | user only   | Shows all of the user items, and he/she can edit any item   |
| `/dashboard/myBids`    | DashboardMyBids    | user only   | Shows all of the user bids                                  |
| `/dashboard/items`     | DashboardItems     | admin only  | Shows all items in website                                  |
| `/dashboard/users`     | DashboardUsers     | admin only  | Shows all users in website                                  |
| `/dashboard/reports`   | DashboardReports   | admin only  | Shows reports in website, and admin can change their status |
| `/verify_account/id`   | VerifyTheAccount   | user only   | A page enables the user to activate their account           |
| `/verify_from_email`   | VerifyFromEmail    | user only   | A wlecome page to a user after register                     |
| `/reset_password/id`   | ResetPassword      | user only   | A page to let a user change his password                    |

## Components

- Login
- Signup
- Home
- Explore
- Item
- Profile
- addItem
- EditItem
- Dashboard
- DashboardMyAccount
- DashboardMyItems
- DashboardMyBids
- DashboardItems
- DashboardUsers
- DashboardReports
- VerifyTheAccount
- VerifyFromEmail
- ResetPassword

## UML Diagram

## Wireframes
