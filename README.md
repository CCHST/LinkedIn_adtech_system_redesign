# LinkedIn AdTech System Redesign

---

## Objective
Redefine user targeting as a Demand-Side Platform (DSP) through Natural Language Processing (NLP) to provide advertising strategies and audience recommendations for companies across industries.

---

## Background
Advertisers can directly set demographic conditions for their target audience, but such conditions often do not accurately reflect advertiser needs. Additionally, these rigid criteria can lead to audience loss.

---

## Methodology
Develop a **Lookalike Model** to analyze the behavior of the existing target audience and identify potential customers with similar characteristics for more precise advertising.

---

## Workflow

1. **Keyword Analysis**  
   Perform tokenization, stop-word filtering, part-of-speech normalization, and assign scores to keywords to identify influential terms.
   - **Key Metrics for Scoring**:
     - **Post Frequency**: Reflects how often a user posts content within a specified timeframe, indicating their activity level.
     - **Average Reaction Ratio**: Represents the average number of reactions (e.g., likes) a user receives per follower, measuring audience engagement with their posts.
     - **Average Comment Ratio**: Captures the average number of comments a user receives per follower, reflecting the depth of interaction their content generates.  
   - **Scoring Method**:  
     Calculate the average score across the three metrics (**Post Frequency**, **Average Reaction Ratio**, **Average Comment Ratio**) for each keyword and normalize the scores to eliminate magnitude differences. These metrics are designed to capture different aspects of user activity and engagement.

2. **Clustering**  
   Group keywords with similar scores to identify lookalike audiences.
   - **Clustering Methods**: K-means and Hierarchical Clustering.

3. **Cosine Similarity**  
   Match clustered keywords against custom criteria such as industry, interests, and behavioral traits for more precise audience targeting.

---

## Conclusion

### Pre-Advertising:  
Use the Lookalike Model to support audience selection, product design, and overall brand strategy.  
- **Enhanced Audience Insights**: Better understand the existing audience and expand to potential customers with similar characteristics, increasing advertising accuracy, effectiveness, and ROI.
- **Expanded Customer Base**: Identify and target potential customers by analyzing the features and behaviors of the existing audience.  
- **Improved Precision**: Minimize ad waste and increase conversion rates by targeting audiences with similar traits.

### Post-Advertising:  
Leverage LinkedIn’s segmentation model to refine market strategies, utilizing variables such as location, age, gender, and interests to better understand and address audience needs.
