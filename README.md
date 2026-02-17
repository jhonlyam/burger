# Pizza App - React Native Pizza Delivery Application

A comprehensive React Native pizza delivery application demonstrating meaningful application logic with multiple functional screens, authentication, cart management, and order history.

## Features

### 🍕 Core Functionality
- **User Authentication**: Login and registration with AsyncStorage
- **Pizza Menu**: Browse pizzas by categories with detailed information
- **Shopping Cart**: Add items, adjust quantities, and calculate totals
- **Order Management**: Complete checkout process with order history
- **User Profile**: Manage personal information and preferences

### 🎨 UI/UX Features
- **Multiple Navigation Types**: Stack, Drawer, Bottom Tabs, and Top Tabs navigation
- **Vector Icons**: React Native Vector Icons for enhanced visual clarity
- **Responsive Design**: Flexbox layouts for different screen sizes
- **Reusable Components**: Custom buttons, inputs, cards, and more
- **Modal Confirmations**: Alerts for important actions

### 🔧 Technical Implementation
- **React Hooks**: useState, useEffect, useContext, useMemo, useCallback
- **Custom Hooks**: useAsyncStorage, useOrders for business logic separation
- **Context API**: AuthContext and CartContext for global state management
- **AsyncStorage**: Primary data storage solution
- **Clean Architecture**: Proper separation of concerns

## Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── Button.js
│   ├── Input.js
│   └── Card.js
├── context/            # React Context providers
│   ├── AuthContext.js
│   └── CartContext.js
├── constants/          # App constants and data
│   ├── colors.js
│   └── pizzaData.js
├── hooks/              # Custom React hooks
│   ├── useAsyncStorage.js
│   └── useOrders.js
├── navigation/         # Navigation configuration
│   ├── AuthNavigator.js
│   ├── AppNavigator.js
│   └── RootNavigator.js
├── screens/            # App screens
│   ├── auth/           # Authentication screens
│   │   ├── LoginScreen.js
│   │   └── RegisterScreen.js
│   └── main/           # Main app screens
│       ├── HomeScreen.js
│       ├── MenuScreen.js
│       ├── PizzaDetailScreen.js
│       ├── CartScreen.js
│       ├── CheckoutScreen.js
│       ├── OrderHistoryScreen.js
│       └── ProfileScreen.js
└── utils/              # Utility functions
```

## Getting Started

> **Note**: Make sure you have completed the [Set Up Your Environment](https://reactnative.dev/docs/set-up-your-environment) guide before proceeding.

### Prerequisites

- Node.js (>= 20)
- React Native CLI
- Android Studio / Xcode
- Metro bundler

### Installation

1. Clone the repository
2. Install dependencies:
```sh
npm install
```

3. For iOS, install CocoaPods:
```sh
cd ios && pod install && cd ..
```

### Running the App

#### Start Metro
```sh
npm start
```

#### Run on Android
```sh
npm run android
```

#### Run on iOS
```sh
npm run ios
```

## App Features in Detail

### Authentication Flow
- User registration with email, name, and phone validation
- Login with email and password
- Persistent authentication using AsyncStorage
- Profile management and updates

### Pizza Ordering System
- Browse pizzas by categories (Classic, Specialty, Vegetarian, Meat Lovers)
- Detailed pizza information with ingredients and pricing
- Size selection (Small, Medium, Large)
- Custom toppings with additional pricing
- Add to cart with quantity management

### Shopping Cart
- Real-time cart updates
- Item quantity adjustment
- Remove items with confirmation
- Subtotal and total calculation
- Delivery fee integration

### Checkout Process
- Delivery information input
- Payment method selection
- Order summary with itemized pricing
- Order placement with confirmation

### Order History
- View all past orders
- Filter orders by status
- Order tracking and management
- Cancel pending orders

### User Profile
- View and edit personal information
- Manage delivery address
- App settings and preferences
- Logout functionality

## Technical Implementation Details

### State Management
- **AuthContext**: User authentication state and methods
- **CartContext**: Shopping cart state and operations
- **AsyncStorage**: Persistent data storage

### Navigation Structure
- **RootNavigator**: Conditional rendering based on auth state
- **AuthNavigator**: Login and registration screens
- **AppNavigator**: Main app navigation with drawer and tabs

### Custom Hooks
- **useAsyncStorage**: Generic AsyncStorage operations
- **useOrders**: Order management and persistence

### UI Components
- **Button**: Customizable button with multiple variants
- **Input**: Form input with validation and icons
- **Card**: Reusable card component with styling

## Dependencies

### Core Dependencies
- `react`: 19.2.0
- `react-native`: 0.83.1

### Navigation
- `@react-navigation/native`
- `@react-navigation/stack`
- `@react-navigation/drawer`
- `@react-navigation/bottom-tabs`
- `@react-navigation/material-top-tabs`

### UI & Storage
- `react-native-vector-icons`
- `@react-native-async-storage/async-storage`
- `react-native-safe-area-context`
- `react-native-screens`
- `react-native-gesture-handler`
- `react-native-reanimated`

## Contributing

This project was created as a demonstration of React Native development best practices and comprehensive app functionality.

## License

This project is for educational purposes.
