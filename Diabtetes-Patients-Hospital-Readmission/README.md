<!DOCTYPE html>
<html lang="en">
<head>
 
</head>
<body>
    <h1>Prediction on Diabetes Patient's Hospital Readmission</h1>

  <h2>Problem Statement and Objective</h2>
  <p>A hospital readmission occurs when a patient, discharged from the hospital, is readmitted within a certain period. Hospital readmission rates are now used as indicators of hospital quality and can adversely affect the cost of care. The Hospital Readmissions Reduction Program, established by the Centers for Medicare & Medicaid Services, aims to improve patient care quality and reduce healthcare spending by applying payment penalties to hospitals with higher than expected readmission rates for certain conditions. Although diabetes is not yet included in these penalties, it could be added in future measures.</p>
  <p>In 2011, American hospitals spent over $41 billion on diabetic patients readmitted within 30 days of discharge. Identifying factors that lead to higher readmission rates and predicting which patients will be readmitted can help hospitals save significant costs and improve care quality. This project uses a medical claims dataset to address the following questions:</p>
  <ul>
      <li>What factors are the strongest predictors of hospital readmission in diabetic patients?</li>
      <li>How well can we predict hospital readmission with the given dataset and features?</li>
  </ul>

  <h2>Data Set Description</h2>
  <table>
      <thead>
          <tr>
              <th>Variable Name</th>
              <th>Description</th>
          </tr>
      </thead>
      <tbody>
          <tr>
              <td>Encounter ID</td>
              <td>Unique identifier of an encounter</td>
          </tr>
          <tr>
              <td>Patient number</td>
              <td>Unique identifier of a patient</td>
          </tr>
          <tr>
              <td>Race</td>
              <td>Values: Caucasian, Asian, African American, Hispanic, and other</td>
          </tr>
          <tr>
              <td>Gender</td>
              <td>Values: male, female, and unknown/invalid</td>
          </tr>
          <tr>
              <td>Age</td>
              <td>Grouped in 10-year intervals: 0, 10), 10, 20), …, 90, 100)</td>
          </tr>
          <tr>
              <td>Weight</td>
              <td>Weight in pounds</td>
          </tr>
          <tr>
              <td>Admission type</td>
              <td>Integer identifier corresponding to 9 distinct values, e.g., emergency, urgent, elective, newborn, and not available</td>
          </tr>
          <tr>
              <td>Discharge disposition</td>
              <td>Integer identifier corresponding to 29 distinct values, e.g., discharged to home, expired, and not available</td>
          </tr>
          <tr>
              <td>Admission source</td>
              <td>Integer identifier corresponding to 21 distinct values, e.g., physician referral, emergency room, and transfer from a hospital</td>
          </tr>
          <tr>
              <td>Time in hospital</td>
              <td>Integer number of days between admission and discharge</td>
          </tr>
          <tr>
              <td>Payer code</td>
              <td>Integer identifier corresponding to 23 distinct values, e.g., Blue Cross/Blue Shield, Medicare, and self-pay Medical</td>
          </tr>
          <tr>
              <td>Medical specialty</td>
              <td>Integer identifier of a specialty of the admitting physician, corresponding to 84 distinct values, e.g., cardiology, internal medicine, family/general practice, and surgeon</td>
          </tr>
          <tr>
              <td>Number of lab procedures</td>
              <td>Number of lab tests performed during the encounter</td>
          </tr>
          <tr>
              <td>Number of procedures</td>
              <td>Number of procedures (other than lab tests) performed during the encounter</td>
          </tr>
          <tr>
              <td>Number of medications</td>
              <td>Number of distinct generic names administered during the encounter</td>
          </tr>
          <tr>
              <td>Number of outpatient visits</td>
              <td>Number of outpatient visits of the patient in the year preceding the encounter</td>
          </tr>
          <tr>
              <td>Number of emergency visits</td>
              <td>Number of emergency visits of the patient in the year preceding the encounter</td>
          </tr>
          <tr>
              <td>Number of inpatient visits</td>
              <td>Number of inpatient visits of the patient in the year preceding the encounter</td>
          </tr>
          <tr>
              <td>Diagnosis 1</td>
              <td>The primary diagnosis (coded as first three digits of ICD9); 848 distinct values</td>
          </tr>
          <tr>
              <td>Diagnosis 2</td>
              <td>Secondary diagnosis (coded as first three digits of ICD9); 923 distinct values</td>
          </tr>
          <tr>
              <td>Diagnosis 3</td>
              <td>Additional secondary diagnosis (coded as first three digits of ICD9); 954 distinct values</td>
          </tr>
          <tr>
              <td>Number of diagnoses</td>
              <td>Number of diagnoses entered into the system</td>
          </tr>
          <tr>
              <td>Glucose serum test result</td>
              <td>Indicates the range of the result or if the test was not taken. Values: “>200,” “>300,” “normal,” and “none” if not measured</td>
          </tr>
          <tr>
              <td>A1c test result</td>
              <td>Indicates the range of the result or if the test was not taken. Values: “>8” if the result was greater than 8%, “>7” if the result was greater than 7% but less than 8%, “normal” if the result was less than 7%, and “none” if not measured.</td>
          </tr>
          <tr>
              <td>Change of medications</td>
              <td>Indicates if there was a change in diabetic medications (either dosage or generic name). Values: “change” and “no change”</td>
          </tr>
          <tr>
              <td>Diabetes medications</td>
              <td>Indicates if there was any diabetic medication prescribed. Values: “yes” and “no”</td>
          </tr>
          <tr>
              <td>24 features for medications</td>
              <td>For generic names like metformin, repaglinide, and others, indicating if the drug was prescribed or dosage changed. Values: “up,” “down,” “steady,” “no”</td>
          </tr>
          <tr>
              <td>Readmitted</td>
              <td>Days to inpatient readmission. Values: “<30” if readmitted in less than 30 days, “>30” if readmitted in more than 30 days, and “No” for no record of readmission</td>
          </tr>
      </tbody>
  </table>

  <h2>Steps Involved</h2>
  <ol>
      <li><strong>Data Preparation & Exploration:</strong> Load and explore the dataset to understand its structure and contents.</li>
      <li><strong>Dealing with Missing Values:</strong> Handle missing data by employing imputation techniques or removing incomplete records.</li>
      <li><strong>Feature Engineering:</strong> Create new features or modify existing ones to improve model performance.</li>
      <li><strong>Data Visualization:</strong> Generate visualizations to identify patterns and relationships within the data.</li>
      <li><strong>Pre-Modeling Data Preprocessing:</strong> Prepare the data for modeling by normalizing or encoding categorical variables.</li>
      <li><strong>Modeling:</strong> Build and evaluate different predictive models.</li>
  </ol>

  <h2>Model Results</h2>
  <table>
      <thead>
          <tr>
              <th>Model</th>
              <th>Accuracy</th>
              <th>Precision</th>
              <th>Recall</th>
          </tr>
      </thead>
      <tbody>
          <tr>
              <td>Logistic Regression</td>
              <td>0.91</td>
              <td>0.00</td>
              <td>0.00</td>
          </tr>
          <tr>
              <td>Decision Tree</td>
              <td>0.86</td>
              <td>0.12</td>
              <td>0.09</td>
          </tr>
          <tr>
              <td>Random Forest</td>
              <td>0.91</td>
              <td>0.11</td>
              <td>0.00</td>
          </tr>
      </tbody>
  </table>

  <h2>Summary</h2>
  <p>The analysis reveals that while logistic regression and random forest models achieved the highest accuracy, they faced challenges with precision and recall, particularly with predicting readmissions. The logistic regression model, despite its accuracy, showed low precision and recall, indicating difficulties in correctly identifying patients who were readmitted within 30 days. Decision trees, while slightly less accurate, provided better interpretability and some improvement in precision and recall.</p>


<h2>Contributing</h2>
<p>Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.</p>
</body>
</html>
