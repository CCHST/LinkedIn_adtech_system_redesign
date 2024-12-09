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
     - **Comment**: Measures the number of comments, reflecting the interest and engagement generated by the post. More comments indicate active discussions.
     - **Reaction**: Tracks likes, applause, and similar actions, representing the resonance and interest your content generates among readers.
     - **Follower**: Indicates LinkedIn user influence and recognition. Higher follower counts can boost brand exposure and improve market visibility.  
   - **Scoring Method**:  
     Calculate the average score across the three metrics (**comment**, **reaction**, **follower**) for each keyword and normalize the scores to eliminate magnitude differences.

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
