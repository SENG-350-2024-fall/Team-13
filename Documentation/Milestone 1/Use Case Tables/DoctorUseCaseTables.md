# Doctor Use Cases

### Use Case 1: Review Results
|Use case | Review Results|
|-- | --|
|Description | Doctors review the triage results to verify that the results are correct.|
|Actors | Doctor|
|Assumptions | The result of the virtual triage is already ready for the doctor to review.|
|Steps | 1. Open the results 2. Read the results 3. Reflect on the results|
|Variations | N/A|
|Non-Functional | N/A|
|Issues | The doctor must still confirm or edit the triage result and potentially treat the patient.|

### Use Case 2: Confirm Results
|Use case | Confirm Results|
|-- | --|
|Description | The doctor confirms or edits the triage results.|
|Actors | Doctor|
|Assumptions | The result of the virtual triage is already ready for the doctor to review and confirm or delete.|
|Steps | 1. Open the results 2. Read the results 3. Reflect on the results 4. Confirm or edit results.|
|Variations | N/A|
|Non-Functional | N/A|
|Issues | The doctor must still confirm or edit the triage result and potentially treat the patient.|

### Use Case 3: Prescribe Medication
|Use case | Prescribe Medication|
|-- | --|
|Description | The doctor can prescribe medication if the patient needs any.|
|Actors | Doctor|
|Assumptions | The patient was correctly triaged and arrived at the ED.|
|Steps | 1. If the patient needs medication the doctor can prescribe it.|
|Variations | Can prescribe 0-infinity different medications|
|Non-Functional | N/A|
|Issues | No fail-safe if they prescribe the wrong medication.|

### Use Case 4: Order Lab Tests
|Use case | Order Lab Tests|
|-- | --|
|Description | Doctor orders additional lab tests if required to further assess a patient.|
|Actors | Doctor|
|Assumptions | The patient was correctly triaged and arrived at the ED.|
|Steps | 1. If the patient needs any lab test the doctor can prescribe them.|
|Variations | Can prescribe none or multiple lab tests.|
|Non-Functional | N/A|
|Issues | There is no fail-safe to verify that the patient gets the necessary lab test.|

### Use Case 5: Provide Medical Advice
|Use case | Provide Medical Advice|
|-- | --|
|Description | Doctor gives medical advice to patients either in person or through a virtual platform based on the triage or consultation.|
|Actors | Doctor|
|Assumptions | The patient was correctly triaged and arrived at the ED.|
|Steps | 1. If the doctor can specify the patient's steps to aid in their recovery.|
|Variations | There may be no medical advice or a lot.|
|Non-Functional | N/A|
|Issues | No regulated format is followed when delivering medical advice.|
