# REINNODROSS ♻️🎨

**REINNODROSS** is a full-stack MERN web application designed to foster a sustainable digital marketplace. It connects individuals looking to sell or donate scrap materials with artists and creators who transform these materials into innovative, eco-friendly products. This platform aims to promote a circular economy, environmental responsibility, and artistic innovation.

The project is divided into two main sections:
*   **Dross:** A marketplace for users to sell or donate unused or waste items.
*   **Reinnovate:** A gallery and shopfront for artists to showcase and sell their upcycled products.

---

## 📜 Table of Contents

*   [About The Project](#about-the-project)
*   [✨ Key Features](#-key-features)
*   [🛠️ Technology Stack](#️-technology-stack)
*   [🚀 Getting Started](#-getting-started)
    *   [Prerequisites](#prerequisites)
    *   [Installation](#installation)
*   [🔧 Usage](#-usage)
*   [🔮 Future Enhancements](#-future-enhancements)
*   [🤝 Contributing](#-contributing)
*   [📝 License](#-license)
*   [👥 Authors & Acknowledgements](#-authors--acknowledgements)

---

## 📖 About The Project

In an era where environmental sustainability is paramount, ReinnoDross presents a unique technological solution uniting ecological responsibility with artistic innovation. The platform addresses the gap between the rising amount of waste and the need for artists/designers to procure low-cost, reusable materials.

Existing platforms cater partially to these needs but fail to provide a streamlined, role-specific ecosystem for scrap acquisition, creative reuse, and eco-product marketing. ReinnoDross aims to:

*   Connect scrap sellers with upcycling artists (reinnovators) and eco-conscious buyers.
*   Facilitate the exchange of discarded materials and promote sustainable, repurposed products.
*   Promote a circular economy by extending the lifecycle of materials.
*   Empower artists and foster creative recycling.

---

## ✨ Key Features

*   **Role-Based Access Control:** Distinct dashboards and functionalities for:
    *   **Scrap Sellers:** List, manage, and sell/donate waste materials.
    *   **Reinnovators (Artists):** Source scrap, list, manage, and sell upcycled products.
    *   **Buyers:** Browse and purchase unique, eco-friendly upcycled products.
    *   **Admin:** Moderate listings, manage users, and oversee platform activity.
*   **Dual Marketplace:**
    *   **Dross Section:** For listing and discovering scrap materials.
    *   **Reinnovate Section:** For showcasing and selling upcycled creations.
*   **User Authentication & Management:** Secure registration, login (JWT-based), and profile management.
*   **Dynamic Product & Scrap Listings:** Users can upload, browse, update, and delete listings with images and descriptions.
*   **Image Hosting:** Integration with Cloudinary for efficient image storage and delivery.
*   **Shopping Cart & Order System:** Buyers can add products to a cart and proceed with a mock checkout process.
*   **Responsive Design:** User-friendly interface adaptable to various devices (desktop, tablet, mobile).
*   **Admin Moderation:** Admin panel for approving/rejecting listings and managing users.
*   **Search & Filtering:** Basic search and filtering capabilities for products and scrap items.

---

## 🛠️ Technology Stack

**Frontend:**
*   React.js
*   HTML5 & CSS3
*   JavaScript (ES6+)
*   React Router (for page navigation)
*   Bootstrap / Custom CSS (for responsive design)
*   Axios (for API calls)

**Backend:**
*   Node.js
*   Express.js (web application framework)
*   JWT (JSON Web Tokens for secure authentication)
*   Bcrypt.js (for password hashing)
*   `dotenv` (for environment configuration)
*   CORS (Cross-Origin Resource Sharing)

**Database:**
*   MongoDB (NoSQL database)
*   Mongoose (Object Data Modeling - ODM for MongoDB)

**Additional Tools:**
*   Cloudinary (for image hosting and transformation)
*   Visual Studio Code (Source code editor)
*   Git & GitHub (Version control and collaboration)
*   Postman (API testing)

---

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

*   Node.js (v14.x or later recommended)
*   npm (usually comes with Node.js) or yarn
*   MongoDB (local instance or a cloud-hosted version like MongoDB Atlas)
*   Git

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/REINNODROSS.git
    cd REINNODROSS
    ```

2.  **Backend Setup:**
    ```bash
    cd backend
    npm install
    ```
    *   Create a `.env` file in the `backend` directory.
    *   Copy the contents of `.env.example` (if provided) or add the following environment variables:
        ```env
        MONGO_URI=your_mongodb_connection_string
        JWT_SECRET=your_very_strong_jwt_secret
        PORT=5000 # Or any port you prefer for the backend
        CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
        CLOUDINARY_API_KEY=your_cloudinary_api_key
        CLOUDINARY_API_SECRET=your_cloudinary_api_secret
        ```

3.  **Frontend Setup:**
    ```bash
    cd ../frontend # Navigate back to the root and then to frontend
    npm install
    ```
    *   Create a `.env` file in the `frontend` directory (if needed for API base URL, though often handled in Axios configs).
        ```env
        REACT_APP_API_URL=http://localhost:5000/api # Example if your backend runs on port 5000
        ```

---

## 🔧 Usage

1.  **Start your MongoDB server** if you are running it locally.
2.  **Start the Backend Server:**
    ```bash
    cd backend
    npm start
    # Or if you have a dev script: npm run dev
    ```
    The backend server should typically start on `http://localhost:5000` (or the port specified in your `.env`).

3.  **Start the Frontend Development Server:**
    ```bash
    cd ../frontend
    npm start
    ```
    The React application will usually open automatically in your browser at `http://localhost:3000`.

Now you can interact with the application, register users with different roles (Seller, Artist, Buyer), list scrap, create upcycled products, and test the admin functionalities.

---




## 🔮 Future Enhancements

While ReinnoDross is functionally robust, several enhancements could further improve its impact:

*   **Integrated Payment Gateway:** Implement Stripe, Razorpay, or PayPal for real commercial transactions.
*   **Real-Time Messaging:** Add chat functionality (e.g., using Socket.IO) for communication between users.
*   **Advanced Search & Filtering:** More granular filtering options (location, material type, price range, popularity).
*   **Notifications System:** Email or in-app notifications for new listings, orders, admin actions.
*   **Rating & Review System:** Allow users to rate products and provide feedback.
*   **Mobile Application:** Develop a native or cross-platform mobile app (React Native/Flutter).
*   **Social Media Integration:** Allow artists to share profiles and products.
*   **Community Features:** Forums or discussion boards for sharing upcycling ideas.
*   **AI-Powered Recommendations:** Suggest scrap items to artists or products to buyers.
*   **Environmental Impact Tracker:** Show users their contribution to sustainability.

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📝 License

Distributed under the MIT License. See `LICENSE` file for more information.
*(You'll need to add a `LICENSE` file to your repository - the MIT license is a good default for open source projects.)*

---

## 👥 Authors & Acknowledgements

This project was submitted in partial fulfillment for the award of the Degree of Bachelor of Technology in Computer Science and Engineering/Information Technology at Dr. A.P.J. Abdul Kalam Technical University, Lucknow.

**Submitted by:**
*   Priyansh Srivastava (2100100130088)
*   Ritu Raj Singh (2100100130098)
*   Prajjwal Malviya (2100100130083)
*   Ritul Singh (2100100130099)

**Under the Supervision of:**
*   Mr. Ratish Kr. Srivastava (Assistant Professor, Department of Computer Science and Engineering, UCER Prayagraj)

**Institution:**
*   United College of Engineering & Research, Prayagraj

**Special Thanks:**
*   Dr. Swapnil Srivastava (Principal, UCER)
*   Dr. Vijay Kumar Dwivedi (Dean Academics & HOD, CSE/IT, UCER)
*   Mr. Shyam Bahadur Verma (Project Coordinator)
*   All authors of books, papers, and documentation consulted.
