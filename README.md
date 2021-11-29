# E-Commerce Back End

## descritption:

This project is the creation of the back end for an e-commerce site. This application used Express.js API and Sequelize to interact with a MySQL database. This application displays creation of database using mySQL with models and associations. Then demonstrates the API Routes to perform RESTful CRUD operations displayed in my walk through videos.

## Installation:

The user should clone the repository from GitHub. This application requires Node.js, Express.js, and Sequelize. To connect to the database run mysql -u root -p and enter password from .env file. Then source the schema.sql. To seed the file run npm run seed. Finally to connect to the server run npm start.

### Database Models:

Database contain the following four models:

- `Category`

  - `id`

    - Integer.

    - Doesn't allow null values.

    - Set as primary key.

    - Uses auto increment.

  - `category_name`

    - String.

    - Doesn't allow null values.

- `Product`

  - `id`

    - Integer.

    - Doesn't allow null values.

    - Set as primary key.

    - Uses auto increment.

  - `product_name`

    - String.

    - Doesn't allow null values.

  - `price`

    - Decimal.

    - Doesn't allow null values.

    - Validates that the value is a decimal.

  - `stock`

    - Integer.

    - Doesn't allow null values.

    - Set a default value of `10`.

    - Validates that the value is numeric.

  - `category_id`

    - Integer.

    - References the `Category` model's `id`.

- `Tag`

  - `id`

    - Integer.

    - Doesn't allow null values.

    - Set as primary key.

    - Uses auto increment.

  - `tag_name`

    - String.

- `ProductTag`

  - `id`

    - Integer.

    - Doesn't allow null values.

    - Set as primary key.

    - Uses auto increment.

  - `product_id`

    - Integer.

    - References the `Product` model's `id`.

  - `tag_id`

    - Integer.

    - References the `Tag` model's `id`.

### Walkthrough Video: 37%

- [View video to see MySQL walk through via Screencastify](https://watch.screencastify.com/v/4YWfCyXDf0vqb60v5TsB)

- [View video to walk through of the API routes.](https://watch.screencastify.com/v/b1DfAWBg59c5Exa1jvuh)

- View video to see Insomnia walk through via screencastify for the following:

[products](https://watch.screencastify.com/v/meHzFpv0pH7DDZqx69yO)

[category](https://watch.screencastify.com/v/k7K9HMVG6VdpMfzAE5bC)

[tags](https://watch.screencastify.com/v/58Ze8zJiLOPbIsa6zm3h)

### Contact me:

- [ GITHUB.](https://github.com/mandy2324)

- [ LINKEDIN.](https://www.linkedin.com/in/m23saini)

- [Email](m23saini@gmail.com)
