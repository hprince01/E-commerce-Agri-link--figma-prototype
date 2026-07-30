# AgriLink Project Documentation

**Group Assignment IV-a — E-Commerce / Web Application UI/UX Design Using Figma**

| | |
|---|---|
| **Course** | INSY 8313 – Management Information System (MIS) |
| **Instructor** | Eric Maniraguha |
| **Institution** | Adventist University of Central Africa |

**Group Members**

| Name | ID |
|---|---|
| RUTAGENGWA Hirwa Prince | 20252NET100 |
| ISHIMWE Christian | 29766 |

---

## Selected Application

**AgriLink Figma Link:** https://www.figma.com/design/IfXTkpGSmVUgLobUUUafr1/Agrilink-Prototype?node-id=0-1&t=iApNPH8cNkE7j7u0-1

**AgriLink Github repo Link:** https://github.com/hprince01/E-commerce-Agri-link--figma-prototype/edit/main


---

## 1. Problem Statement

Farmers around Kigali (in areas such as Bugesera, Kamonyi, and the outskirts of Gasabo) currently sell the majority of their produce to middlemen at low, informal prices. These middlemen then transport and resell the produce at urban markets such as Kimironko and Nyabugogo at significantly higher prices, while the farmer — who does all the labor of growing the crop — receives the smallest share of the final price.

At the same time, urban buyers have no reliable, direct way to purchase fresh produce straight from the source, and must rely on informal, unregulated market transactions with no trust or quality assurance system.

**Target users:**
- Farmers in peri-urban areas around Kigali who currently rely on middlemen or word-of-mouth to sell their produce.
- Buyers in Kigali (individuals, small restaurants, and shop owners) who want fresher produce at fairer prices without visiting a physical market.

**Why this system matters:**
AgriLink digitizes an entirely informal, word-of-mouth agricultural supply chain. By connecting farmers and buyers directly, it removes the middleman markup, increases farmer income, lowers prices for buyers, and introduces a simple trust mechanism (ratings, verified pickup points) into a previously unregulated process. The app is designed around local payment realities (MTN Mobile Money and Airtel Money) rather than assuming card-based payment, making it realistic and usable in the Rwandan context.

---

## 2. User Personas

### Persona 1 — Buyer

| Field | Detail |
|---|---|
| **Name** | Kai |
| **Age** | 20 |
| **Occupation** | Young professional working in Kigali |
| **Location** | Kigali, Rebero |

**Goals**
- Buy fresh produce without traveling to a crowded physical market
- Pay conveniently using Mobile Money
- Know exactly where and when to pick up an order

**Challenges / Frustrations**
- Market produce is often not as fresh as expected
- No transparency in market pricing — prices vary depending on who is selling
- No easy way to know which farmer/seller is reliable

### Persona 2 — Farmer

| Field | Detail |
|---|---|
| **Name** | Jean Bosco |
| **Age** | 41 |
| **Occupation** | Smallholder tomato farmer |
| **Location** | Bugesera |

**Goals**
- Sell produce directly to buyers at a fair price
- Avoid depending entirely on middlemen who dictate low prices
- Reach more buyers than word-of-mouth allows

**Challenges / Frustrations**
- Limited access to buyers outside his local area
- Middlemen often underpay for produce
- No digital tools currently used in his selling process

---

## 3. User Flow Explanation

The application supports two parallel user journeys branching from a single entry point:

**Buyer flow:**
`Login/Sign up → Choose role (Buyer) → Home/Browse → Product Detail → Cart → Checkout (MTN Mobile Money / Airtel Money / Cash on Pickup) → Payment Confirmation → Order Confirmed → Profile → Log out`

**Farmer flow:**
`Login/Sign up → Choose role (Farmer) → Farmer Dashboard → Add Produce Listing / Manage Orders → Profile → Log out`

Both flows share the same entry (Login/Sign up) and exit (Profile/Log out) points, keeping the app's core navigation consistent regardless of user type. This was a deliberate design decision: rather than building two disconnected apps, AgriLink uses one shared shell with role-based branching, which keeps the experience predictable for both user types.

---

## 4. Wireframes (Low-Fidelity)

Low-fidelity wireframes were created in Figma as simple grayscale structural layouts before high-fidelity design, covering:

1. Login/Register page
2. Home page (browse/search)
3. Product detail page
4. Cart
5. Checkout page

These wireframes focused purely on layout, hierarchy, and navigation structure, without color, imagery, or final typography, to validate the flow before visual design began.


---

## 5. High-Fidelity UI Design

The high-fidelity design applies AgriLink's visual identity consistently across all screens:

- **Color palette:** Dark charcoal background (`#1a1a1a`), card surfaces (`#262626`), green accent (`#3aa66f`) for primary actions and highlights, amber/gold for ratings, and brand-accurate yellow/red for MTN Mobile Money and Airtel Money payment options.
- **Typography:** Clean sans-serif throughout, bold weights for headings and prices, regular/light gray for secondary information.
- **Imagery:** Real photographs of produce (tomatoes, carrots, red onions, avocado) rather than generic icons, to keep the marketplace feeling authentic.
- **Iconography:** Simple, consistent icon set for navigation (home, cart, orders, profile) and status indicators.

**Screens delivered (11 total, exceeding the minimum 6 required):**

1. Login
2. Sign Up
3. Home / Browse (Buyer)
4. Product Detail
5. Cart
6. Checkout (Payment Method Selection)
7. Payment Confirmation
8. Order Confirmed
9. Farmer Dashboard
10. Add Produce Listing
11. Orders (Farmer) / Buyer Profile

---

## 6. Interactive Prototype

All screens are connected in Figma's Prototype mode with the following interactions:

- Button taps navigate between screens (e.g. "Continue as buyer," "Add to Cart," "Proceed to Checkout")
- Product cards on the Home screen link to their respective Product Detail screens
- Bottom navigation icons (Home, Cart, Orders, Profile) link consistently across all buyer screens
- The Checkout → Payment Confirmation → Order Confirmed sequence includes a "Simulate confirmation" interaction to represent the real-world Mobile Money PIN confirmation step
- "Log Out" buttons on both the Farmer Dashboard and Buyer Profile screens return to the Login screen

**Figma Prototype Link:** `[paste your public "Anyone with the link can view" Figma link here]`

---

## 7. Accessibility Considerations

- **Font sizes:** Body text and labels are kept at readable sizes (minimum 11–12px for secondary text, 13–16px for primary content), avoiding overly small text anywhere in the flow.
- **Color contrast:** White and light gray text is used against dark surfaces to maintain strong contrast; green accents were chosen with sufficient contrast against both dark backgrounds and white card backgrounds.
- **Consistent navigation:** The bottom navigation bar and back arrows remain in the same position across every relevant screen, so users always know how to move forward or backward.
- **Clear affordances:** Buttons are visually distinct (solid green fill for primary actions, outlined/text style for secondary actions like "Log in with a different method"), so interactive elements are never ambiguous.
- **Local-context accessibility:** Payment options include Mobile Money and Cash on Pickup, rather than assuming card payment, making the app usable by the widest possible range of local users regardless of banking access.

---

## 8. Features Implemented

- Dual role-based flow (Buyer and Farmer) from a single login
- Product browsing with category filters and search
- Product detail view with farmer profile, rating, and story
- Shopping cart with pickup point selection
- Local payment method integration (MTN Mobile Money, Airtel Money, Cash on Pickup)
- Order confirmation flow with order number and pickup details
- Farmer-side listing management (add, view active listings)
- Farmer-side order management (view and track incoming orders)
- Shared Profile/Log out flow for both user types

---

## 9. Challenges Faced

- Balancing a single shared design system (colors, buttons, cards) across two distinct user flows (buyer vs. farmer) while keeping each flow feeling purpose-built.
- Ensuring realistic local context (RWF pricing, Kigali pickup points, Mobile Money) was reflected accurately throughout, rather than defaulting to generic e-commerce patterns.
- Managing prototype linking across 11 screens to ensure every interactive path (including back navigation and log out) worked correctly.

---

## 10. Conclusion

AgriLink demonstrates how a simple, well-scoped digital marketplace can address a real, everyday problem in the Kigali agricultural supply chain. By focusing on two clear user types, a locally relevant payment method, and a consistent visual identity, the prototype shows a complete, believable user experience from account creation through to a confirmed order — and from a farmer's perspective, from listing produce to managing incoming orders. The project reinforced the importance of designing for real local context (payment methods, geography, language) rather than defaulting to generic international app patterns.

---

## Asset Organization

```
AgriLink-Project/
│
├── wireframes/
│   ├── login-wireframe.png
│   ├── home-wireframe.png
│   ├── product-detail-wireframe.png
│   └── cart-checkout-wireframe.png
│
├── high-fidelity-designs/
│   ├── login.png
│   ├── signup.png
│   ├── home.png
│   ├── product-detail.png
│   ├── cart.png
│   ├── checkout.png
│   ├── payment-confirmation.png
│   ├── order-confirmed.png
│   ├── farmer-dashboard.png
│   ├── add-listing.png
│   └── buyer-profile.png
│
├── assets/
│   ├── agrilink-logo.svg
│   └── produce-photos/
│
└── prototype/
    └── figma-prototype-link.txt
```
