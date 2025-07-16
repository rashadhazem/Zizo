# Zizo
Zizo Restaurant - ASP.NET MVC Website project:
# Zizo Restaurant - ASP.NET MVC Website

A complete responsive restaurant website for "Zizo" specializing in traditional Egyptian cuisine, built with ASP.NET MVC 8.0 and C#.

## 🍽️ Features

### Customer Features
- **Responsive Design**: Works perfectly on mobile, tablet, and desktop
- **Modern UI**: Clean white background with bright orange accents
- **Advanced Menu System**: Browse categories with advanced filtering, sorting, and search
- **Shopping Cart**: Add items, adjust quantities, and manage cart with real-time updates
- **Online Ordering**: Complete checkout process with multiple payment methods
- **User Authentication**: Register, login, and manage orders
- **Order Tracking**: View order history and status with real-time updates
- **Customer Reviews & Ratings**: Rate and review menu items
- **Loyalty Program**: Earn points with every order and redeem for discounts
- **Advanced Search**: Search by name, description, category, and dietary preferences
- **Dietary Filters**: Filter by vegetarian, spicy, gluten-free, and halal options
- **Price Range Filtering**: Filter items by price range
- **Multiple Sorting Options**: Sort by price, name, popularity, and ratings

### Admin Features
- **Advanced Dashboard**: Overview of orders, revenue, popular items, and analytics
- **Category Management**: Add, edit, and delete menu categories with image upload
- **Menu Item Management**: Full CRUD operations for menu items with advanced options
- **Order Management**: View, update status, and manage all orders with real-time tracking
- **Image Upload**: Upload and manage images for categories and menu items
- **Review Management**: Moderate and approve customer reviews
- **Loyalty Program Management**: Manage loyalty points and rewards
- **Discount Management**: Create and manage promotional codes
- **Analytics & Reports**: Detailed sales and customer analytics
- **Customer Management**: View customer profiles and order history

### Technical Features
- **ASP.NET MVC 8.0**: Latest framework with modern features
- **Entity Framework Core**: Database-first approach with SQL Server
- **Identity System**: User authentication and authorization
- **Session Management**: Shopping cart functionality
- **Payment Integration**: Stripe payment processing
- **Responsive Design**: Bootstrap 5 with custom CSS
- **Modern JavaScript**: Interactive features and animations

## 🎨 Design Theme

- **Primary Colors**: White background with bright orange (#ff6b35) accents
- **Typography**: Poppins font family for modern, clean look
- **Animations**: Smooth hover effects and page transitions
- **Icons**: Font Awesome icons throughout the interface
- **Responsive**: Mobile-first design approach

## 🚀 Getting Started

### Prerequisites
- .NET 8.0 SDK
- SQL Server (LocalDB or full instance)
- Visual Studio 2022 or VS Code

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd ZizoRestaurant
   ```

2. **Restore dependencies**
   ```bash
   dotnet restore
   ```

3. **Update database connection**
   - Open `appsettings.json`
   - Update the connection string to match your SQL Server instance

4. **Run database migrations**
   ```bash
   dotnet ef database update
   ```

5. **Run the application**
   ```bash
   dotnet run
   ```

6. **Access the application**
   - Main site: `https://localhost:5001`
   - Admin panel: `https://localhost:5001/Admin`

### Default Admin Account
- **Email**: admin@zizo.com
- **Password**: Admin123!

## 📁 Project Structure

```
ZizoRestaurant/
├── Controllers/           # Main controllers
├── Models/               # Data models
├── Views/                # Razor views
├── Data/                 # Database context and migrations
├── Areas/
│   └── Admin/           # Admin area
│       ├── Controllers/ # Admin controllers
│       ├── Models/      # Admin view models
│       └── Views/       # Admin views
├── wwwroot/             # Static files
│   ├── css/            # Stylesheets
│   ├── js/             # JavaScript files
│   └── images/         # Images
└── Program.cs          # Application entry point
```

## 🗄️ Database Schema

### Core Tables
- **Categories**: Menu categories (Koshary, Clay Pots, Pastries, etc.)
- **MenuItems**: Individual menu items with prices and descriptions
- **Orders**: Customer orders with status tracking
- **OrderItems**: Individual items within orders
- **AspNetUsers**: User accounts (extends Identity)

### Sample Data
The application includes seeded data with:
- 5 menu categories
- 15 menu items across all categories
- Admin user account

## 💳 Payment Integration

The application supports multiple payment methods:
- **Cash on Delivery**
- **Credit/Debit Cards** (via Stripe)
- **Mobile Wallets**

To enable Stripe payments:
1. Sign up for a Stripe account
2. Update the Stripe keys in `appsettings.json`
3. Test with Stripe's test card numbers

## 🎯 Key Features Explained

### Shopping Cart
- Session-based cart storage
- Real-time quantity updates
- Special instructions for items
- Persistent across browser sessions

### Menu Filtering
- Category-based filtering
- Search functionality
- Dietary preference filters (vegetarian, spicy)
- Responsive grid layout

### Admin Panel
- Secure admin area with role-based access
- Dashboard with key metrics
- Full CRUD operations for menu management
- Order status management

## 🔧 Customization

### Adding New Categories
1. Log in as admin
2. Navigate to Admin > Categories
3. Click "Add Category"
4. Upload image and fill details

### Adding Menu Items
1. Navigate to Admin > Menu Items
2. Click "Add Menu Item"
3. Select category and fill details
4. Upload item image

### Styling Changes
- Main styles: `wwwroot/css/site.css`
- Color variables defined in CSS root
- Responsive breakpoints included

## 🚀 Deployment

### Local Development
```bash
dotnet run --environment Development
```

### Production Deployment
1. Update connection string for production database
2. Set environment to Production
3. Configure HTTPS certificates
4. Set up proper logging

## 📱 Mobile Responsiveness

The website is fully responsive with:
- Mobile-first design approach
- Touch-friendly navigation
- Optimized images and layouts
- Fast loading times

## 🔒 Security Features

- **Authentication**: ASP.NET Core Identity
- **Authorization**: Role-based access control
- **CSRF Protection**: Anti-forgery tokens
- **Input Validation**: Model validation and sanitization
- **Secure Headers**: HTTPS enforcement

## 🧪 Testing

The application includes:
- Model validation
- Form validation
- Error handling
- User-friendly error messages

## 📞 Support

For questions or issues:
- Check the documentation
- Review the code comments
- Test with the provided sample data

## 📄 License

This project is created for educational and demonstration purposes.

---

**Zizo Restaurant** - Bringing authentic Egyptian cuisine to your table! 🇪🇬 
