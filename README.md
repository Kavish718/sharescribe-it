# ShareScribe-It

ShareScribe-It is a subscription-sharing platform designed to help people reduce the cost of subscriptions they use occasionally. It connects users with similar subscription interests so they can share eligible plans and split costs, making subscriptions more affordable while giving users access to a wider range of services and potential sharing partners.

Subscriptions are organised into five categories: **Streaming, Education, Productivity, Magazines, and Music**.

## Features

- **User accounts:** Register and sign in to manage a personal account.
- **Preference matching:** Select subscription categories and record subscription preferences to find users with similar interests.
- **Subscription listings:** Browse subscriptions that other users are willing to share.
- **Share an existing subscription:** Add subscription details such as the service, cost, and billing cycle.
- **Profile management:** View and update personal subscription preferences.
- **Payment flow:** Includes a payment form and processing page.
- **Provider links:** Visit a subscription provider's official website when no shareable listing is available.

## Technology Stack

- **Frontend:** HTML, CSS
- **Backend:** PHP
- **Database:** MySQL
- **Matching approach:** SQL queries that match users based on their selected subscription interests

## Database Structure

The application uses the `subscriptionapp` database, with the following main tables:

- `users` – stores user account information.
- `user_preferences` – stores users' selected preferences.
- `subscriptions` – stores subscription details and sharing information.

## Project Structure

```text
sharescribe-it/
├── css/          # Stylesheets for the application's pages
├── images/       # Image assets
├── php/          # PHP pages and backend logic
├── index.html    # Login and registration entry page
└── README.md
```

The PHP directory contains the application's account, preference, subscription-listing, profile, and payment workflows.

## Getting Started

### Prerequisites

- A local PHP development environment (for example, XAMPP, WAMP, or MAMP).
- MySQL.
- A web browser.

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/Kavish718/sharescribe-it.git
   ```

2. Move the project folder into your local web server's document root (for example, `htdocs` when using XAMPP).

3. Start the Apache and MySQL services.

4. Create a MySQL database named `subscriptionapp`.

5. Configure the database connection in `php/config.php` with your local MySQL host, username, password, and database name.

6. If a database schema or seed script is available in your project materials, import it into `subscriptionapp` before using the application. The repository documentation identifies the `users`, `user_preferences`, and `subscriptions` tables.

7. Open the application in your browser through your local server, for example:

   ```text
   http://localhost/sharescribe-it/
   ```

## How It Works

1. A user creates an account or signs in.
2. The user selects subscription categories and records their preferences.
3. ShareScribe-It uses SQL queries to find users with matching subscription interests.
4. Users can browse available shared subscriptions or add a subscription they are willing to share.
5. When no suitable shared option is listed, users can follow a link to the service provider.

## Subscription Categories

- Streaming
- Education
- Productivity
- Magazines
- Music

## Note

This repository documents a prototype subscription-sharing application. Configure the database locally before running it, and use test data and a safe test environment when exploring the payment workflow. Do not store real payment-card details or share account credentials through the application.
