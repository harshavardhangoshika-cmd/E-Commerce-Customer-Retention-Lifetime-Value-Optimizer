# 📊 E-Commerce Churn Prediction \& Propensity Pipeline



An end-to-end Machine Learning pipeline utilizing an optimized Random Forest Classifier to predict customer churn propensity. This model shifts the business from a reactive stance to an aggressive, data-driven defense strategy by assigning every customer an individual risk score (0% to 100%) before they walk away.

### 

### 👥 The Business Story \& Context

### 

In e-commerce, customer acquisition costs (CAC) are exponentially higher than retention costs. Relying on simple, lagging indicators—such as looking at who left last month—means the business is always one step too late.



#### The Problem



Our team identified that the existing churn monitoring framework was passive. We needed a system capable of analyzing behavioral patterns in real-time to answer a critical forward-looking question: "Which active customers have the highest mathematical probability of abandoning the platform within the next 30 days?"

#### 

#### The Solution



By rebuilding our data pipeline and training an ensemble Random Forest model, we created a continuous Propensity Engine. Instead of a blunt "Yes/No" flag, the engine grades accounts into actionable risk tiers (Low, Medium, High Risk), allowing the customer success and marketing teams to prioritize high-value VIP cohorts and distribute retention budget efficiently.

### 

### 📈 Key Findings \& Executive Metrics



The model was rigorously validated against production test splits, yielding world-class performance metrics:

#### 

#### Model Precision: 98.26% 🎯



What this means for the business: Out of every 100 customers the model flags as a churn risk, more than 98 of them actually leave. False alarms are virtually non-existent. This guarantees that retention budgets (vouchers, discounts, loyalty offers) are never wasted on safe, stable customers.



#### Model ROC-AUC Score: Excellent Differentiation 📈



The model demonstrates near-perfect statistical separation between active buyers and fading accounts, allowing for granular adjustments to our intervention triggers.



#### Top Churn Drivers



Recency / Inactivity Window: The number of days elapsed since the last checkout remains the absolute heaviest statistical anchor.



Purchase Frequency Decay: A sudden drop-off in standard weekly/monthly transaction volume compared to historical baselines.



Customer Support Ticket Volume: Spikes in unresolved complaints serve as the primary reactive trigger for immediate churn.



### ⚙️ Technical Architecture \& Pipeline



The system processes data from raw transactional layers to clean executive outputs across four structured phases:



Phase 1: Ingestion \& Data Extraction: Extracts multi-source relational data (customer profiles, transaction history, and support tickets) from production databases.



Phase 2: Feature Engineering \& Preprocessing: Handles missing values, encodes categorical features, and constructs behavioral baseline metrics like rolling purchase decay and recency windows.



Phase 3: Model Inference \& Scoring: Passes the preprocessed vectors through the optimized Random Forest Classifier to output continuous churn probability scores.



Phase 4: Actionable Orchestration \& Triage: Segregates scores into operational risk tiers (Low, Medium, High) and exports the data to automated marketing tools and customer success dashboards.

