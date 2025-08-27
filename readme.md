# Commerce Project

A simple e-commerce platform with Django REST API backend and planned React frontend.

## 📁 Project Structure

```
Commerce/
├── Django/          # Backend API
└── Frontend/        # React app (planned)
```

## 🚀 Django Backend (Completed)

**Models:**
- `User` - Customer accounts with authentication
- `Product` - Items with SKU, price, categories
- `Category` - Hierarchical product categories (tree structure)
- `Order` & `OrderItem` - Shopping cart and order management

**API Endpoints:**
```
# Categories (for menus)
GET  /api/v1/categories/           # Root categories
GET  /api/v1/categories/tree/      # Complete nested tree
POST /api/v1/categories/create/    # Create category
PUT  /api/v1/categories/{id}/update/  # Update category

# Products, Orders, Users (existing endpoints)
```

**Features:**
- ✅ Clean response utilities
- ✅ Pydantic validation schemas  
- ✅ Service layer architecture
- ✅ Django admin interface
- ✅ Hierarchical categories for frontend menus

## 📋 TODO: React Frontend

### Core Features
- [ ] Product catalog with category navigation
- [ ] Hierarchical menu system using category tree API
- [ ] Shopping cart functionality
- [ ] User authentication/registration
- [ ] Order management
- [ ] Responsive design

### Technical Setup
- [ ] Create React app with TypeScript
- [ ] Set up API client (axios/fetch)
- [ ] State management (Context API or Redux)
- [ ] Routing (React Router)
- [ ] UI framework (Material-UI, Tailwind, or similar)

### Category Menu Implementation
- [ ] Fetch category tree from `/api/v1/categories/tree/`
- [ ] Build recursive menu components
- [ ] Implement dropdown/mega-menu navigation
- [ ] Category-based product filtering

### Pages Needed
- [ ] Home page with featured products
- [ ] Product listing with category filters
- [ ] Product detail pages
- [ ] Shopping cart
- [ ] Checkout flow
- [ ] User account pages

## 🔧 Development

**Backend:** Django REST Framework with clean architecture  
**Frontend:** React + TypeScript (planned)  
**Database:** SQLite (dev) / PostgreSQL (prod)
