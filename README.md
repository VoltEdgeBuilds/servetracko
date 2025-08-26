# Local Micro-Business Tool - Setup Instructions

## 🚀 Quick Setup

### 1. Update Supabase Configuration
Replace `YOUR_SUPABASE_URL` and `YOUR_SUPABASE_ANON_KEY` in all HTML files with your actual Supabase credentials:

```javascript
const supabaseUrl = 'https://your-project.supabase.co';
const supabaseKey = 'your-anon-key-here';
```

**Files to update:**
- index.html
- dashboard.html
- orders.html
- customers.html
- invoice.html
- payments.html
- plan_payment.html

### 2. Database Setup
Your Supabase database is already configured with the provided schema. The tables include:
- users
- customers
- orders
- invoices
- payments
- subscriptions

### 3. Features Implemented

#### ✅ Authentication
- Email/password signup and login
- No email confirmation required
- Automatic user profile creation

#### ✅ Business Management
- Customer management with WhatsApp integration
- Order tracking with status updates
- Invoice generation with preview
- Payment tracking and reminders

#### ✅ Plan Management
- Free, Plus (₹99/month), Pro (₹299/month)
- Secure payment processing simulation
- Plan upgrade functionality

#### ✅ WhatsApp Integration
- Send order updates to customers
- Payment reminders
- Invoice notifications

### 4. File Structure
```
local/
├── index.html          # Login/Register & Plan Selection
├── dashboard.html      # Main Navigation Hub
├── orders.html         # Order Management
├── customers.html      # Customer Management
├── invoice.html        # Invoice Creation & Management
├── payments.html       # Payment Tracking
├── plan_payment.html   # Plan Upgrade & Payment
└── README.md          # This file
```

### 5. Usage Flow
1. **index.html** - User registers/logs in and selects plan
2. **dashboard.html** - Main hub with navigation cards
3. **customers.html** - Add and manage customer information
4. **orders.html** - Create orders linked to customers
5. **invoice.html** - Generate invoices from completed orders
6. **payments.html** - Track payment status and send reminders
7. **plan_payment.html** - Upgrade to paid plans

### 6. Key Features
- **Offline-first**: Works without internet for basic operations
- **Mobile-friendly**: Responsive design for mobile devices
- **Bilingual support**: English and Malayalam labels
- **WhatsApp integration**: Direct messaging to customers
- **Plan restrictions**: Free plan limited to 5 invoices/month
- **Professional invoices**: Watermarked based on plan

### 7. Next Steps
1. Replace Supabase credentials in all files
2. Test the complete flow
3. Customize business types and services as needed
4. Add real payment gateway integration (Razorpay)

### 8. Security Notes
- Row Level Security (RLS) is enabled
- Users can only access their own data
- No sensitive data stored in localStorage
- Secure authentication via Supabase

## 🛠️ Customization
- Modify plan prices in `plan_payment.html`
- Add more business types in `index.html`
- Customize invoice templates in `invoice.html`
- Update WhatsApp message templates as needed

## 📱 Mobile Support
All pages are fully responsive and work well on mobile devices, perfect for local business owners who primarily use smartphones.
