# Laravel E-Commerce Website with Stripe Payment Gateway

This project is a fully-functional **Laravel-based e-commerce website** built to facilitate online shopping with support for **Stripe payment gateway** integration. It provides a robust platform to manage products, categories, and subcategories, as well as a seamless shopping experience with features like product combos, a shopping cart, and checkout options.

### Features
- **User-friendly shopping cart**: Add, edit, and remove products in the cart.
- **Product Management**: Manage products in different categories and subcategories.
- **Product Combos**: Create product combos to provide bundle discounts and increase sales.
- **Order Checkout**: Supports both **Stripe payments** and **Cash on Delivery (COD)** options.
- **Twilio Integration**: Send SMS notifications to users for order confirmations and updates.
- **Mail Integration**: Automated email notifications for order status and confirmation.
- **Category & Subcategory Management**: Easily manage your product catalog through categories and subcategories.
- **Responsive Design**: Fully responsive and ready for production.

### Tech Stack
- **Backend**: Laravel (PHP framework)
- **Frontend**: Blade Templates (HTML, CSS, JS)
- **Database**: MySQL
- **Payment Gateway**: Stripe
- **SMS Service**: Twilio
- **Email Service**: SMTP (Mail)

## Installation Steps

Follow these instructions to get the project up and running on your local machine or server.

### Prerequisites
Make sure you have the following installed:

- **PHP 8.0 or higher**
- **Composer** (for managing PHP dependencies)
- **MySQL** or any other compatible database
- **Node.js and NPM** (for frontend assets compilation)
- **Git** (for cloning the repository)

### 1. Download and Clone the Repository

To download the project, you need to clone the GitHub repository. Run the following command:

```bash
git clone https://github.com/your-username/Laravel-E-commerce-website-with-stripe-payment-gateway.git
```

```bash
cd Laravel-E-commerce-website-with-stripe-payment-gateway
```
### 2. Install PHP and JavaScript Dependencies

- **Install the backend dependencies using Composer:**
  ```bash
    composer install
  ```
  
- **Install frontend dependencies using NPM:**
  ```bash
    npm install
  ```
  ### 3. Set up the Environment
  
- **Copy the example environment file to create your own** `.env` **file:**
  ```bash
    cp .env.example .env
  ```
  ### 4. Configure Environment Variables

- **Open the** `.env` **file and configure the following          variables:**
  ```bash
    DB_DATABASE=your_database_name
    DB_USERNAME=your_database_username
    DB_PASSWORD=your_database_password
  ```
- **Stripe Configuration:**
  ```bash
    STRIPE_KEY=your_stripe_key
    STRIPE_SECRET=your_stripe_secret
  ```
- **Twilio Configuration:**
  ```bash
   TWILIO_SID=your_twilio_sid
   TWILIO_AUTH_TOKEN=your_twilio_auth_token
   TWILIO_PHONE_NUMBER=your_twilio_phone_number
  ```
- **Mail Configuration** (for sending emails):
  ```bash
    MAIL_MAILER=smtp
    MAIL_HOST=smtp.gmail.com  # Or your preferred mail service
    MAIL_PORT=587
    MAIL_USERNAME=your-email@example.com
    MAIL_PASSWORD=your-email-password
    MAIL_FROM_ADDRESS=your-email@example.com
    MAIL_FROM_NAME="Your Store Name"
  ```
- **5. Generate Application Key**
- Run the following command to generate your application's encryption key:
 ```bash
    php artisan key:generate
 ```
- **6. Run Database Migrations**
- Next, run the database migrations to create the necessary tables in your database:
  ```bash
    php artisan migrate
  ```
- **7. Compile Frontend Assets**
- To compile the frontend assets (CSS, JavaScript), run the following command:
  ```bash
    npm run dev
  ```
- For a build, run:
  ```bash
      npm install
      npm run dev
  ```
- **8. Start the Development Server**
- Run the Laravel development server:

```bash
  php artisan serve
```
- **10. Access the Application**
- You can now access the application in your browser by navigating to:

  ```bash
    http://127.0.0.1:8000
  ```

This will start the application at http://127.0.0.1:8000.
### 11. Testing Payment Flow

#### Stripe:
- Use **Stripe's test keys** and test card numbers (e.g., `4242 4242 4242 4242`) for testing payments.
- Ensure that the **Stripe payment gateway** works correctly by making a test purchase.

#### Cash on Delivery (COD):
- The checkout process supports the **Cash on Delivery (COD)** option.
- Test this by selecting **COD** as the payment method during checkout.

---

### Notes

- **Twilio**: Integration allows sending **SMS notifications** for order confirmations and updates.
- **Mail**: **Email notifications** are sent to users for order confirmations and status updates.
- **Replace Placeholders**: Ensure you replace all placeholder values (`your-...`) in the `.env` file and the code with actual API keys, credentials, and values.



  












