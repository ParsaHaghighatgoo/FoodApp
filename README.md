# 🍔 FoodApp

A comprehensive food ordering application built with JavaFX, designed to streamline the process of browsing restaurants, managing shopping carts, and placing orders.

## 📋 Overview

FoodApp is a desktop application that provides a complete food ordering system with features for managing restaurants, menu items, user accounts, shopping carts, and order processing. The application uses JavaFX for the user interface and follows object-oriented design principles.

## ✨ Features

- **Restaurant Management**: Browse restaurants with details including location, minimum purchase requirements, and coordinates
- **Menu System**: View food items with prices, photos, and detailed descriptions organized by categories
- **Shopping Cart**: Add items to cart, manage quantities, and calculate totals
- **Order Processing**: Place orders with delivery address and track order status
- **User Management**: User authentication and profile management
- **Delivery System**: Calculate delivery fees based on location
- **Feedback System**: Submit and manage customer feedback
- **Working Hours**: Display restaurant operating hours

## 🏗️ Architecture

The project follows a layered architecture with clear separation of concerns:

### Core Classes

- **User**: Manages user information (ID, name, phone)
- **Restaurant**: Handles restaurant data (name, location, minimum purchase, coordinates)
- **Item**: Represents menu items with pricing and details
- **ShoppingCart**: Manages cart items with quantities and timestamps
- **Order**: Processes orders with status tracking
- **OrderDetail**: Stores individual order line items
- **Address**: Manages delivery addresses
- **Category**: Organizes items into categories
- **ItemCategory**: Links items to categories
- **DeliveryFee**: Calculates delivery costs
- **Feedback**: Handles customer reviews and ratings
- **WorkingTime**: Manages restaurant operating hours

### Data Access Layer

- **UserDAO**: Data access object for user operations

## 🛠️ Technology Stack

- **Java 22**: Latest Java features and performance improvements
- **JavaFX 22**: Modern UI framework for desktop applications
- **Maven**: Dependency management and build automation
- **JUnit 5.10.0**: Unit testing framework

## 📦 Prerequisites

- Java Development Kit (JDK) 22 or higher
- Apache Maven 3.6 or higher
- JavaFX 22 SDK

## 🚀 Getting Started

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ParsaHaghighatgoo/FoodApp.git
   cd FoodApp
   ```

2. **Build the project**
   ```bash
   mvn clean install
   ```

3. **Run the application**
   ```bash
   mvn javafx:run
   ```

### Maven Commands

- **Compile**: `mvn compile`
- **Test**: `mvn test`
- **Package**: `mvn package`
- **Clean**: `mvn clean`

## 📁 Project Structure

```
FoodApp/
├── src/
│   └── main/
│       ├── java/
│       │   ├── Classes/           # Domain models
│       │   │   ├── User.java
│       │   │   ├── Restaurant.java
│       │   │   ├── Item.java
│       │   │   ├── ShoppingCart.java
│       │   │   ├── Order.java
│       │   │   ├── OrderDetail.java
│       │   │   ├── Address.java
│       │   │   ├── Category.java
│       │   │   ├── ItemCategory.java
│       │   │   ├── DeliveryFee.java
│       │   │   ├── Feedback.java
│       │   │   └── WorkingTime.java
│       │   ├── DaoClasses/        # Data access objects
│       │   │   └── UserDAO.java
│       │   └── org/example/foodapp/  # Application entry point
│       └── resources/
│           └── org/example/foodapp/
│               └── hello-view.fxml
├── pom.xml
└── README.md
```

## 🎯 Key Functionalities

### Shopping Cart Management
The `ShoppingCart` class provides functionality to:
- Add items with timestamps
- Track quantities
- Calculate totals based on item prices
- Manage cart items per user

### Order Processing
The order system supports:
- Order creation with delivery addresses
- Status tracking (pending, processing, delivered, etc.)
- Order details with multiple items
- Integration with delivery fee calculation

### Restaurant Features
- Minimum purchase requirements
- Geographic coordinates for location-based services
- Photo management
- City-based filtering

## 🧪 Testing

Run the test suite using:
```bash
mvn test
```

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Development Guidelines

- Follow Java naming conventions
- Write unit tests for new features
- Document public APIs with JavaDoc
- Keep classes focused and cohesive
- Use meaningful variable and method names

## 🔮 Future Enhancements

- Database integration (MySQL/PostgreSQL)
- Payment gateway integration
- Real-time order tracking
- Mobile application version
- Admin dashboard
- Advanced search and filtering
- Recommendation system
- Multi-language support

## 📄 License

This project is available for educational and personal use.

## 👤 Author

**Parsa Haghighatgoo**

- GitHub: [@ParsaHaghighatgoo](https://github.com/ParsaHaghighatgoo)

## 🙏 Acknowledgments

- JavaFX community for excellent documentation
- Maven for simplified dependency management
- JUnit for robust testing framework

---

**Note**: This is a work in progress. Features and documentation are continuously being updated.
