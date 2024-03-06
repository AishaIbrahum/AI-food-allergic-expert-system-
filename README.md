# AI-food-allergic-expert-system-
## Introduction
### Problem Description:
Food allergies are a prevalent health issue affecting a significant portion of the global population. Allergic reactions to specific foods can range from mild to severe, and in extreme cases, they can be life-threatening. Individuals with food allergies must exercise constant vigilance to avoid consuming products that contain allergens, as even trace amounts can trigger an adverse reaction.
Identifying allergens in food items can be a complex task. Food labels often list allergens by their technical names, which may not be easily recognizable to consumers. Additionally, cross-contamination during food processing and handling can introduce allergens into products that are not inherently allergenic. This poses a significant challenge for individuals with food allergies, as they must rely on accurate and comprehensive information to make informed decisions about the foods they consume.

### Necessity of Developing an Expert System:
### The Importance of an Expert System for Food Allergy Management

### The development of an expert system to address food allergies is of paramount importance for several compelling reasons:


#### Rising Prevalence of Food Allergies: 
The prevalence of food allergies has been steadily increasing, making it a significant public health concern. An expert system can serve as a valuable tool for individuals to navigate the complexities of food labeling and make informed dietary choices.

#### Diverse Food Market:
The food market is characterized by a vast array of products, with new items being introduced regularly. An expert system can provide consumers with rapid and accurate assessments of product safety based on their allergen profiles.

#### Complex Allergen Information:
Allergen information can be intricate, with allergens often listed by their technical names or hidden within ingredient lists. An expert system can simplify this process by providing a user-friendly interface that allows users to input their allergies and receive clear feedback on the safety of specific products.

#### Cross-Contamination Concerns:
Cross-contamination during food processing and handling is a common issue that can pose significant risks to individuals with food allergies. An expert system can take into account not only the listed ingredients but also potential cross-contamination risks, offering a more comprehensive assessment of product safety.

#### Emergency Preparedness: 
For individuals with severe allergies, consuming an allergen can trigger life-threatening reactions. An expert system can contribute to emergency preparedness by aiding users in making informed choices and reducing the risk of accidental exposure.

#### Continuous Updates:
The food industry is constantly evolving, with new products and formulations being introduced regularly. An expert system can be designed to stay updated with the latest information, ensuring that users have access to accurate and current allergen data.

#### Empowerment of Individuals: 
An expert system empowers individuals with food allergies to take control of their dietary decisions. It provides a tool for self-management, fostering independence and confidence in making safe food choices.

By leveraging an expert system, individuals with food allergies can navigate the complexities of food labeling, make informed dietary choices, and reduce the risk of adverse reactions. This technology has the potential to significantly improve the quality of life for those affected by food allergies.

## Knowledge Sources:
## The allergen information used in the knowledge base is based on general knowledge about common food allergens. However, specific details about allergens in food can be found in various authoritative sources, including:

1-US Food and Drug Administration (FDA): The FDA provides information on food allergens, labeling requirements, and resources for consumers. You can visit the FDA's Food Allergens page for more details: [https://www.fda.gov/food/food-ingredients-packaging/food-allergens]

2- European Food Safety Authority (EFSA): EFSA also provides information on allergens and intolerances. You can explore their website for scientific opinions and resources: [https://www.efsa.europa.eu/en/topics/topic/allergens]

3- World Health Organization (WHO): The WHO may provide global perspectives on food allergens. Visit their website for relevant information: [https://www.who.int/health-topics/food-allergies#tab=tab_1]

4- National Institute of Allergy and Infectious Diseases (NIAID): NIAID, part of the National Institutes of Health (NIH), provides information on food allergies and research. You can explore their resources here: [https://www.niaid.nih.gov/diseases-conditions/food-allergy]

## Facts
##### Many food recipes share common basic ingredients. However, these ingredients may trigger allergies for individuals sensitive to specific components. For instance, chocolate cake often contains eggs, milk, and gluten, which are common allergens. Therefore, it is crucial to provide a comprehensive database about food allergies to help individuals easily understand food components and identify potential allergens.Such a database would empower individuals with food allergies to make informed dietary choices. It would provide clear and concise information about common allergens and their presence in various food items. This would enable individuals to quickly and easily identify foods that are safe for them to consume and avoid those that may trigger allergic reactions.The database should be user-friendly and accessible to all. It should include a wide range of food items and provide detailed information about their ingredients and potential allergens. Regularly updating the database with the latest information is also essential to ensure its accuracy and reliability.By providing a comprehensive food allergy database, we can empower individuals with food allergies to take control of their dietary choices and live healthier, safer lives.

## Rules:
##### 1: A rule to verify whether the product contains a specified component representing an allergen.
##### 2:A rule to check if the product is safe, meaning it does not contain any of the specified allergenic components. Also make ensure that none of the allergens are present in the product.

## Test Code:
- has_allergen(chocolate_cake, eggs) ? .
- % Test cases
- is_safe(chocolate_cake, [eggs, milk, gluten]) ?.
- % Output should be false, as chocolate cake contains eggs.
- is_safe(peanut_butter_cookies, [peanuts, gluten]) ?.
- % Output should be false, as peanut butter cookies contain peanuts.
- is_safe(seafood_pasta, [seafood, gluten]) ?.
- % Output should be false, as seafood pasta contains seafood.
- is_safe(cheese_pizza, [dairy, gluten]) ?.
- % Output should be false, as cheese pizza contains dairy.
- is_safe(veggie_wrap, [soy, gluten]) ?.
- % Output should be false, as veggie wrap contains soy.
- is_safe(ice_cream, [milk, nuts]) ?.
- % Output should be false, as ice cream contains milk and nuts.
- % Test cases that should be true
- is_safe(fruit_salad, [])?.
- % Output should be true, as fruit salad is safe for someone with no specified allergens.
- is_safe(chocolate_cake, [peanuts, dairy]) ?.
- % Output should be true, as chocolate cake does not contain peanuts or dairy.
- is_safe(veggie_wrap, [nuts]) ?.
- % Output should be true, as veggie wrap does not contain nuts.
- is_safe(seafood_pasta, [])?.
- % Output should be true, as seafood pasta is safe for someone with no specified allergens.
## Result :
<img src="https://github.com/AishaIbrahum/Advanced-Database-Design-and-Implementation-of-a-Blood-Bank-Management-System/assets/143902740/0ff95d1a-bf94-49d9-98a7-974746d781b8" width = "400" alt="Image description">

