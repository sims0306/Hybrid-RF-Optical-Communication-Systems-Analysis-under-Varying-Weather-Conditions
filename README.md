# Hybrid-RF-Optical-Communication-Systems-Analysis-under-Varying-Weather-Conditions
**Project Overview**
In today's data-driven world, the demand for faster, more reliable, and efficient communication systems has grown exponentially. Traditional Radio Frequency (RF) communication systems, while widely used, face challenges such as bandwidth limitations and vulnerability to atmospheric conditions. To overcome these, hybrid RF/Optical communication systems have emerged as a promising solution, combining the robustness and wide coverage of RF with the high speed and large bandwidth capabilities of optical links.

This project investigates the impact of varying weather conditions on data transmission quality in both RF and hybrid RF/Optical communication systems. The aim is to develop predictive models that accurately estimate channel attenuation caused by environmental factors, enhancing system reliability and performance.

**Problem Statement**
Both RF and optical communication systems suffer from performance degradation due to environmental factors, especially weather conditions. These variations affect the stability and quality of data transmission, creating a need for robust models that can predict attenuation under different conditions.

**Methodology**
Data Source: Weather and attenuation data with SYNOP codes representing weather conditions.

Models Used: Random Forest Regression.

Three modeling approaches were employed:

Generic Method: A single model applied across the entire dataset.

Specific Method: Separate models built for each SYNOP categorical weather code.

Joint Method: Utilizes outputs from the Generic Method as input features to capture inter-channel dependencies, enhancing prediction accuracy.

**Results**
**RF Attenuation Prediction:**

Generic Method: R² = 0.9716, RMSE = 0.5790

Specific Method: R² = 0.9378, RMSE = 0.6136

Joint Method: R² = 0.9739, RMSE = 0.3088

**FSO Attenuation Prediction:**
Generic Method: R² = 0.9377, RMSE = 0.9737

Specific Method: R² = 0.9501, RMSE = 0.9933

**Joint Method**: R² = 0.9384 (RMSE value to be updated)

The Joint Method showed improved accuracy in RF attenuation prediction by capturing interdependencies between channels.

Significance
This work contributes to the development of more reliable hybrid RF/Optical communication infrastructures that can sustain high-quality data transmission regardless of weather challenges. It highlights the potential of machine learning models, especially ensemble methods like Random Forest, to enhance communication system design and operation.

**How to Use This Repository**
Explore the data preprocessing and feature engineering scripts.

Run the Random Forest models to replicate or extend the study.

Use the evaluation scripts to validate model performance.

Adapt the methodology to other environmental or communication datasets.

**Future Work**
Integration of other machine learning techniques such as Gradient Boosting and Neural Networks.

Expansion of weather condition categories for more granular modeling.

Real-time system implementation and testing.

