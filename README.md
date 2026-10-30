# Smart India Hackathon Workshop
# Date:30/10/2026
## Reference Number:26018924
## Name:KIRUSH J

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution

1. Detailed explanation
FarmDirect is a mobile app and website where farmers and FPOs list their crops with price and quantity. Consumers and bulk buyers (hotels, retailers, hostels) order directly from them. Our delivery partners handle pickup and delivery, and the farmer gets paid through UPI. AI predicts demand and plans the best delivery routes.
2. How it addresses the problem
No middlemen means the farmer keeps more of the price.
Buyers get fresh produce at a lower price.
Logistics support solves the transport problem for small farmers.
AI reduces waste by telling farmers what to grow and sell.
3. Innovation and uniqueness
AI demand forecasting, so farmers know the likely demand before harvest.
Route optimization that combines orders from nearby farms to cut transport cost.
Voice and regional language support (Tamil, Hindi) for less-educated farmers.
A fair price suggestion that uses mandi rates and demand.
Support for FPOs and bulk orders, not just single buyers.

## Technical Approach

1. Technologies
Frontend: Flutter (mobile app), React (website)
Backend: Node.js with Express
Database: PostgreSQL / MongoDB
AI/ML: Python with Prophet / LSTM for demand forecasting; Google OR-Tools for route optimization
Maps: Google Maps API
Payments: UPI / Razorpay
Notifications: SMS and WhatsApp API
Hosting: AWS / Firebase
2. Methodology
Farmer registers and lists the crop (type, quantity, price, location).
Buyer searches and places an order.
The AI model suggests a fair price and predicts demand.
The system groups nearby orders and plans the best route.
A delivery partner picks up from the farm and delivers to the buyer.
Payment goes straight to the farmer's account.
Ratings and feedback improve the system.

Flowchart:

FARMDIRECT
                        |
      +-----------------+-----------------+
      |                 |                 |
   SELLERS            PLATFORM           BUYERS
(Farmers / FPOs)     (App + AI)    (Consumers / Bulk)
      |                 |                 |
 Register & login   Verifies users     Register & login
      |                 |                 |
 List crop:             |             Search crops
 type, qty, price       |             near them
      |                 |                 |
      +--------> AI ENGINE <--------------+
                        |
         +--------------+--------------+
         |              |              |
      Demand        Fair price       Route
     forecast      suggestion     optimization
   (Prophet/LSTM)  (mandi rates)  (OR-Tools)
         |              |              |
         +--------------+--------------+
                        |
                  Buyer places order
                        |
                 Orders grouped by area
                        |
                  LOGISTICS SUPPORT
                        |
         +--------------+--------------+
         |                             |
   Pickup from farm /          Delivery partner
   village collection point    takes best route
         |                             |
         +--------------+--------------+
                        |
                  Quality check
                        |
                Delivered to buyer
                        |
                 PAYMENT (UPI)
                        |
         +--------------+--------------+
         |                             |
  Money goes directly           Small platform fee
  to farmer                     for delivery
                        |
                Ratings & feedback
                        |
          Data goes back to AI to improve
          (loop returns to AI ENGINE)

          
## Feasibility and Viability

1. Feasibility
Most Indians already use smartphones and UPI, so adoption is realistic.
All the technologies are open-source or low-cost.
Government data (Agmarknet, e-NAM) is available for training the AI.
FPOs already exist, so we can partner with them to onboard farmers.
2. Challenges and risks
Many farmers have low digital literacy.
Poor internet in villages.
Perishable produce can spoil in transit.
Trust issues about quality and payments.
Delivery cost for small orders.
3. Strategies to overcome them
Voice-based, regional language app with a simple UI.
Offline mode and SMS support.
Collection points near villages and fast delivery slots.
Quality grading, ratings, and secure payments.
Order grouping and bulk orders to reduce delivery cost.
Training through FPOs and local volunteers.

## Impact and Benefits

1. Impact on the target audience
Farmers/FPOs: higher income and a direct market.
Consumers: fresher food at lower prices.
Bulk buyers: steady supply and transparent pricing.
Government: better price monitoring and data.
2. Benefits
Social: empowers small farmers and builds trust between farmers and buyers.
Economic: better prices for farmers, lower prices for buyers, and less loss in the supply chain.
Environmental: less food waste and fewer vehicle trips from route optimization.

## Research and References

e-NAM (National Agriculture Market): https://enam.gov.in
Agmarknet (mandi price data): https://agmarknet.gov.in
Ministry of Consumer Affairs, Food & Public Distribution: https://consumeraffairs.nic.in
NABARD reports on FPOs: https://www.nabard.org
FAO reports on food supply chains and food loss: https://www.fao.org
Google OR-Tools (route optimization): https://developers.google.com/optimization
Prophet (forecasting library): https://facebook.github.io/prophet
