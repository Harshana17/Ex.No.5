

# EXP 5: Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios

## Name: HARSHANA M V
## Reg No: 212224240053

# Aim:
To compare different prompting techniques and evaluate their effectiveness in solving real-world engineering problems by using a problem selected from a student's final-year project work. 


# EXPERIMENT OVERVIEW

In this experiment, each student/team selects a genuine problem from their ongoing or completed 3rd-year or final-year engineering project.
The same engineering problem is given to an AI system using different prompting techniques. Students then compare the responses based on relevance, accuracy, completeness, clarity, feasibility and usefulness.
The purpose is not simply to obtain an AI-generated answer. Students must analyse how changing the prompting technique changes the quality of the solution.

##### EXPERIMENT PROCEDURE
Step 1 – Select the Engineering Problem
Choose one genuine problem from the student's 3rd-year or final-year project.

Step 2 – Write the Base Prompt
Write a simple prompt describing the engineering problem without using advanced prompting techniques.

Step 3 – Apply Different Prompting Techniques
Rewrite the same problem using at least four different prompting techniques.
For example:
Technique 1 – Straightforward Prompt
Suggest a method to detect crop diseases using computer vision.structure.

Run Experiments with ChatGPT:
Input the naïve prompt for each scenario and record the generated response.
Then input the corresponding basic prompt and capture that response.
Repeat this process for all selected scenarios to gather a full set of results.

Evaluate Responses : 
	Compare how ChatGPT performs when given naïve versus basic prompts and analyze the output based on Quality,Accuracy and Depth. Also analyse does ChatGPT consistently provide better results with basic prompts? Are there scenarios where naïve prompts work equally well?
Deliverables:

A table comparing ChatGPT's responses to naïve and basic prompts across all scenarios.
Analysis of how prompt clarity impacts the quality, accuracy, and depth of ChatGPT’s outputs.
Summary of findings with insights on how to structure prompts for optimal results when using ChatGPT.

#**STUDENT SUBMISSION FORMAT**
Each student/team should submit:
Project title and problem statement
Selected engineering scenario
Base prompt
Minimum four improved prompts using different techniques
AI-generated outputs
Comparison/evaluation table
Analysis and observations
Final selected prompting technique
Refined/final prompt
Engineering validation

## Project Title:
### A UNIFIED MULTI-CROP DIGITAL TWIN FOR EXPLAINABLE AI-DRIVEN CROP MONITORING AND INTELLIGENT FARM MANAGEMENT

## AI TOOLS REQUIRED
- ChatGPT

## OBJECTIVE
To apply different prompting patterns to the same engineering problem — building a multi-crop digital twin for explainable, AI-driven farm management — and study how the generated outputs differ.

The following prompting patterns are used:

1. Zero-Shot Prompting
2. Few-Shot Prompting
3. Role-Based Prompting
4. Step-by-Step Prompting

---

## 1. PROBLEM STATEMENT

Traditional farm monitoring relies on manual field inspection and generalized irrigation/fertilization schedules that do not account for crop-specific needs, real-time soil conditions, or weather variability. This often leads to over-irrigation, under-fertilization, delayed disease detection, and reduced yield.

The objective is to design a **Unified Multi-Crop Digital Twin** — a virtual, continuously-updated replica of the farm — that:

- Monitors multiple crops simultaneously (e.g., Wheat, Rice, Maize, Cotton).
- Tracks soil moisture, temperature, humidity, and a vegetation health index (NDVI-like).
- Uses AI to classify crop health status.
- Explains *why* a decision was made (Explainable AI), not just *what* the decision is.
- Recommends irrigation, fertilization, or alert actions per crop.
- Continuously updates the digital twin as new sensor data arrives.

---

## 2. PROMPTING PATTERN USED

### Zero-Shot Prompt
> Design an AI-based digital twin system for monitoring multiple crops on a farm.

**Generated Output**
The AI suggests a system that collects soil and weather data and uses AI to monitor crop conditions and suggest irrigation actions.

### Few-Shot Prompt
> Consider the following examples:
> Soil Moisture 65%, Healthy NDVI → "Healthy – No Action"
> Soil Moisture 30%, Low NDVI → "Stressed – Irrigate Immediately"
> Soil Moisture 45%, Medium NDVI → "Moderate – Monitor Closely"
> Now design a multi-crop digital twin that follows the same classification logic for explainable decision-making.

**Generated Output**
The AI creates a system that measures soil moisture and vegetation index and classifies each crop's health into three explainable categories.

### Role-Based Prompt
> Act as an Agricultural AI and Digital Twin engineer. Design a unified digital twin system for multiple crops using soil sensors, weather data, an explainable AI decision module, and a farm management dashboard. Explain the components and working of the system.

**Generated Output**
The AI provides an engineering-oriented solution containing sensors, a digital twin data layer, an explainable AI reasoning module, and a farm-management decision layer.

### Step-by-Step Prompt
> Design a multi-crop digital twin step by step. Explain how sensor data is collected, how each crop's digital twin state is updated, how AI evaluates crop health, how explanations are generated, and how farm management recommendations are issued.

**Generated Output**
The AI produces a structured workflow from data collection to explainable farm-management recommendations.

---

## 3. SYSTEM ARCHITECTURE

<img width="1377" height="232" alt="image" src="https://github.com/user-attachments/assets/bb16d8a2-2d2d-4ded-8682-4f29de4b3516" />

### System Components

| Component | Function |
|---|---|
| Soil & Weather Sensors | Collect soil moisture, temperature, humidity, and vegetation index data |
| Data Ingestion Layer | Cleans and routes incoming sensor data per crop/field |
| Digital Twin State Store | Maintains a live virtual replica of each crop's condition |
| Explainable AI Decision Module | Classifies crop health and generates human-readable reasons |
| Farm Management Dashboard | Displays crop status, trends, and recommendations |
| Alert & Recommendation Engine | Issues irrigation, fertilization, or inspection alerts |

---

## 4. WORKING PRINCIPLE

The unified multi-crop digital twin works through the following stages:

**Step 1 – Data Collection**
Soil moisture, temperature, humidity, and NDVI-like vegetation index values are collected for each crop/field.

**Step 2 – Digital Twin Update**
Each crop's virtual replica (digital twin) is updated with the latest sensor readings.

**Step 3 – Health Classification**
The AI module classifies each crop's condition into Healthy, Moderate Stress, or Critical Stress.

**Step 4 – Explanation Generation**
The system generates a human-readable explanation for the classification (which factors triggered it).

**Step 5 – Recommendation**
The system issues an action recommendation (e.g., irrigate, monitor, inspect for disease).

**Step 6 – Continuous Monitoring**
The digital twin keeps updating as new sensor data streams in, keeping the farm management view current.

---

## 5. CROP HEALTH CLASSIFICATION LOGIC

| Soil Moisture | Vegetation Index (NDVI-like) | Health Status | Recommended Action |
|---|---|---|---|
| Below 35% | Below 0.4 | Critical Stress | Irrigate Immediately |
| 35% – 55% | 0.4 – 0.6 | Moderate Stress | Monitor Closely |
| Above 55% | Above 0.6 | Healthy | No Action Needed |

---

## 6. FLOWCHART

<img width="541" height="587" alt="image" src="https://github.com/user-attachments/assets/564a478e-399d-4518-9e5d-b827f0393c74" />


---

## 7. ALGORITHM

1. Start the program.
2. Read soil moisture, temperature, and vegetation index (NDVI-like) for each crop.
3. If moisture is below 35% or NDVI is below 0.4, classify as **Critical Stress**.
4. Recommend immediate irrigation.
5. Otherwise, if moisture is below 55% or NDVI is below 0.6, classify as **Moderate Stress**.
6. Recommend close monitoring.
7. Otherwise, classify as **Healthy**.
8. No action is recommended.
9. Generate an explanation stating which factor(s) drove the classification.
10. Update the digital twin state for that crop.
11. Display the crop name, health status, explanation, and recommendation.
12. Repeat the process for all crops for continuous monitoring.
13. Stop.

---

## 8. PYTHON PROGRAM

```python
crops = {
    "Wheat":  {"moisture": 60, "temperature": 28, "ndvi": 0.72},
    "Rice":   {"moisture": 32, "temperature": 33, "ndvi": 0.38},
    "Maize":  {"moisture": 48, "temperature": 30, "ndvi": 0.55},
    "Cotton": {"moisture": 70, "temperature": 27, "ndvi": 0.80},
}

def classify_crop(moisture, ndvi):
    reasons = []

    if moisture < 35 or ndvi < 0.4:
        status = "Critical Stress"
        action = "Irrigate Immediately"
        if moisture < 35:
            reasons.append(f"soil moisture is low ({moisture}%)")
        if ndvi < 0.4:
            reasons.append(f"vegetation index is low ({ndvi})")

    elif moisture < 55 or ndvi < 0.6:
        status = "Moderate Stress"
        action = "Monitor Closely"
        if moisture < 55:
            reasons.append(f"soil moisture is moderate ({moisture}%)")
        if ndvi < 0.6:
            reasons.append(f"vegetation index is moderate ({ndvi})")

    else:
        status = "Healthy"
        action = "No Action Needed"
        reasons.append(f"soil moisture ({moisture}%) and vegetation index ({ndvi}) are both within healthy range")

    explanation = "Because " + " and ".join(reasons) + "."
    return status, action, explanation


for crop, data in crops.items():
    status, action, explanation = classify_crop(data["moisture"], data["ndvi"])
    print("Crop:", crop)
    print("Soil Moisture:", data["moisture"], "%")
    print("Temperature:", data["temperature"], "°C")
    print("NDVI:", data["ndvi"])
    print("Health Status:", status)
    print("Explanation:", explanation)
    print("Recommended Action:", action)
    print()
```

---

## 9. PROGRAM EXECUTION

### Sample Output
```
Crop: Wheat
Soil Moisture: 60 %
Temperature: 28 °C
NDVI: 0.72
Health Status: Healthy
Explanation: Because soil moisture (60%) and vegetation index (0.72) are both within healthy range.
Recommended Action: No Action Needed

Crop: Rice
Soil Moisture: 32 %
Temperature: 33 °C
NDVI: 0.38
Health Status: Critical Stress
Explanation: Because soil moisture is low (32%) and vegetation index is low (0.38).
Recommended Action: Irrigate Immediately

Crop: Maize
Soil Moisture: 48 %
Temperature: 30 °C
NDVI: 0.55
Health Status: Moderate Stress
Explanation: Because soil moisture is moderate (48%) and vegetation index is moderate (0.55).
Recommended Action: Monitor Closely

Crop: Cotton
Soil Moisture: 70 %
Temperature: 27 °C
NDVI: 0.8
Health Status: Healthy
Explanation: Because soil moisture (70%) and vegetation index (0.8) are both within healthy range.
Recommended Action: No Action Needed
```

---

## 10. OUTPUT ANALYSIS

**Wheat** — Moisture = 60%, NDVI = 0.72 → both above thresholds → **Healthy**, no action.

**Rice** — Moisture = 32% (< 35%), NDVI = 0.38 (< 0.4) → both critical triggers fire → **Critical Stress**, irrigate immediately.

**Maize** — Moisture = 48% (< 55%), NDVI = 0.55 (< 0.6) → falls in moderate band → **Moderate Stress**, monitor closely.

**Cotton** — Moisture = 70%, NDVI = 0.80 → both above thresholds → **Healthy**, no action.

---

## 11. TESTING

| Test Case | Moisture (%) | NDVI | Expected Status | Result |
|---|---|---|---|---|
| TC01 | 60 | 0.72 | Healthy | PASS |
| TC02 | 32 | 0.38 | Critical Stress | PASS |
| TC03 | 48 | 0.55 | Moderate Stress | PASS |
| TC04 | 20 | 0.30 | Critical Stress | PASS |
| TC05 | 55 | 0.60 | Healthy | PASS |

---

## 12. TEST CASE ANALYSIS

**TC01** — Moisture 60%, NDVI 0.72 → both above upper thresholds → Healthy. **Result: PASS**

**TC02** — Moisture 32%, NDVI 0.38 → both below critical thresholds → Critical Stress. **Result: PASS**

**TC03** — Moisture 48%, NDVI 0.55 → both in moderate band → Moderate Stress. **Result: PASS**

**TC04** — Moisture 20%, NDVI 0.30 → far below critical thresholds → Critical Stress. **Result: PASS**

**TC05** — Moisture 55%, NDVI 0.60 → exactly at healthy boundary → Healthy. **Result: PASS**

---

## 13. COMPARISON OF PROMPTING PATTERNS

| Prompt Pattern | Output Characteristics | Suitable For |
|---|---|---|
| Zero-Shot | General solution | Simple problems |
| Few-Shot | Pattern-based, example-driven solution | Classification tasks |
| Role-Based | Domain-specific, engineering-oriented solution | System design |
| Step-by-Step | Structured, staged solution | Complex, multi-module problems |

---

## 14. COMPARATIVE ANALYSIS

**Zero-Shot Prompting**
Provides a quick and general solution without requiring examples.
- Advantage: Simple and fast.
- Limitation: May lack crop-specific or explainability detail.

**Few-Shot Prompting**
Uses labeled examples to guide the AI toward the expected classification behavior.
- Advantage: Produces consistent, pattern-based results.
- Limitation: Requires well-chosen, representative examples.

**Role-Based Prompting**
Makes the AI respond from the perspective of a digital-twin/agricultural-AI engineer.
- Advantage: Produces domain-oriented, technically grounded explanations.
- Limitation: Assigning a role does not guarantee agronomic correctness.

**Step-by-Step Prompting**
Breaks the digital twin design into logical, sequential stages.
- Advantage: Well suited to multi-module systems like a digital twin.
- Limitation: Output can become longer than necessary.

---

## 15. OVERALL EVALUATION

| Parameter | Zero-Shot | Few-Shot | Role-Based | Step-by-Step |
|---|---|---|---|---|
| Quality | 7/10 | 8/10 | 9/10 | 9/10 |
| Accuracy | 7/10 | 8/10 | 9/10 | 9/10 |
| Relevance | 7/10 | 9/10 | 9/10 | 9/10 |
| Explainability | 6/10 | 8/10 | 9/10 | 10/10 |
| Ease of Use | 10/10 | 8/10 | 8/10 | 7/10 |

---

## 16. PROMPT CHAIN FOR THE MULTI-CROP DIGITAL TWIN

<img width="242" height="502" alt="image" src="https://github.com/user-attachments/assets/f69fc54a-ca8e-4e87-9001-4cf8486054ca" />


---

## 17. FINAL SYSTEM WORKFLOW

<img width="1393" height="182" alt="image" src="https://github.com/user-attachments/assets/8a000c67-1aac-4955-9544-dfcfc56f899a" />

---

## 18. ADVANTAGES OF THE PROPOSED SYSTEM

- Monitors multiple crops simultaneously within a single unified system.
- Provides explainable reasoning behind every AI decision, not just a raw output.
- Reduces over-irrigation and under-fertilization through crop-specific thresholds.
- Enables early detection of crop stress before visible damage occurs.
- Continuously updates the digital twin as new sensor data arrives.
- Can be extended with satellite imagery, drones, and machine-learning models.
- Supports integration with IoT-based smart farming infrastructure.

## 19. LIMITATIONS

- The Python program is a simulation and does not connect to real sensors.
- Real deployment requires calibrated soil, weather, and vegetation-index sensors.
- NDVI-like values in a real system require camera/satellite-based computation.
- Incorrect or noisy sensor data can affect classification accuracy.
- Explanations are rule-based here; a production XAI module may need model-based explanation techniques (e.g., SHAP, LIME).

## 20. FUTURE ENHANCEMENT

The system can be improved by:

- Using real-time satellite or drone-based NDVI imagery.
- Applying machine learning models for yield and stress prediction.
- Integrating IoT soil and weather sensors across fields.
- Adding pest and disease detection using computer vision.
- Generating model-based explanations (SHAP/LIME) instead of rule-based ones.
- Connecting the digital twin to a cloud-based farm management platform.
- Using historical data to forecast irrigation and fertilization needs.

## 21. KEY FINDINGS

- Different prompting patterns produce different styles and depths of AI-generated system designs.
- Zero-shot prompting is suitable for a quick, general first draft.
- Few-shot prompting improves consistency for classification-style logic.
- Role-based prompting produces more domain-accurate, engineering-grade designs.
- Step-by-step prompting is best suited for multi-module systems like a digital twin.
- Prompt chaining allows a complex system (digital twin + XAI + farm management) to be broken into manageable stages.
- Explainability is a key differentiator between a plain classifier and a true digital-twin decision system.
- AI-generated programs and logic should always be tested across multiple crop and condition scenarios before use.

---

## OUTPUT
## CONCLUSION

The Unified Multi-Crop Digital Twin for Explainable AI-Driven Crop Monitoring and Intelligent Farm Management was successfully designed using different prompting patterns and prompt chaining techniques.

Zero-shot, few-shot, role-based, and step-by-step prompting were applied to the same engineering problem. The generated outputs were compared based on quality, accuracy, relevance, and explainability.

The Python simulation successfully classified multiple crops into Healthy, Moderate Stress, and Critical Stress categories, generated human-readable explanations for each decision, and issued corresponding farm-management recommendations.

The experiment demonstrates that prompt engineering and prompt chaining can help students design explainable, multi-component AI systems systematically — from problem identification and requirement analysis through architecture, algorithm, programming, testing, and documentation.

## RESULT

The Unified Multi-Crop Digital Twin was successfully designed and simulated using different prompting patterns. The Python program was executed successfully, all test cases produced the expected results, and each decision was accompanied by a clear, human-readable explanation. The experiment demonstrated that suitable prompting patterns and prompt chaining can improve the quality, structure, and explainability of AI-assisted engineering solutions for intelligent farm management.
 
The prompt for the above said problem executed successfully
