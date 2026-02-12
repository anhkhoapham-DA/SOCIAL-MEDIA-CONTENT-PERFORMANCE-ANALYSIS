# Social Media Marketing Performance Analysis

## 1. Background
Our business is currently looking to evaluate the effectiveness of our marketing efforts, specifically focusing on social media content. The primary goal is to assess the current marketing situation based on historical performance data and identify strategic directions to improve engagement and reach. By understanding which content resonates best with our audience, we aim to optimize our future content strategy.

## 2. Objectives
The main objective of this project is to leverage **Python** for in-depth data analysis and visualization to uncover actionable insights that will support our social media marketing strategy.

Key analysis focuses include:
* Evaluating performance metrics across different **Content Categories**.
* Analyzing the impact of various **Post Types** (e.g., images, videos, carousels) on user engagement.
* Identifying trends and patterns to provide data-driven recommendations for future content creation.

## 3. Workflow
The project follows a structured data analysis pipeline involving Excel, SQL, and Python:

### Step 1: Initial Data Cleaning (Excel)
* Performed a preliminary review of the raw dataset.
* Standardized formats and removed obvious duplicates or irrelevant columns to prepare the data for database ingestion.

### Step 2: Data Processing & Querying (SQL)
* **Handling Missing Values:** Executed SQL queries to identify and impute or filter out null values to ensure data integrity.
* **KPI Extraction:** Wrote complex queries to calculate essential Key Performance Indicators (KPIs) such as Total Reach, Engagement Rate, and Conversion Rate per post.

### Step 3: Advanced Analysis & Visualization (Python)
* **Statistical Analysis:**
    * Performed **T-tests** and **ANOVA** to determine the statistical significance of differences in engagement between various content categories and post types.
* **Visualization:**
    * Created **Heatmaps** to visualize correlations between variables (e.g., time of posting vs. engagement).
    * Generated **Scatter Charts** to observe the relationship between reach and engagement metrics.
* **Insight Generation:** Synthesized findings to draw conclusions on the most effective content strategies.

## Technologies Used
* **Microsoft Excel:** Data inspection and initial cleaning.
* **SQL:** Data manipulation, missing value treatment, and KPI calculation.
* **Python:**
    * *Pandas* for data manipulation.
    * *SciPy* for statistical testing (T-test, ANOVA).
    * *Matplotlib / Seaborn* for data visualization (Heatmaps, Scatter plots).

## 4. Insights

### 1. Correlation Analysis

<img width="857" height="690" alt="image" src="https://github.com/user-attachments/assets/ad52173f-1133-4345-b86e-38449e4e580c" />

### 💡 Insight: Volume Metrics vs. Engagement Efficiency
- **Finding:** **'Views'** and **'Impressions'** exhibit a perfect positive correlation (**1.00**), driving strong absolute numbers for **'Likes' (0.94)** and **'Shares' (0.94)**. However, **'Engagement Rate'** is negatively correlated across the board (e.g., **-0.32** with Views), suggesting that as reach scales, the percentage of active interaction per user naturally declines.
- **Action:** Since **'Clicks'** and **'Comments'** share a strong correlation (**0.87**), prioritize content that sparks discussion to effectively drive downstream traffic.Establish separate performance benchmarks for **"Mass Awareness"** (High Views, Lower Rate) vs. **"Community Nurturing"** (Lower Views, High Rate) content to evaluate success accurately.

### 2. Platform Performance Analysis

<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/c7c5d15e-4892-4874-a263-bb494faeeec3" />

- **Top Performer:** **Instagram** leads with an average Engagement Rate of ~15,8%
- **Action:** Boost content on Instagram.

### 3. Content Category Analysis

<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/5afd4f5d-1de5-4226-a018-df06b569453c" />

### 💡 Insight: Content That Resonates
- **Insights:** Content categorized as **'Educational' and 'Customer Story'** consistently yields the highest median engagement rates (~20%). This indicates a strong user preference for value-driven content over purely promotional material.
- **Strategy:** Shift focus from purely entertaining content to value-driven educational posts and customer success stories.

### 4. Post Type Analysis

<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/8a982b82-cf8c-4faf-97ee-6b46e152f232" />

### 💡 Insight: The 'Image' Surprise
- **Crucial Finding:** Contrary to industry trends, **Static Images** significantly outperform Video content in this dataset (**17.95% vs. 14.41%**).
- **Statistical Proof:** T-test p-value $\approx 0$, confirming this is a robust pattern.
- **Recommendation:** Invest in high-quality graphic design (infographics, carousels) as a cost-effective alternative to video production.

### 5. Organic vs. Sponsored Content

<img width="700" height="548" alt="image" src="https://github.com/user-attachments/assets/17f768c9-d17a-4e0d-bd23-2994a667cc22" />

### 💡 Insight: Paid vs. Organic Reach
- **Finding:** There is **no statistically significant difference** ($p > 0.05$) in Engagement Rate between Organic and Sponsored content.
- **Implication:** While paid ads increase reach, they do not inherently improve interaction quality. Content relevance remains key.

### 6. Hashtag Optimization

<img width="990" height="590" alt="image" src="https://github.com/user-attachments/assets/476ddf47-26ab-4b80-8b53-fe03511d2b7c" />

### 💡 Insight: Niche Tags Win
- **Top Performers:** Specific tags like `#Testimonial` and `#SuccessStory` yield the highest engagement (~20%+).
- **Tactic:** Avoid over-saturated generic tags; target specific communities with niche hashtags.

### 7. Interaction Analysis: Region vs. Content Category
This section examines the variations in engagement levels across different content categories within specific geographic markets to identify regional user preferences.

<img width="1089" height="590" alt="image" src="https://github.com/user-attachments/assets/1bba2eda-ebca-417f-a995-5f4b602df7a7" />


### 💡 Insight: Educational Content Dominates Emerging Markets
- **Finding:** The strategy is highly standardized, with **'Customer Story'** and **'Educational'** content consistently leading at **~20%** across all regions. However, **India and Brazil** show a distinct preference for **'Event/Webinar'** content **(14.3%)**, while **Australia** leads the push in **'Product Promotion'** (11.82%).
- **Action:** Prioritize **'Event/Webinar'** budgets for **India and Brazil** to capitalize on their higher-than-average engagement with interactive formats.
Double down on **'Product Promotion'** in **Australia** to leverage the region's higher receptivity to direct sales messaging.
Maintain the **'Customer Story'** dominance in the **UK and Australia (over 20%)** to reinforce social proof in these mature markets where trust-building is critical.

### 8. Tactical Matrix: Content Category vs. Post Type
This analysis identifies which post formats (Video, Image, Carousel, Text) yield the highest efficiency for each specific content theme.

<img width="1100" height="590" alt="image" src="https://github.com/user-attachments/assets/36cc83ca-1692-459e-9adf-a4843b77668c" />

### 💡 Insight: Video for Education, Images for Entertainment
- **Finding:** The **PDF** format paired with **'Educational'** content achieves the highest performance. Also, **'Entertainment' and 'Product Promotion'** content sees engagement spikes when utilizing **PDF** formats.
- **Action:** 
Focus on creating more **PDF** content for **'Educational'** posts to maximize engagement.
Leverage **PDF** format for **'Entertainment'** and **'Product Promotion'** content to boost audience interaction.
Align content strategy by matching content types with their most effective format for higher overall performance.

## Conclusion & Strategic Recommendations
Based on the statistical analysis, the following strategic shifts are recommended:
1. **Content Strategy:**  Focus on "Customer Story" and "Educational" pillars. Rationale: ANOVA results indicate that Customer Story and Educational categories consistently achieve the highest mean Engagement Rates (~20%), significantly outperforming Entertainment. Shifting focus to these categories offers a statistically higher probability of user interaction compared to chasing viral entertainment trends.
2. **Metric-Driven Goals:**  Adopt a Dual-KPI Framework: "Growth" vs. "Engagement". Rationale: The correlation analysis reveals a negative correlation (-0.31) between Views and Engagement Rate. This implies that strategies maximizing reach often dilute engagement density. Therefore, campaigns should have distinct, non-conflicting targets:Objective A (Brand Awareness): Maximize Impressions/Shares (Strong positive correlation: 0.94).Objective B (Community Depth): Maximize Engagement Rate (via Educational/Story content).
3. **Resource Allocation:** Pivot Production Budget from Video to Static/PDF Formats. Rationale: Contrary to the trend of "video-first," our data shows that Static Images and PDFs significantly outperform Videos in Engagement Rate (17.95% vs 14.41%, confirmed by ANOVA). Additionally, T-tests show no significant difference ($p > 0.05$) between Organic and Sponsored content performance.Action: Reallocate budget from expensive video production and paid ads towards high-quality, design-intensive Infographics (Images) and Carousel (PDF) content.





