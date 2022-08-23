# Constructiveness of Amazon PC Product Reviews
*Author: Yifei Yin, Siqi Wu, Eddie Guo*

Both buyers and sellers on Amazon rely on reviews to align their expectations with the actual product. Customers rely on Amazon reviews to get detailed information about the product, while sellers use reviews to collect feedback on their products and make adjustments. In this project, we are only interested in annotating the degree of constructiveness of Amazon PC product reviews from the sellers’ perspective. A constructive review is clear and factual, aiming at helping the seller/manufacturer to achieve a better outcome. It should also be detailed, specific, and honest, recognizing the pros and cons of product design and functionality and pinpointing areas for potential improvements. A non-constructive review could be opinionated without supporting evidence, lacking insights for the seller/manufacturer to take responsible actions.

“Constructiveness” is annotated in a spectrum between 0 to 5, with 0 being not constructive at all and 5 being the most constructive. To make “constructiveness” measurable, we have defined it in the following five categories, and a review gets one point by hitting each of the five categories:
- The review comments on the pros and/or cons of the product’s design (e.g.,  size, color, weight, etc.)*
- The review comments on the pros and/or cons of the product’s feature/functionality (e.g., battery life, cell service reception, etc.)
- The review comments on the pros and/or cons of the product’s material/internal/external parts (e.g., CPU, keyboard, display, warranty).
- The review provides details on user experience/scenario that add more information to one or more of the previous three points. The review also discusses the installation process, customer support, and product value. (eg. “The battery drains quickly, especially when it’s cold outside.”, ”you can’t beat for the price”)
- The review provides suggestions for improving/keeping the quality of the product in regards to its design, feature/functionality, or material/internal/external parts (e.g., “my iPhone bends easily, Apple should definitely use more sturdy materials.”) 

One important note is that a review that helps customers make purchase decisions does not necessarily help sellers understand their products better. For example, if a review says, “I own another PC from xx, but this one works better”, a potential customer may find the insights on user experience and the comparison with a substitute helpful, but the review does not help the seller improve the product as it lacks details about specific features. Therefore, to avoid the confusion on “helpfulness” and “constructiveness”, we decided to select reviews that reflect similar levels of helpfulness to customers. Our preliminary plan is to only use reviews that have more than 50% of helpful votes (dividing # helpful votes by # total votes)

Our data source is Amazon Review Data (https://nijianmo.github.io/amazon/index.html)