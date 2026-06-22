Here is the end-to-end blueprint for building your two-phase marketing strategy generation system tailored specifically for the food industry.
------------------------------
## 1. Universal JSON Structure & Phase 1 Input Fields
To keep the application highly scannable, predictable, and simple for non-marketers, collect user data using this exact JSON schema.

{
  "business_type": "food_service", 
  "business_name": "Mama's Artisanal Pizza",
  "core_offering": "Sourdough pizzas with locally sourced toppings",
  "target_audience": "families_and_foodies",
  "price_point": "premium",
  "primary_channel": "dine_in_and_takeaway",
  "main_competitor_flaw": "Mass-produced, greasy fast-food pizzas nearby",
  "business_goal": "increase_weekend_orders",
  "selected_framework": "4P"
}

## UI Input Fields Mapping

* Business Type: Dropdown or Radio (food_service or food_product).
* Business Name: Short text input.
* What do you sell? (Core Offering): Short text area with examples like "Vegan burgers" or "Bottled hot sauce".
* Who buys from you? (Target Audience): Multi-select tags (Families, Students, Health-conscious, Busy professionals).
* Pricing Style (Price Point): Dropdown (Budget-friendly, Mid-range, Premium/Luxury).
* How do customers buy? (Primary Channel): Multi-select tags (Dine-in, Takeaway, Online delivery, Grocery retail, E-commerce website).
* What makes you better than competitors? (Competitor Flaw): Open text box mapping to their unique value.
* What is your immediate goal? (Business Goal): Dropdown (Get more foot traffic, Launch new item, Boost online sales, Build local awareness).
* Choose a Strategy Framework: Dropdown (SWOT, STP, 4P, SOSTAC, RACE, AARRR). [1] 

------------------------------
## 2. Optimal Prompt-Generation Engine Template
Your backend code should ingest the JSON data above and compile it into a unified framework prompt. Below is the master template your system will use to construct the final prompt sent to Gemini Flash 2.5.

You are an expert AI Marketing Strategist specializing in the Food Service and Packaged Food Product industries. 

Your task is to take the basic business attributes provided below and transform them into a highly sophisticated, comprehensive marketing strategy following the strict guidelines of the selected framework.
### INPUT DATA- Business Type: {{business_type}}- Business Name: {{business_name}}- Core Offering: {{core_offering}}- Target Audience Focus: {{target_audience}}- Price Positioning: {{price_point}}- Distribution Channels: {{primary_channel}}- Competitive Edge Focus: {{main_competitor_flaw}}- Ultimate Strategy Goal: {{business_goal}}
### COMPLIANCE RULES1. Framework Strictness: You must exclusively utilize the {{selected_framework}} framework.2. Structure Continuity: Follow the exact Markdown layout, section order, and headers provided in the Framework Specification. Do not omit any section.3. Industry Execution: Contextualize all tactical recommendations for food constraints (e.g., foot traffic, food margins, perishability, shelf-life, local SEO, sensory marketing).4. Accessibility vs Value: Write so a non-marketer can understand the actions immediately, but ensure the underlying strategy is robust enough for a professional agency to execute.5. Diagramming: Include the specific Mermaid diagram specified for this framework to visually summarize data.
### FRAMEWORK SPECIFICATION[System will append the matching section from Item 5 & 6 here]

------------------------------
## 3. Example Prompt-Generation Outputs (Food Service vs. Food Product)## Example A: Food Service (Restaurant) Appended Segment

### SYSTEM DIRECTIVE FOR FOOD SERVICE (SWOT ANALYSIS)Apply the input details to a physical restaurant environment. - "Strengths" must evaluate menu quality, kitchen speed, and physical location vibes.- "Weaknesses" must address seasonal foot traffic patterns or high operating margins.- "Opportunities" must check local event partnerships or food delivery app optimization.- "Threats" must look into rising ingredient supply costs or local competing diners.
[Append SWOT Markdown Structure & Mermaid Diagram here]

## Example B: Food Product (Packaged CPG) Appended Segment

### SYSTEM DIRECTIVE FOR FOOD PRODUCT (4P ANALYSIS)Apply the input details to a retail consumer packaged food product.- "Product" must evaluate packaging design, nutrition labeling, and unboxing shelf-life.- "Price" must analyze retail margin structures, MSRP, or bulk bundle discounts.- "Place" must map out grocery store shelving placement, distributor networks, or Direct-to-Consumer e-commerce.- "Promotion" must cover in-store sampling events, digital coupon drops, or food-influencer unboxing campaigns.
[Append 4P Markdown Structure & Mermaid Diagram here]

------------------------------
## 4. Framework Output Formats & Mermaid Diagram Alignments
To ensure your output structure remains completely consistent across different businesses, map each framework to these exact Markdown templates and visual diagrams.
## Framework 1: SWOT Analysis

# Marketing Strategy for [Business Name]: SWOT Analysis
## 1. Executive SummaryBrief non-technical breakdown of how to use this SWOT strategy to achieve the goal of: [Goal].
## 2. SWOT Matrix Diagram```mermaid
quadrantChart
    title SWOT Matrix Analysis
    x-axis Internal Factors --> External Factors
    y-axis Negative Impacts --> Positive Impacts
    quadrant-1 Opportunities
    quadrant-2 Strengths
    quadrant-3 Weaknesses
    quadrant-4 Threats
    "Menu Quality / Product Taste": [0.3, 0.8]
    "High Operational Costs": [0.2, 0.2]
    "Local Event Catering Trends": [0.8, 0.7]
    "Competitor Price Undercutting": [0.7, 0.3]
```
## 3. Detailed Framework Breakdown*   **Strengths (Internal / Positive):** [3 precise bullets tailored to food quality, staff, or location]
*   **Weaknesses (Internal / Negative):** [3 precise bullets covering operational issues or cost bottlenecks]
*   **Opportunities (External / Positive):** [3 precise bullets on local trends, delivery platforms, or partnerships]
*   **Threats (External / Negative):** [3 precise bullets focusing on competition or supply chain shifts]
## 4. Tactical Action Plan (TOWS Matrix Alignment)*   **SO Strategy (Using Strengths to capture Opportunities):** [Actionable step]
*   **WO Strategy (Overcoming Weaknesses by exploiting Opportunities):** [Actionable step]

## Framework 2: STP (Segmentation, Targeting, Positioning)

# Marketing Strategy for [Business Name]: STP Framework
## 1. Executive SummaryOverview of the core audience market segments and how [Business Name] stands out.
## 2. Customer Segmentation Tree```mermaid
graph TD
    A[Total Market] --> B[Segment 1: Health-Conscious Foodies]
    A --> C[Segment 2: Busy Convenience Seekers]
    B --> D[Targeted: High Priority Focus]
    C --> E[Secondary Focus]
```
## 3. Detailed Framework Breakdown### Market Segmentation*   **Demographics:** [Age, Income bracket, Occupation]
*   **Psychographics:** [Food values, Lifestyle choice, Dietary restrictions]
*   **Behavioral:** [Occasion of purchase, Loyalty frequency]
### Target Market Selection*   **Primary Target Profile:** Detailed pen-portrait of the ideal food buyer.*   **Justification:** Why this specific group solves the stated business goal.
### Positioning Strategy*   **Value Proposition:** The definitive reason why they choose this food over competitors.
*   **Positioning Statement:** "For [Target Group] who need [Need], [Business Name] provides [Offering] because of [Core Edge]."
## 4. Tactical Action Plan*   [Actionable step to reach target segment via tailored messaging]

## Framework 3: 4Ps (Marketing Mix)

# Marketing Strategy for [Business Name]: The 4Ps Mix
## 1. Executive SummaryHow to balance the product, price, placement, and promotion variables to hit targets.
## 2. Marketing Mix Core Connection```mermaid
mindmap
  root((4Ps Marketing Mix))
    Product
      Core Offering
      Food Packaging Style
    Price
      Menu Strategy
      Value Impression
    Place
      Store Front/Retail
      Delivery Network
    Promotion
      Sensory Marketing
      Local Social Ads
```
## 3. Detailed Framework Breakdown*   **Product:** [Food flavor details, presentation, portion sizing, packaging materials, or shelf-life features]
*   **Price:** [Pricing strategy explained simply, margins, competitive matching vs premium tiering]
*   **Place:** [Physical location visibility, third-party distribution apps, website checkout ease, or retail placement]
*   **Promotion:** [Hyper-local ad ideas, seasonal discounts, appetizing image styling strategies, or community events]
## 4. Tactical Action Plan*   [Step-by-step checklist matching the mix variables]

## Framework 4: SOSTAC

# Marketing Strategy for [Business Name]: SOSTAC Plan
## 1. Executive SummaryHigh-level overview of where the business is now, where it needs to go, and how to get there.
## 2. Strategy Timeline Flow```mermaid
gantt
    title SOSTAC Roadmap
    dateFormat  YYYY-MM-DD
    section Phase 1
    Situation Analysis & Objectives    :active, des1, 2026-07-01, 7d
    section Phase 2
    Strategy & Tactics Implementation :        des2, 2026-07-08, 14d
    section Phase 3
    Action Execution & Control Review :        des3, 2026-07-22, 7d
```
## 3. Detailed Framework Breakdown*   **Situation:** Where is the business currently positioned relative to local market rivals?*   **Objectives:** SMART goals based on the user's input goals.*   **Strategy:** The overarching creative route chosen to achieve these goals.*   **Tactics:** The specific marketing toolset items chosen (e.g., SEO, sampling).*   **Action:** Operational steps regarding who does what, and when.*   **Control:** Simple metrics the owner can check to evaluate success weekly.
## 4. Tactical Action Plan*   [Step-by-step launch schedule]

## Framework 5: RACE Planning

# Marketing Strategy for [Business Name]: RACE Framework
## 1. Executive SummaryA digital marketing framework designed to build customer acquisition and loyalty.
## 2. Digital Marketing Funnel```mermaid
graph TD
    Reach[Reach: Attract Food Traffic & Web Clicks] --> Act[Act: Encourage Menu Browsing / Email Signups]
    Act --> Convert[Convert: Secure the First Order / Purchase]
    Convert --> Engage[Engage: Build Repeat Customer Loyalty]
```
## 3. Detailed Framework Breakdown*   **Reach:** [Methods to get discovered online via Search, Instagram Reels, Maps, or Influencer tags]
*   **Act:** [Ways to get prospects to view menu pages, download a voucher, or visit a landing page]
*   **Convert:** [Conversion tricks like simple online checkouts, limited-time welcome offers, or visible reviews]
*   **Engage:** [Retention loops like email newsletter receipts, birthday offers, or social media loyalty clubs]
## 4. Tactical Action Plan*   [Funnel optimization checklist]

## Framework 6: AARRR (Pirate Metrics)

# Marketing Strategy for [Business Name]: AARRR Growth Framework
## 1. Executive SummaryA lean growth-hacking strategy prioritizing fast customer acquisition and viral loops.
## 2. Growth Engine Mechanics```mermaid
stateDiagram-v2
    Acquisition --> Activation
    Activation --> Retention
    Retention --> Referral
    Retention --> Revenue
    Referral --> Acquisition
```
## 3. Detailed Framework Breakdown*   **Acquisition:** [How prospects find the food brand initially via lowest-cost distribution loops]
*   **Activation:** [The immediate "Aha!" moment when the user tastes the signature item or experiences the fast service]
*   **Retention:** [Strategies to keep them ordering weekly instead of checking out other competitors]
*   **Referral:** [Viral food mechanics like "Bring a friend for a free drink" or user-generated food photography tags]
*   **Revenue:** [Methods to upsell sides, appetizers, premium modifications, or subscription meal bundles]
## 4. Tactical Action Plan*   [Growth experimentation matrix]

------------------------------
## 5. System Best Practices for Non-Marketers

* Contextual Explanation Headers: Always include a 1-sentence plain-English subtitle underneath standard marketing jargon headers. For example: ## Product should append a sub-caption reading "What you sell and how it is packaged to look appetizing."
* The "Cheese Pull" Rule: Instruct your base prompt generation system to explicitly ban generic output phrases like "Post consistently on social media." The system must force Gemini to offer descriptive sensory equivalents such as "Post high-definition macro videos showing the texture, steam, or liquid consistency of the product during local lunch hours."
* Action-First Formatting: Every single marketing point must lead with an active, functional verb (e.g., "Run...", "Build...", "Redesign...", "Print..."). This forces the AI to output tasks that read like an actionable to-do checklist rather than a theoretical textbook lecture.

Would you like to build out a custom error-handling framework prompt to check inputs before they hit Phase 2? Or would you prefer to review concrete code implementations for rendering these specific Mermaid diagrams inside your application front-end UI?

[1] [https://www.cliffsnotes.com](https://www.cliffsnotes.com/tutors-problems/Business-Other/58464603-QSO-340-Module-Two-Case-Scenario-Overview-Before-a-project/)
