# **Fraud Detection with ETL Pipeline**  

## **Project Description**  
This project develops a **fraud detection system using ETL and Machine Learning** to automatically identify suspicious transactions. Using **Apache Airflow**, this pipeline extracts transaction data from the database, processes it, and then applies a Machine Learning model to detect fraudulent activities. If a suspicious transaction is detected, the system will send an email notification to the relevant team for further investigation.  

## **ETL Process Flow**  
1. **Extract** → Retrieve transaction data from PostgreSQL using Airflow.  
2. **Load** → Store the processed data back into the database.  
3. **Predict** → Use a Machine Learning model to classify transactions as fraud or non-fraud.  
4. **Alert** → If a suspicious transaction is detected, the system sends an email notification to the relevant team.  

## **Technologies Used**  
- **ETL Orchestration**: Apache Airflow  
- **Database**: PostgreSQL  
- **Programming**: Python, Pandas, NumPy  
- **Machine Learning**: Scikit-learn, XGBoost, Random Forest, Isolation Forest  
- **Deployment**: Pickle (model serialization), JSON  
- **Automation & Notification**: EmailOperator (Airflow)  

## **File Structure**  
- `Fraud_DAG.py` → Airflow DAG script for ETL pipeline and fraud prediction  
- `Modeling.ipynb` → Exploration and processing of transaction data  
- `model.pkl` → Machine Learning model used for prediction  

## **Conclusion and Recommendations**  
- **Automated fraud detection increases efficiency** → By implementing Apache Airflow, suspicious transaction detection can be performed automatically without manual intervention.  
- **Real-time notifications help the team with investigations** → The automatic alert system ensures preventive actions can be taken quickly to reduce potential losses due to fraud.  
- **Improved model accuracy** → With clean data and an optimized pipeline, the model can more accurately identify fraud transaction patterns.  
- **Future development** → Integration with a visualization dashboard (e.g., Tableau or Kibana) can provide deeper insights into suspicious transaction trends.  

## **Business Impact**  
- **Reduce losses due to fraud** → With faster and more accurate detection, the company can minimize potentially damaging fraudulent transactions.  
- **Increase customer trust** → A strong security system makes customers more confident in conducting transactions on the platform.  
- **Optimize security team resources** → With automated fraud detection, the team can focus more on investigating complex cases rather than manually processing transactions.  
- **Enhance compliance with regulations** → The fraud detection system helps the company meet financial security requirements and ensures more transparent transaction audits.  

## **How to Run the Project**  
1. **Run Apache Airflow** and ensure PostgreSQL is connected.  
2. **Add the DAG to Airflow** by saving `Fraud_DAG.py` in the DAG folder.  
3. **Activate the DAG** through the Airflow UI to process data and make predictions.  
4. **Check email notifications** if any transactions are detected as fraudulent.  

## **Contact**  
For any questions or suggestions regarding this project, please contact:  
**Email**: yinkasinulingga@gmail.com
