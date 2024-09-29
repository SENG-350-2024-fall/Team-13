### Use Case 1: Register Account
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 1: Register Account                                                                              |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows a patient to create a new account in the Mister ED Healthcare System. The account is required to access other services, such as health profile management and hospital services. |
| **Actors**                                  | **Patient**: The individual seeking to create an account and access the healthcare services.              |
| **Assumptions**                             | 1. The patient has access to a mobile device or computer with an internet connection.<br> 2. The patient does not already have a registered Mister ED account. |
| **Steps**                                   | 1. The patient accesses the Mister ED homepage and clicks "Register Account".<br> 2. The patient enters required information (e.g., username, password, email).<br> 3. The patient optionally provides initial medical history.<br> 4. The patient confirms registration by clicking "Create Account".<br> 5. The patient is automatically logged into their new account and redirected to the homepage. |
| **Variations (Optional)**                   | 1. If the chosen username is already in use, the system prompts the patient to choose a different one.       |
| **Non-Functional (Optional)**               | 1. The system must securely store all sensitive information, including personal and medical data.            |
| **Issues**                                  | 1. Secure storage and encryption of sensitive personal data.<br> 2. Ensuring that password strength is adequate for account security. |

---

### Use Case 2: Log In / Out
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 2: Log In / Out                                                                                  |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows a patient to log into their Mister ED account to access services or log out to end their session. |
| **Actors**                                  | **Patient**: The individual logging into or out of their account.                                       |
| **Assumptions**                             | 1. The patient has an existing Mister ED account.                                                          |
| **Steps**                                   | 1. The patient clicks "Log In" on the homepage.<br> 2. The patient enters their username and password.<br> 3. Upon successful login, the system redirects the patient to their homepage.<br> 4. To log out, the patient clicks their profile in the top-right corner and selects "Log Out". |
| **Variations (Optional)**                   | 1. If the login credentials are incorrect, the system displays an error message and prompts the patient to retry. |
| **Non-Functional (Optional)**               | 1. The system must securely handle passwords and sessions, preventing unauthorized access.                 |
| **Issues**                                  | 1. Ensuring secure storage and encryption of login credentials to protect against unauthorized access.      |

---

### Use Case 3: Update Health Profile
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 3: Update Health Profile                                                                         |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to update their health profile, adding new medical conditions, allergies, or any other relevant health data. |
| **Actors**                                  | **Patient**: The individual updating their health profile.                                              |
| **Assumptions**                             | 1. The patient is logged into their Mister ED account.                                                     |
| **Steps**                                   | 1. The patient navigates to the health profile section.<br> 2. The patient updates their health information (e.g., new allergies, medications).<br> 3. The patient saves the updated information, and the system confirms the changes. |
| **Variations (Optional)**                   | 1. N/A                                                                                                    |
| **Non-Functional (Optional)**               | 1. The system must ensure that health data is stored securely and updated in real-time.                    |
| **Issues**                                  | 1. Ensuring that the updated data is accurate and securely stored.                                         |

---

### Use Case 4: Find Nearby Hospitals
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 4: Find Nearby Hospitals                                                                         |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to locate nearby hospitals using GPS and a map interface.                 |
| **Actors**                                  | **Patient**: The individual searching for nearby hospitals.                                             |
| **Assumptions**                             | 1. The patient’s device has GPS enabled, and they have internet access.                                    |
| **Steps**                                   | 1. The patient clicks "Find Nearby Hospitals" on the homepage.<br> 2. The system accesses the patient’s location and displays a map with nearby hospitals.<br> 3. The patient can click on a hospital to get more information, such as contact details and services. |
| **Variations (Optional)**                   | 1. N/A                                                                                                    |
| **Non-Functional (Optional)**               | 1. The system must display an accurate and up-to-date map based on the patient’s location.                 |
| **Issues**                                  | 1. Ensuring GPS accuracy and reliable mapping service.                                                     |

---

### Use Case 5: View Hospital Wait Times
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 5: View Hospital Wait Times                                                                      |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to view estimated wait times at hospitals nearby, which helps them decide where to seek medical treatment. |
| **Actors**                                  | **Patient**: The individual checking hospital wait times.                                               |
| **Assumptions**                             | 1. The patient has already found nearby hospitals through the system.                                      |
| **Steps**                                   | 1. The patient selects a hospital on the map.<br> 2. The system displays the estimated wait times for that hospital.<br> 3. The patient can compare wait times and choose the most convenient hospital. |
| **Variations (Optional)**                   | 1. N/A                                                                                                    |
| **Non-Functional (Optional)**               | 1. The system must regularly update wait times to reflect the current status at the hospital.              |
| **Issues**                                  | 1. Ensuring that hospital wait times are updated in real-time to provide accurate information.             |

---

### Use Case 6: Call Emergency Hotline
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 6: Call Emergency Hotline                                                                        |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows a patient to call an emergency hotline for urgent medical assistance. The system connects the patient with an emergency service or a healthcare professional. |
| **Actors**                                  | **Patient**: The individual seeking emergency medical assistance.                                       |
| **Assumptions**                             | 1. The patient is logged into their Mister ED account and has access to a phone or internet service.        |
| **Steps**                                   | 1. The patient clicks "Call Emergency Hotline" on the homepage.<br> 2. The system connects the patient to an emergency service for immediate medical assistance.<br> 3. The patient communicates their emergency to the service, and assistance is dispatched if necessary. |
| **Variations (Optional)**                   | 1. N/A                                                                                                    |
| **Non-Functional (Optional)**               | 1. The call must be secure and private to protect patient confidentiality.                                 |
| **Issues**                                  | 1. Ensuring the quality and reliability of the emergency communication system.                             |

---

### Use Case 7: Register for Virtual Triage
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 7: Register for Virtual Triage                                                                   |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to register for virtual triage, providing initial symptom information and receiving advice or next steps based on the assessment. |
| **Actors**                                  | **Patient**: The individual seeking medical evaluation through virtual triage.                          |
| **Assumptions**                             | 1. The patient is logged into their account and has internet access.                                       |
| **Steps**                                   | 1. The patient clicks "Register for Virtual Triage" and enters their symptoms.<br> 2. The system processes the symptoms and provides triage results, including possible next steps for treatment. |
| **Variations (Optional)**                   | 1. N/A                                                                                                    |
| **Non-Functional (Optional)**               | 1. The system must provide a quick and accurate evaluation of the patient's symptoms.                     |
| **Issues**                                  | 1. Ensuring that the virtual triage system provides accurate and timely medical advice.                    |

---

### Use Case 8: View Triage Results
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 8: View Triage Results                                                                           |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to view the results of their virtual triage session, which may include recommended next steps or suggested medical treatments. |
| **Actors**                                  | **Patient**: The individual reviewing the results of their virtual triage.                              |
| **Assumptions**                             | 1. The patient has already completed the virtual triage process and is logged into their account.           |
| **Steps**                                   | 1. The patient receives a notification that their triage results are available.<br> 2. The patient clicks "View Triage Results" and reviews the system's recommendations. |
| **Variations (Optional)**                   | 1. N/A                                                                                                    |
| **Non-Functional (Optional)**               | 1. The system must ensure that results are presented clearly and securely to the patient.                  |
| **Issues**                                  | 1. Ensuring the accuracy of triage results and safeguarding patient privacy.                               |

---

### Use Case 9: View Waitlist Position
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 9: View Waitlist Position                                                                        |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to view their position on a hospital or clinic waitlist.                  |
| **Actors**                                  | **Patient**: The individual checking their position on the waitlist.                                    |
| **Assumptions**                             | 1. The patient has previously joined a waitlist through the Mister ED system.                              |
| **Steps**                                   | 1. The patient clicks "View Waitlist Position" on the homepage.<br> 2. The system displays the patient’s current position on the waitlist for a hospital or clinic. |
| **Variations (Optional)**                   | 1. N/A                                                                                                    |
| **Non-Functional (Optional)**               | 1. The system must display real-time information about the patient’s waitlist position.                    |
| **Issues**                                  | 1. Ensuring real-time synchronization with the hospital or clinic's waitlist data.                         |

---

### Use Case 10: Leave Waitlist
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 10: Leave Waitlist                                                                               |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to leave a hospital or clinic waitlist if they no longer wish to remain in line for services. |
| **Actors**                                  | **Patient**: The individual removing themselves from a hospital or clinic waitlist.                     |
| **Assumptions**                             | 1. The patient has previously joined a waitlist.                                                           |
| **Steps**                                   | 1. The patient clicks "Leave Waitlist" on the homepage.<br> 2. The system confirms the patient’s removal from the waitlist. |
| **Variations (Optional)**                   | 1. N/A                                                                                                    |
| **Non-Functional (Optional)**               | 1. The system must immediately update the waitlist to reflect the patient’s removal.                       |
| **Issues**                                  | 1. Ensuring the patient is promptly removed from the waitlist and notifications are sent to the hospital or clinic. |

### Use Case 11: View Medical History
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 11: View Medical History                                                                         |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to view their past medical history, including previous treatments, diagnoses, and procedures. |
| **Actors**                                  | **Patient**: The individual reviewing their medical history.                                            |
| **Assumptions**                             | 1. The patient is logged into their account and has previously visited medical providers through the Mister ED system. |
| **Steps**                                   | 1. The patient navigates to the "Health Profile" section.<br> 2. The patient clicks "View Medical History" to see a detailed log of past treatments, diagnoses, and medical visits.<br> 3. The patient can filter or search specific records if needed. |
| **Variations (Optional)**                   | 1. The patient may request to download a copy of their medical history.                                    |
| **Non-Functional (Optional)**               | 1. The system must securely store and display medical records, ensuring patient privacy and data protection. |
| **Issues**                                  | 1. Ensuring the accuracy of the displayed medical history and compliance with data privacy regulations.     |