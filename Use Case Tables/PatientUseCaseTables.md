# Use Cases
### Actor: Patient
**Use Case 1:** [Register Account](#use-case-1-register-account)<br>
**Use Case 2:** [Log In / Out](#use-case-2-log-in--out)<br>
**Use Case 3:** [Update Health Profile](#use-case-3-update-health-profile)<br>
**Use Case 4:** [Find Nearby Hospitals](#use-case-4-find-nearby-hospitals)<br>
**Use Case 5:** [View Hospital Wait Times](#use-case-5-view-hospital-wait-times)<br>
**Use Case 6:** [Call Emergency Hotline](#use-case-6-call-emergency-hotline)<br>
**Use Case 7:** [Register for Virtual Triage](#use-case-7-register-for-virtual-triage)<br>
**Use Case 8:** [View Triage Results](#use-case-8-view-triage-results)<br>
**Use Case 9:** [View Waitlist Position](#use-case-9-view-waitlist-position)<br>
**Use Case 10:** [Leave Waitlist](#use-case-10-leave-waitlist)<br>
**Use Case 11:** [View Medical History](#use-case-11-view-medical-history)<br>

# Patient Diagram
<div align="center">
  <picture>
    <source
      media="(prefers-color-scheme: dark)"
      srcset="https://github.com/SENG-350-2024-fall/Team-13/blob/main/Use%20Case%20Diagrams/Patient%20Diagram%20DR.png"
    />
    <source
      media="(prefers-color-scheme: light)"
      srcset="https://github.com/SENG-350-2024-fall/Team-13/blob/main/Use%20Case%20Diagrams/Patient%20Diagram%20WH.png"
    />
    <img
      alt="PlantUML"
      src="https://github.com/SENG-350-2024-fall/Team-13/blob/main/Use%20Case%20Diagrams/Patient%20Diagram%20WH.png"
    />
  </picture>
</div>


# PlantUML Script
```plantuml
@startuml
left to right direction
actor "Patient" as patient
rectangle "Mister ED Healthcare System" {
  rectangle "Account Management" {
    usecase "Register Account" as UC1
    usecase "Log In / Out" as UC2
  }
  rectangle "Health Profile" {
    usecase "Update Health Profile" as UC3
    usecase "View Medical History" as UC11
  }
  rectangle "Hospital Services" {
    usecase "Find Nearby Hospitals" as UC4
    usecase "View Hospital Wait Times" as UC5
    usecase "View Waitlist Position" as UC9
    usecase "Leave Waitlist" as UC10
  }
  usecase "Call Emergency Hotline" as UC6
  rectangle "Virtual Triage" {
    usecase "Register for Virtual Triage" as UC7
    usecase "View Triage Results" as UC8
  }
}

patient --> UC1
patient --> UC2
patient --> UC4
patient --> UC6
patient --> UC7
patient --> UC9

UC1 ..> UC3 : includes
UC2 ..> UC11 : includes
UC2 ..> UC3 : includes
UC7 ..> UC8 : includes
UC4 <|-- UC5 : extends
UC9 <|-- UC10 : extends

@enduml
```

# Use Case Tables

### Use Case 1: Register Account
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 1: Register Account                                                                              |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows a patient to create a new account in the Mister ED Healthcare System. The account is required to access other services, such as health profile management and hospital services. |
| **Actors**                                  | **Patient**: The individual seeking to create an account and access the healthcare services.              |
| **Assumptions**                             | - The patient has access to a mobile device or computer with an internet connection.<br> - The patient does not already have a registered Mister ED account. |
| **Steps**                                   | - The patient accesses the Mister ED homepage and clicks "Register Account".<br> - The patient enters required information (e.g., username, password, email).<br> - The patient optionally provides initial medical history.<br> - The patient confirms registration by clicking "Create Account".<br> - The patient is automatically logged into their new account and redirected to the homepage. |
| **Variations (Optional)**                   | - If the chosen username is already in use, the system prompts the patient to choose a different one.       |
| **Non-Functional (Optional)**               | - The system must securely store all sensitive information, including personal and medical data.            |
| **Issues**                                  | - Secure storage and encryption of sensitive personal data.<br> - Ensuring that password strength is adequate for account security. |

---

### Use Case 2: Log In / Out
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 2: Log In / Out                                                                                  |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows a patient to log into their Mister ED account to access services or log out to end their session. |
| **Actors**                                  | **Patient**: The individual logging into or out of their account.                                       |
| **Assumptions**                             | - The patient has an existing Mister ED account.                                                          |
| **Steps**                                   | - The patient clicks "Log In" on the homepage.<br> - The patient enters their username and password.<br> - Upon successful login, the system redirects the patient to their homepage.<br> - To log out, the patient clicks their profile in the top-right corner and selects "Log Out". |
| **Variations (Optional)**                   | - If the login credentials are incorrect, the system displays an error message and prompts the patient to retry. |
| **Non-Functional (Optional)**               | - The system must securely handle passwords and sessions, preventing unauthorized access.                 |
| **Issues**                                  | - Ensuring secure storage and encryption of login credentials to protect against unauthorized access.      |

---

### Use Case 3: Update Health Profile
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 3: Update Health Profile                                                                         |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to update their health profile, adding new medical conditions, allergies, or any other relevant health data. |
| **Actors**                                  | **Patient**: The individual updating their health profile.                                              |
| **Assumptions**                             | - The patient is logged into their Mister ED account.                                                     |
| **Steps**                                   | - The patient navigates to the health profile section.<br> - The patient updates their health information (e.g., new allergies, medications).<br> - The patient saves the updated information, and the system confirms the changes. |
| **Variations (Optional)**                   | - N/A                                                                                                    |
| **Non-Functional (Optional)**               | - The system must ensure that health data is stored securely and updated in real-time.                    |
| **Issues**                                  | - Ensuring that the updated data is accurate and securely stored.                                         |

---

### Use Case 4: Find Nearby Hospitals
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 4: Find Nearby Hospitals                                                                         |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to locate nearby hospitals using GPS and a map interface.                 |
| **Actors**                                  | **Patient**: The individual searching for nearby hospitals.                                             |
| **Assumptions**                             | - The patient’s device has GPS enabled, and they have internet access.                                    |
| **Steps**                                   | - The patient clicks "Find Nearby Hospitals" on the homepage.<br> - The system accesses the patient’s location and displays a map with nearby hospitals.<br> - The patient can click on a hospital to get more information, such as contact details and services. |
| **Variations (Optional)**                   | - N/A                                                                                                    |
| **Non-Functional (Optional)**               | - The system must display an accurate and up-to-date map based on the patient’s location.                 |
| **Issues**                                  | - Ensuring GPS accuracy and reliable mapping service.                                                     |

---

### Use Case 5: View Hospital Wait Times
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 5: View Hospital Wait Times                                                                      |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to view estimated wait times at hospitals nearby, which helps them decide where to seek medical treatment. |
| **Actors**                                  | **Patient**: The individual checking hospital wait times.                                               |
| **Assumptions**                             | - The patient has already found nearby hospitals through the system.                                      |
| **Steps**                                   | - The patient selects a hospital on the map.<br> - The system displays the estimated wait times for that hospital.<br> - The patient can compare wait times and choose the most convenient hospital. |
| **Variations (Optional)**                   | - N/A                                                                                                    |
| **Non-Functional (Optional)**               | - The system must regularly update wait times to reflect the current status at the hospital.              |
| **Issues**                                  | - Ensuring that hospital wait times are updated in real-time to provide accurate information.             |

---

### Use Case 6: Call Emergency Hotline
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 6: Call Emergency Hotline                                                                        |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows a patient to call an emergency hotline for urgent medical assistance. The system connects the patient with an emergency service or a healthcare professional. |
| **Actors**                                  | **Patient**: The individual seeking emergency medical assistance.                                       |
| **Assumptions**                             | - The patient is logged into their Mister ED account and has access to a phone or internet service.        |
| **Steps**                                   | - The patient clicks "Call Emergency Hotline" on the homepage.<br> - The system connects the patient to an emergency service for immediate medical assistance.<br> - The patient communicates their emergency to the service, and assistance is dispatched if necessary. |
| **Variations (Optional)**                   | - N/A                                                                                                    |
| **Non-Functional (Optional)**               | - The call must be secure and private to protect patient confidentiality.                                 |
| **Issues**                                  | - Ensuring the quality and reliability of the emergency communication system.                             |

---

### Use Case 7: Register for Virtual Triage
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 7: Register for Virtual Triage                                                                   |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to register for virtual triage, providing initial symptom information and receiving advice or next steps based on the assessment. |
| **Actors**                                  | **Patient**: The individual seeking medical evaluation through virtual triage.                          |
| **Assumptions**                             | - The patient is logged into their account and has internet access.                                       |
| **Steps**                                   | - The patient clicks "Register for Virtual Triage" and enters their symptoms.<br> - The system processes the symptoms and provides triage results, including possible next steps for treatment. |
| **Variations (Optional)**                   | - N/A                                                                                                    |
| **Non-Functional (Optional)**               | - The system must provide a quick and accurate evaluation of the patient's symptoms.                     |
| **Issues**                                  | - Ensuring that the virtual triage system provides accurate and timely medical advice.                    |

---

### Use Case 8: View Triage Results
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 8: View Triage Results                                                                           |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to view the results of their virtual triage session, which may include recommended next steps or suggested medical treatments. |
| **Actors**                                  | **Patient**: The individual reviewing the results of their virtual triage.                              |
| **Assumptions**                             | - The patient has already completed the virtual triage process and is logged into their account.           |
| **Steps**                                   | - The patient receives a notification that their triage results are available.<br> - The patient clicks "View Triage Results" and reviews the system's recommendations. |
| **Variations (Optional)**                   | - N/A                                                                                                    |
| **Non-Functional (Optional)**               | - The system must ensure that results are presented clearly and securely to the patient.                  |
| **Issues**                                  | - Ensuring the accuracy of triage results and safeguarding patient privacy.                               |

---

### Use Case 9: View Waitlist Position
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 9: View Waitlist Position                                                                        |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to view their position on a hospital or clinic waitlist.                  |
| **Actors**                                  | **Patient**: The individual checking their position on the waitlist.                                    |
| **Assumptions**                             | - The patient has previously joined a waitlist through the Mister ED system.                              |
| **Steps**                                   | - The patient clicks "View Waitlist Position" on the homepage.<br> - The system displays the patient’s current position on the waitlist for a hospital or clinic. |
| **Variations (Optional)**                   | - N/A                                                                                                    |
| **Non-Functional (Optional)**               | - The system must display real-time information about the patient’s waitlist position.                    |
| **Issues**                                  | - Ensuring real-time synchronization with the hospital or clinic's waitlist data.                         |

---

### Use Case 10: Leave Waitlist
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 10: Leave Waitlist                                                                               |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to leave a hospital or clinic waitlist if they no longer wish to remain in line for services. |
| **Actors**                                  | **Patient**: The individual removing themselves from a hospital or clinic waitlist.                     |
| **Assumptions**                             | - The patient has previously joined a waitlist.                                                           |
| **Steps**                                   | - The patient clicks "Leave Waitlist" on the homepage.<br> - The system confirms the patient’s removal from the waitlist. |
| **Variations (Optional)**                   | - N/A                                                                                                    |
| **Non-Functional (Optional)**               | - The system must immediately update the waitlist to reflect the patient’s removal.                       |
| **Issues**                                  | - Ensuring the patient is promptly removed from the waitlist and notifications are sent to the hospital or clinic. |

### Use Case 11: View Medical History
| **Field**                                   | **Description**                                                                                          |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Use Case Identifier and Reference Number**| Use Case 11: View Medical History                                                                         |
| **Modification History**                    | Created 2024/09/29 by Arfaz Hussain                                                                       |
| **Description**                             | This use case allows the patient to view their past medical history, including previous treatments, diagnoses, and procedures. |
| **Actors**                                  | **Patient**: The individual reviewing their medical history.                                            |
| **Assumptions**                             | - The patient is logged into their account and has previously visited medical providers through the Mister ED system. |
| **Steps**                                   | - The patient navigates to the "Health Profile" section.<br> - The patient clicks "View Medical History" to see a detailed log of past treatments, diagnoses, and medical visits.<br> - The patient can filter or search specific records if needed. |
| **Variations (Optional)**                   | - The patient may request to download a copy of their medical history.                                    |
| **Non-Functional (Optional)**               | - The system must securely store and display medical records, ensuring patient privacy and data protection. |
| **Issues**                                  | - Ensuring the accuracy of the displayed medical history and compliance with data privacy regulations.     |
