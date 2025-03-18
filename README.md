# Lead Management System (LMS)  

## Overview  
The Lead Management System (LMS) is a comprehensive C++ program designed to manage leads (users), products, and their interactions. The core focus of this project is the Score System and Tier System for Leads, which categorizes users and products based on their engagement and performance. This system rewards users with membership tiers and products with categories, unlocking exclusive privileges, discounts, and benefits.  

The LMS also includes features for user authentication, product management, shopping cart functionality, order history, personalized messaging, and admin controls.  

---

## Core Focus: Score System and Tier System  

### 1. User Score System  
User scores are a measure of a lead's engagement and activity within the system. Scores are earned through actions like purchasing products, adding items to the cart, and saving items.  

#### How Scores Are Earned  
- Purchasing a product: Users earn 0.05 * product cost price points.  
- Adding to cart: Users earn 0.03 * product cost price points.  
- Saving an item: Users earn 0.02 * product cost price points.  

#### Membership Tiers  
Membership tiers are determined by user scores and unlock exclusive privileges:  

1. General Tier (Score: 0 - 99):  
   - Basic access to the system.  
   - No additional privileges.  
   - Standard pricing on all products.  

2. Gold Tier (Score: 100 - 149):  
   - 5% discount on all purchases.  
   - Access to exclusive Gold-tier products.  
   - Priority customer support.  
   - 10% discount during their birthday month.  

3. Diamond Tier (Score: 150+):  
   - 10% discount on all purchases.  
   - Access to exclusive Diamond-tier products.  
   - Free shipping on all orders.  
   - 15% discount during their birthday month.  
   - Personalized recommendations based on order history.  

---

### 2. Product Score System  
Product scores are a measure of a product's popularity and sales performance. Scores are earned through units sold and user interactions like adding to cart or saving.  

#### How Scores Are Earned  
- Units sold: Products earn 0.005 * product cost price points per unit sold.  
- Added to cart: Products earn 0.003 * product cost price points.  
- Saved by users: Products earn 0.002 * product cost price points.  

#### Product Categories  
Product categories are determined by scores and influence pricing and visibility:  

1. Low Category (Score: 0 - 19):  
   - Standard pricing (1.25 * cost price).  
   - Limited visibility in the product catalog.  

2. Medium Category (Score: 20 - 49):  
   - Reduced pricing (1.15 * cost price).  
   - Highlighted in the product catalog.  
   - Eligible for promotional campaigns.  

3. High Category (Score: 50+):  
   - Discounted pricing (1.05 * cost price).  
   - Featured prominently in the product catalog.  
   - Exclusive to Gold and Diamond users.  

---

## Full Feature Guide  

### 1. User Features  
1. Signup:  
   - Users can create an account by providing their name, email, password, and birthday.  
   - Birthday is used for personalized discounts and reminders.  

2. Login:  
   - Users can log in using their email and password.  

3. View Items:  
   - Users can view all available products, categorized by their scores (Low, Medium, High).  

4. Buy Item:  
   - Users can purchase a product directly.  
   - Earns points based on the product's cost price.  

5. Add to Cart:  
   - Users can add products to their shopping cart.  
   - Earns points based on the product's cost price.  

6. View Cart:  
   - Users can view the items in their cart and the total cost.  
   - Discounts are applied based on the user's membership tier.  

7. Order Cart:  
   - Users can place an order for all items in their cart.  
   - Earns points for each product purchased.  

8. Save Item:  
   - Users can save items for later.  
   - Earns points based on the product's cost price.  

9. View Saved Items:  
   - Users can view their saved items.  

10. View Messages:  
    - Users can view personalized messages, such as:  
      - Reminders for past orders.  
      - Birthday month discounts.  
      - Special person's birthday reminders.  

11. Add Special Person's Birthday:  
    - Users can add birthdays of special people to receive reminders.  

12. View Dashboard:  
    - Users can view their profile information, including:  
      - Score and membership tier.  
      - Number of items in cart and saved items.  
      - Unread messages and special person birthdays.  

---

### 2. Admin Features  
1. Add Product:  
   - Admins can add new products with a name and cost price.  

2. Delete Product:  
   - Admins can delete products.  

3. View All Products:  
   - Admins can view all available products, categorized by their scores.  

4. View Users by Category:  
   - Admins can view users categorized by their membership tier (General, Gold, Diamond).  

5. View Products by Category:  
   - Admins can view products categorized by their score (Low, Medium, High).  

6. View Dashboard:  
   - Admins can view system statistics, such as:  
     - Total number of users.  
     - Total number of products.  

---

### 3. Personalized Messaging  
The system sends personalized messages to users based on their activity and special dates:  
- Order Reminders:  
  - "Last year in this month, you ordered [Product Name]. Would you like to order it again?"  
- Birthday Month Discounts:  
  - "It's your birthday month! Enjoy a [10%/15%] discount on all orders."  
- Special Person's Birthday Reminders:  
  - "[Name]'s birthday is in this month! Would you like to order something for them?"  

---

### 4. Scoring and Tier System Benefits  

#### For Users  
- General Tier: Basic access to the system.  
- Gold Tier:  
  - 5% discount on all purchases.  
  - Access to exclusive Gold-tier products.  
  - Priority customer support.  
  - 10% birthday month discount.  
- Diamond Tier:  
  - 10% discount on all purchases.  
  - Access to exclusive Diamond-tier products.  
  - Free shipping on all orders.  
  - 15% birthday month discount.  
  - Personalized recommendations.  

#### For Products  
- Low Category: Standard pricing and visibility.  
- Medium Category: Reduced pricing and highlighted visibility.  
- High Category: Discounted pricing, featured visibility, and exclusivity for Gold and Diamond users.  

---

## Example Use Case  

### User Journey  
1. A user signs up and starts purchasing products.  
2. After purchasing $500 worth of products, their score reaches 100, upgrading them to Gold tier.  
3. They now enjoy:  
   - A 5% discount on all purchases.  
   - Access to exclusive Gold-tier products.  
   - A 10% discount during their birthday month.  
4. As they continue to engage, their score reaches 150, upgrading them to Diamond tier.  
5. They now enjoy:  
   - A 10% discount on all purchases.  
   - Free shipping on all orders.  
   - A 15% discount during their birthday month.  

### Product Journey  
1. A product is added with a cost price of $100.  
2. Initially, it is categorized as Low and priced at $125.  
3. As users purchase and interact with the product, its score increases.  
4. When the score reaches 20, it is categorized as Medium and priced at $115.  
5. When the score reaches 50, it is categorized as High and priced at $105, becoming exclusive to Gold and Diamond users.  

---

## Conclusion  
The Lead Management System (LMS) leverages a robust Score System and Tier System to reward leads (users) and products based on their engagement and performance. This system encourages user loyalty, promotes high-performing products, and provides a seamless experience for both users and administrators.  

This project is ideal for hackathons, as it combines data-driven decision-making (scores and tiers) with user-centric features (personalized messaging, discounts, and exclusive benefits).
