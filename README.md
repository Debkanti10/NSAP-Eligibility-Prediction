# 🛡️ NSAP Scheme Eligibility Prediction using IBM Watson AutoAI

This project uses **IBM Watson Studio and AutoAI** to predict the most appropriate scheme under the **National Social Assistance Programme (NSAP)** for applicants based on district-wise demographic and socio-economic data.

## 📌 Problem Statement

The NSAP aims to provide financial support to the elderly, widows, and persons with disabilities in Below Poverty Line (BPL) households.  
Manual verification of applications often leads to delays and inaccuracies.  
This project builds a **multi-class classification model** to automatically assign the right NSAP scheme (`IGNOAPS`, `IGNWPS`, or `IGNDPS`) to each applicant or region.

## 🧠 Tools & Technologies Used

- **IBM Cloud Lite**
- **IBM Watson Studio**
- **IBM AutoAI** (No-code ML model builder)
- **IBM Watson Machine Learning** (for deployment)
- **CSV Dataset** from AI Kosh

## 🧾 Dataset Description

Source: [AI Kosh – NSAP Dataset](https://aikosh.indiaai.gov.in/web/datasets/details/district_wise_pension_data_under_the_national_social_assistance_programme_nsap_1.html)

Key Features:
- `totalbeneficiaries`
- `totalmale`, `totalfemale`, `totaltransgender`
- `totalaadhaar`, `totalmobile`
- Caste: `totalsc`, `totalst`, `totalobc`, `totalgen`
- `districtname`, `statename`
- **Target Column**: `schemecode` (used for classification)


## ⚙️ Project Workflow

1. Imported dataset into **IBM Watson Studio**
2. Configured **AutoAI experiment**, selected `schemecode` as prediction column
3. AutoAI automatically:
   - Preprocessed the data
   - Trained and evaluated multiple ML models
   - Selected the best-performing classification model
4. Deployed the model using **Watson Machine Learning**
5. Tested predictions on **Jammu & Kashmir** and **Bihar** data

---

## ✅ Results

- Model correctly predicted NSAP schemes for **Pulwama**, **Srinagar**, **Samba**, and **Patna**, **Gaya**, **Bhagalpur**
- Achieved **100% confidence scores** in AutoAI output
- Visualized prediction confidence and class distribution


## 🖼️ Screenshots

- 📊 AutoAI Pipeline  
- 📈 Model Leaderboard  
- ✅ Prediction Results 

## 🔮 Future Scope

- Incorporate real-time applicant data
- Expand to include age, income, education level, etc.
- Build a web or mobile portal for citizen access
- Periodically retrain the model for accuracy improvement


## 🧑‍💻 Author

**Deb Kanti Pal**  

## 📜 License

This project is open-source for educational use. Attribution appreciated if reused.

