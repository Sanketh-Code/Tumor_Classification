# Breast Cancer Detection

## Objective
To build a good logistic regression model to predict whether the data provided on a cell is Malignant (M) or Benign (B).

## Dataset
Obtained the dataset from kaggle named, Wisconsin Breast Cancer Dataset.
It has a total of 30 Feautures and 569 entries.

## Features:

1. **id** - Unique ID  
2. **diagnosis** - The Target Feature consisting of labes for Malignant(cancerous) and Benign(non-cancerous).  
3. **radius_mean** - Average distance from center to points on the perimeter (larger radius → larger cell nuclei).  
4. **texture_mean** - Standard deviation of gray-scale values (measures variation in texture).  
5. **perimeter_mean** - Mean size of the nucleus perimeter  
6. **area_mean** - Mean area of the nucleus  
7. **smoothness_mean** - How smooth the edges of the nucleus are (variation in radius lengths).  
8. **compactness_mean** - measures how compact the nucleus shape is. [ (perimeter^2 / area) - 1.0]  
9. **concavity_mean** - Severity of concave (indentation) portions of the nucleus contour.  
10. **concave points_mean** - Number of concave portions in the contour.  
11. **symmetry_mean** - How symetrical the nucleus is  
12. **fractal_dimension_mean** - Measures irregularity or complexity of the contour (higher → more irregular).  
13. **radius_se** - Standard error of the mean radius.  
14. **texture_se** - Standard error of the texture.  
15. **perimeter_se** - Standard error of the perimeter.  
16. **area_se** - Standard error of the area.  
17. **smoothness_se** - Standard error of the smoothness.  
18. **compactness_se** - Standard error of the compactness.  
19. **concavity_se** - Standard error of the concavity.  
20. **concave points_se** - Standard error of concave points.  
21. **symmetry_se** - Standard error of the symmetry.  
22. **fractal_dimension_se** - Standard error of the fractal dimension.  
23. **radius_worst** - Mean of the three largest radius measurements.  
24. **texture_worst** - Mean of the three largest texture values.  
25. **perimeter_worst** - Mean of the three largest perimeter values.  
26. **area_worst** - Mean of the three largest area values  
27. **smoothness_worst** - Mean of the three largest smoothness values.  
28. **compactness_worst** - Mean of the three largest compactness values.  
29. **concavity_worst** - Mean of the three largest concavity values  
30. **concave points_worst** - Mean of the three largest concave points values.  
31. **symmetry_worst** - Mean of the three largest symmetry values.  
32. **fractal_dimension_worst** - Mean of the three largest fractal dimension values.

## Relevance of different features.

1. **Radius**: Malignant cells usually have englarged nucli. Larger radius -> high cancer risk
2. **Perimeter**: Malignant cells have uneven edges. increase in the perimeter might indicate that the cells might be cancerous.
3. **area**: Total pixel area of the nucleus. Malignant cells have larger areas.
4. **smoothness**: Measures how smooth or jagged the boundary is. Malignant cells have irregular bumpy edges due to disorganized growth. Low smoothness -> more likely to be malignant.
5. **Concavity**: Captures indentation or flods along the nucleus edge. Malignant cells have deep indentations caused by uncontrolled structural deformation. High concavity high indicate high chances of cell being cancerous.
6. **symmetry**: Measures how evenly shaped the nucleus is. Malignant cells are more unevnen. 

## Pipline overview

1. Data Cleaning
2. Corelation-based Feature Reduction
3. Feature Selection
4. Feature Scaling ( StandardScaler)
5. Model Training (Logistic Regression)
6. Model Evaluation ( Accuracy, Precision, Recall, F1, ROC-AUC)
7. Visualization ( Corelation heatmap, Confusion Matrix)

## Results
- Accuracy: 98.8%
- Precision: 98.4%
- Recall: 98.4%
- ROC-AUC: 0.997
