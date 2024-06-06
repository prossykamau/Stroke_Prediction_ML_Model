{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "18069018-f8c1-4ad8-b85f-dc5b731c1c16",
   "metadata": {},
   "source": [
    " ### **Stroke Prediction Model**"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "f2b5ff64-73c4-4f63-8acf-a8aed34e002e",
   "metadata": {},
   "source": [
    "**Overview**\n",
    "\n",
    "This repository contains a machine learning project aimed at predicting the likelihood of stroke occurrence based on various health parameters. By analyzing a comprehensive dataset with features like age, hypertension, heart disease, glucose levels, BMI, gender, marital status, work type, residence type, and smoking status, this project seeks to build robust classification models to accurately predict stroke risk."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "c219cc0b-3378-40e6-b6d0-d71ffb517282",
   "metadata": {},
   "source": [
    "**Business and Data Understanding**\n",
    "\n",
    "**Stakeholder Audience**\n",
    "\n",
    "The primary stakeholders for this project include healthcare providers, researchers, and public health officials. The goal is to equip them with a predictive tool that can help in early identification of individuals at high risk of stroke, allowing for timely intervention and better resource allocation."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "393c538e-02ef-4b6d-8b20-f8a9e4fd4a6f",
   "metadata": {},
   "source": [
    "**Dataset Choice**\n",
    "\n",
    "The dataset used in this project comprises anonymized health records with various features related to stroke risk factors. It is chosen for its comprehensiveness and relevance to the problem at hand, providing a solid foundation for building accurate predictive models."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "b1778049-af2b-4c77-b23c-4a680e91bc97",
   "metadata": {},
   "source": [
    "**Modeling**\n",
    "\n",
    "The project employs several classification algorithms to predict stroke risk. These models are trained and evaluated using a pipeline that includes data preprocessing steps such as scaling numeric features and one-hot encoding categorical features. The models explored include K-Nearest Neighbors (KNN) with hyperparameter tuning to optimize performance,RandomForestClassifier,DecisionTreeClassifier, LogisticRegression and GradientBoostingClassifier."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "ae7c366a-a12f-46dc-be01-e182f214854f",
   "metadata": {},
   "source": [
    "**Evaluation**\n",
    "\n",
    "The performance of the models is evaluated using metrics such as precision, recall, f1-score, and accuracy. The results indicate high accuracy in predicting non-stroke cases but highlight challenges in accurately predicting stroke occurrences due to class imbalance."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "9dcf22cc-560a-4b53-97c4-336a81c40c41",
   "metadata": {},
   "source": [
    "**Conclusion**\n",
    "\n",
    "The developed models show promising results in predicting stroke risk, particularly for non-stroke cases. However, further work is needed to improve prediction accuracy for stroke cases, potentially through techniques like class balancing, feature engineering, and exploring more complex algorithms."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "8ad756e0-6e4a-40c0-876a-8c48836f74a6",
   "metadata": {},
   "source": [
    "**Getting Started**\n",
    "\n",
    "**Prerequisites**\n",
    "\n",
    "    Python 3.6 \n",
    "    Anaconda \n",
    "    Jupyter\n",
    "    Git Bash"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "ea4ecae4-310a-4712-b379-37af22ddf0d5",
   "metadata": {},
   "source": [
    "**Installation**\n",
    "\n",
    "   1. **Clone the repository**"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "b3a46b18-9131-4dd8-a516-07c920781f0c",
   "metadata": {},
   "source": [
    "git clone https://github.com/prossykamau/Stroke-Prediction-Model\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "16ab296f-7bf3-46be-952a-3284a3e1aa75",
   "metadata": {},
   "source": [
    "2. **Navigate to the project directory:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "fc767ccc-e2bd-4282-a523-f1a420da93bb",
   "metadata": {},
   "outputs": [],
   "source": [
    "cd stroke-prediction-model\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "835504ba-acb6-4f37-a45c-0e248bbd17fc",
   "metadata": {},
   "source": [
    "3. **Create and activate a virtual environment:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "a7fbdc16-d592-4f95-b762-d04265588687",
   "metadata": {},
   "outputs": [],
   "source": [
    "python -m venv env\n",
    "source env/bin/activate  # On Windows use `env\\Scripts\\activate`\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a30d1cb2-d6cb-4188-a792-b71bea022c2a",
   "metadata": {},
   "source": [
    "4. **Install the required packages:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "0f84e5b1-32f8-4c6d-a3ae-dbe67826dbeb",
   "metadata": {},
   "outputs": [],
   "source": [
    "pip install -r requirements.txt\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "82ffab3a-473f-4e7a-b0bb-f10bd21a31fd",
   "metadata": {},
   "source": [
    "**Usage**"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "777e3941-1700-47b1-8b9e-faf0f8c15123",
   "metadata": {},
   "source": [
    "1. **Run the Jupyter Notebook:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "d700aa84-1f29-4d19-bd52-2608d06638d3",
   "metadata": {},
   "outputs": [],
   "source": [
    "jupyter notebook\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "1ee32893-34e2-47ce-be00-326475dce1f6",
   "metadata": {},
   "source": [
    "2. **Open the stroke_prediction.ipynb notebook and follow the steps to preprocess data, train models, and evaluate performance.**"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "b223259b-5440-433b-9a24-52f51c287cc2",
   "metadata": {},
   "source": [
    "**Help**"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "fe2dd31c-04d6-4aeb-b6d0-d72986efcbe0",
   "metadata": {},
   "source": [
    "If you encounter any issues or have questions, feel free to  reach out via email at prossykamau@gmail.com."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "1315332e-5768-48d3-8f8d-48e8598a00b0",
   "metadata": {},
   "source": [
    "**Maintainers**"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "3dff7213-6da2-462b-9766-95b3c7336a2e",
   "metadata": {},
   "source": [
    "Prossy Nansubuga Kamau"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "5c0b54bf-500a-48f4-a810-a75037a7a660",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.11.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
