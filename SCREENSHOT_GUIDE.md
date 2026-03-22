# Screenshot Capture Guide - FASTAPI Food Delivery App

## **IMPORTANT: Manual Screenshot Upload Required**

This guide documents the 20 screenshots that need to be captured and uploaded.

## Swagger UI URL
**https://sturdy-waddle-7vw76r9pj6qw2r4g-8000.app.github.dev/docs**

---

## Required Screenshots (20 Total)

### Q1_home.png - Swagger UI Homepage
- **URL**: /docs
- **Description**: Main Swagger UI interface showing all available endpoints
- **Content**: Full page view of all 16 endpoints listed

### Q2_get_menu.png - GET /menu  
- **Endpoint**: GET /menu
- **Description**: Retrieve complete menu with all items
- **Action**: Click endpoint → Try it out → Execute
- **Capture**: Request + Response with menu items array

### Q3_get_by_id.png - GET /menu/{item_id}
- **Endpoint**: GET /menu/{item_id}
- **Description**: Get specific menu item by ID
- **Parameters**: item_id = 1
- **Capture**: Request + Response showing single menu item

### Q4_menu_summary.png - GET /menu/summary
- **Endpoint**: GET /menu/summary
- **Description**: Get menu summary statistics
- **Capture**: Response showing total items, available, unavailable, categories

### Q5_search_menu.png - GET /menu/search
- **Endpoint**: GET /menu/search
- **Parameters**: keyword = "Pizza"
- **Capture**: Search results with matching items

### Q6_sort_menu_by_price.png - GET /menu/sort
- **Endpoint**: GET /menu/sort
- **Parameters**: sort_by = "price", order = "asc"
- **Capture**: Sorted menu items

### Q7_paginate.png - GET /menu/page
- **Endpoint**: GET /menu/page
- **Parameters**: page = 1, limit = 3
- **Capture**: Paginated results

### Q8_browse.png - GET /menu/browse
- **Endpoint**: GET /menu/browse
- **Parameters**: keyword = "Burger", sort_by = "price"
- **Capture**: Browse results

### Q9_filter_menu.png - GET /menu/filter
- **Endpoint**: GET /menu/filter
- **Parameters**: category = "Pizza", is_available = true
- **Capture**: Filtered menu items

### Q10_get_orders.png - GET /orders
- **Endpoint**: GET /orders
- **Description**: Retrieve all orders
- **Capture**: Orders array response

### Q11_create_order.png - POST /orders
- **Endpoint**: POST /orders
- **Request Body**: 
```json
{
  "customer_name": "John Doe",
  "item_id": 1,
  "quantity": 2,
  "delivery_address": "123 Main Street, Hyderabad",
  "order_type": "delivery"
}
```
- **Capture**: Request body + Success response

### Q12_search_orders.png - GET /orders/search
- **Endpoint**: GET /orders/search
- **Parameters**: customer_name = "John"
- **Capture**: Search results

### Q13_add_to_cart.png - POST /cart/add
- **Endpoint**: POST /cart/add
- **Parameters**: item_id = 1, quantity = 2
- **Capture**: Cart item added response

### Q14_view_cart.png - GET /cart
- **Endpoint**: GET /cart
- **Description**: View current cart
- **Capture**: Cart items with grand total

### Q15_remove_from_cart.png - DELETE /cart/{item_id}
- **Endpoint**: DELETE /cart/{item_id}
- **Parameters**: item_id = 1
- **Capture**: Item removed confirmation

### Q16_checkout.png - POST /cart/checkout
- **Endpoint**: POST /cart/checkout
- **Request Body**:
```json
{
  "customer_name": "Jane Smith",
  "delivery_address": "456 Park Avenue, Hyderabad"
}
```
- **Capture**: Checkout success with orders

### Q17_root_endpoint.png - GET /
- **Endpoint**: GET /
- **Description**: Root welcome endpoint
- **Capture**: Welcome message response

### Q18_schemas.png - Data Schemas
- **Location**: Scroll down to "Schemas" section
- **Content**: CheckoutRequest, OrderRequest schemas
- **Capture**: Schema definitions

### Q19_validation_errors.png - Validation Errors
- **Content**: HTTPValidationError, ValidationError schemas
- **Capture**: Error schema structures

### Q20_response_examples.png - Response Examples
- **Content**: Sample response bodies and headers
- **Capture**: Various response examples from any endpoint

---

## How to Upload Screenshots

1. **Capture all 20 screenshots** using Windows Snipping Tool (Win+Shift+S)
2. **Name them exactly**: Q1_home.png, Q2_get_menu.png, etc.
3. **Upload to this repository**:
   - Go to repository main page
   - Click "Add file" → "Upload files"
   - Drag and drop all 20 PNG files
   - Commit with message: "Add all 20 endpoint screenshots"

---

## Repository Structure (Target)
```
FASTAPI_FOOD_DELIVERY_APP/
├── main.py
├── SCREENSHOT_GUIDE.md (this file)
├── Q1_home.png
├── Q2_get_menu.png
├── Q3_get_by_id.png
├── Q4_menu_summary.png
├── Q5_search_menu.png
├── Q6_sort_menu_by_price.png
├── Q7_paginate.png
├── Q8_browse.png
├── Q9_filter_menu.png
├── Q10_get_orders.png
├── Q11_create_order.png
├── Q12_search_orders.png
├── Q13_add_to_cart.png
├── Q14_view_cart.png
├── Q15_remove_from_cart.png
├── Q16_checkout.png
├── Q17_root_endpoint.png
├── Q18_schemas.png
├── Q19_validation_errors.png
└── Q20_response_examples.png
```

---

**Server URL**: https://sturdy-waddle-7vw76r9pj6qw2r4g-8000.app.github.dev/docs
**Student ID**: IN226001602
**Project**: QuickBite Food Delivery System
