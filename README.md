# Ring Landing Page A/B Testing

This project contains an A/B testing experiment for the Ring landing page, aiming to optimize the product browsing experience and increase purchase conversion rates.

## Motivation

A behavioral audit of the current Ring website revealed several potential areas for improvement:

1. **Choice Overload**: The "Shop All" page presents an extensive array of product options, which could overwhelm users and lead to decision paralysis.
2. **Lack of Prioritization**: It's unclear what criteria determine the featured "Best Sellers" products, missing an opportunity to guide customers.
3. **Hidden Pricing**: Prices are not disclosed on the main product grid, creating friction and obscuring a key decision factor.
4. **Absence of Social Proof**: The page lacks customer ratings, reviews, or popularity signals that could build trust and guide purchases.

## Hypothesis

Redesigning the Ring "Shop All" page to reduce choice overload, highlight recommended products, show prices upfront, and incorporate social proof will increase product exploration and purchase conversion compared to the current design.

## Test Setup

- **Target Population**: All U.S. visitors to the Ring.com "Shop All" page on desktop and mobile web.
- **Sample Size**: 776,000 unique users split evenly between control and treatment groups, providing 80% power and 95% significance for detecting a minimum 10% effect with a 5% baseline conversion rate.
- **Control (A)**: Current "Shop All" design with all products shown in a grid without prices or reviews.
- **Treatment (B)**: Alternate "Shop All" design with the following changes:
 - Collapsed product category sections showing a curated set of 5 "Editor's Picks" per category.
 - "Best Sellers" section expanded to a full row showing the top 10 products with price and star rating under each.
 - "Top Deals" row added to highlight 5-10 best discounted products with savings shown as "X% off".
 - Average rating and total reviews displayed under each product in the main grid.

## Metrics

- **Primary Success Metric**: Purchase conversion rate (orders/unique visitors).
- **Secondary Metrics**: Click-through rate from Shop All to product pages, average order value, engagement with "Best Sellers" and "Deals" sections, product-specific conversion rates, performance segmented by new vs. returning users.

## Analysis

- Two-sample proportion t-test to compare conversion rates between control and treatment with an alpha of 0.05.
- Analyze lift in secondary metrics and segment performance.

## Limitations and Future Opportunities

This test focuses heavily on optimizing the initial product browsing experience but does not address potential pain points or drop-offs further down the purchase funnel, which could cap the overall revenue impact. A full-funnel analysis and testing roadmap should be developed.

Additionally, the current test leans into pricing and popularity as key decision levers. Future experiments could explore the impact of other choice architectures and information designs, such as:

- Guided selling based on user needs or intent.
- Elevated educational content and product comparison tools.
- Personalized recommendations and recently viewed modules.
- Urgency triggers like low-stock or sale countdown timers.
- Shipping cost and speed promises.

## References to Behavioral Principles

- **Choice architecture**: Structuring the presentation of options to influence decisions via defaults, sorting, filtering, and grouping. Here, we collapse and curate the choices to reduce overload.
- **Information architecture**: Designing the display of information to make key details salient and easy to process. Adding prices and ratings on the main page applies this.
- **Social proof**: Leveraging the influence of the crowd to guide individual decisions. Expanding the Best Sellers section and adding reviews taps into this principle.
- **Dual process theory**: Designing for both the deliberative System 2 thought process and the intuitive System 1 process. Clear categories aid deliberative comparisons, while Best Sellers and Deal tags provide System 1 shortcuts.
