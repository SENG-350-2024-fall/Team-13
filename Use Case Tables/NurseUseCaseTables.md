

| Use case | Conduct Initial Virtual Triage |
| :---- | :---- |
| **Description** | The **Nurse** conducts a virtual triage by interviewing the **Patient** and documenting symptoms, observations, and other information in real-time into the system. The **Nurse** uses this information to decide the appropriate course of action. |
| **Actors** | Primary: **Nurse**, Secondary: **Patient** |
| **Assumptions** | \- The **Nurse** has access to the system during the triage process. \- The **Patient** provides accurate and complete information during the meeting. |
| **Steps** | 1\. The **Nurse** starts the virtual triage process in the system. 2\. The **Nurse** asks the **Patient** questions about their symptoms and condition. 3\. The **Nurse** documents the symptoms and observations in real-time using the system. 4\. The **Nurse** makes a decision for what the next step is (e.g. whether to refer to a doctor, advise self-care, or recommend further medical evaluation). |
| **Variations** | \- The **Nurse** may ask follow-up questions based on incomplete information from the patient. |
| **Non-Functional** | \- The system should allow quick data entry and saving of information with minimal delay. |
| **Issues** | \- What should happen when the **Patient** cannot provide enough information for a complete triage? |

| Use case | Monitor ED Waiting Queue |
| :---- | :---- |
| **Description** | The **Nurse** monitors the emergency department (ED) waiting queue to assess patient triage priorities and ensure timely care for those needing immediate attention, in coordination with the **Receptionist**. |
| **Actors** | Primary: **Nurse**, Secondary: **Receptionist**, **Patient** |
| **Assumptions** | \- The **Receptionist** manages the queue logistics (e.g. adding/removing patients).  |
| **Steps** | 1\. The **Nurse** accesses the ED waiting queue. 2\. The **Nurse** reviews patient priority levels based on triage results. 3\. The **Nurse** adjusts the queue if any patients need faster attention. 4\. The **Nurse** provides feedback to the **Receptionist** to update the waiting list if needed. 5\. The **Nurse** coordinates with the **Receptionist** to manage the queue based on triage priorities. |
| **Variations** | \- The **Receptionist** may notify the **Nurse** of any administrative changes (e.g., patient check-ins). \- Patients may need to be re-triaged based on new symptoms. |
| **Non-Functional** | \- The ED queue is updated in real-time. |
| **Issues** | \- How should the system handle situations when the ED is overloaded and no beds are available? |

| Use case | Check Available Beds |
| :---- | :---- |
| **Description** | The **Nurse** checks the availability of beds in the ED to ensure that patients being called in for in-person visits can be accommodated. |
| **Actors** | Primary: **Nurse**, Secondary: **Patient** |
| **Assumptions** | \- The system accurately reflects real-time bed availability. |
| **Steps** | 1\. The **Nurse** accesses the ED bed availability list. 2\. The **Nurse** reviews the available beds and their statuses. 3\. The **Nurse** coordinates with the **receptionist** to update **patient** appointments based on bed availability.. |
| **Variations** | N/A |
| **Non-Functional** | \- The bed availability dashboard must refresh every 30 seconds. |
| **Issues** | \- How should the system handle discrepancies between the system information and the actual conditions (e.g. a patient takes longer to leave a bed than expected)? |

| Use case | Monitor Patient Post-Medication |
| :---- | :---- |
| **Description** | The **Nurse** monitors the patient after they have received and taken medication provided by the **Pharmacist**, checking for any adverse reactions or complications and ensuring that the medication is having the desired effect. |
| **Actors** | Primary: **Nurse**, Secondary: **Pharmacist**, **Doctor**, **Patient** |
| **Assumptions** | \- The **Patient** has picked up the medication from the **Pharmacist** and started taking it as prescribed. \- The **Nurse** has access to the patient's medication information and medical history. |
| **Steps** | 1\. The **Patient** takes the medication as prescribed. 2\. The **Nurse** schedules and conducts regular check-ins to monitor the patient’s response to the medication. 3\. The **Nurse** reviews any reported symptoms or side effects. 4\. If any complications arise, the **Nurse** consults with the **Doctor** or **Pharmacist** for further instructions. 5\. The **Nurse** updates the patient’s medical records with observations and outcomes. |
| **Variations** | \- If the patient experiences severe side effects, the **Nurse** may need to escalate the issue to the **Doctor** immediately. |
| **Non-Functional** | \- The system must allow for quick updates to patient records and facilitate real-time communication with the **Doctor** and **Pharmacist**. |
| **Issues** | \- How should the system handle cases where the patient does not adhere to the medication regimen? |

| Use case | Prepare Patient for Doctor Consultation |
| :---- | :---- |
| **Description** | The **Nurse** prepares the patient for their consultation with the **Doctor** by ensuring that all necessary medical information is up to date and ready for review. |
| **Actors** | Primary: **Nurse**, Secondary: **Doctor, Patient** |
| **Assumptions** | \- The **Patient** has provided all relevant medical data. \- The **Doctor** is ready to consult. |
| **Steps** | 1\. The **Nurse** gets the patient's medical records ready for the **Doctor**.  2\. The **Nurse** updates or collects any missing information from the patient. 3\. The **Nurse** ensures the patient is ready for the consultation. 4\. The **Nurse** notifies the **Doctor** that the patient is prepared for the consultation. |
| **Variations** | \- The **Nurse** may need additional tests or evaluations before the consultation begins. |
| **Non-Functional** | \- The system must ensure that the patient’s information is available to the **Doctor** within 30 seconds of the **Nurse** marking the patient as prepared. |
| **Issues** | \- How should the system handle incomplete patient records? |

