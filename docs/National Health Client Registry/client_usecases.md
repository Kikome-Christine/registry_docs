# Client Registry Process Flows: 

## Registration Business Process 

![Registration Business Process](/images/Picture 1.png) 
## Use Case 1: Registering a New Patient
Registration of a new patient that does not exist in the facility based SHR.  
### Pre- conditions
-	Patient doesn’t exist in the shared health record
-	New Patient in Clinic 
-	Not Registered in either EMR
### Post Conditions
-	Patient is registered in the EMR
-	Patient exits in SHR
-	SHR generated ID is stored with the patient record in EMR
### Process Flow:
1.	Search Patient Record in either EMR or Shared Health Record.
2.	Register Patient Record in EMR.
3.	Post Patient Record in the Shared Health Record.
4.	Update Patient Record in EMR with Unique Identifier from the Shared Health Record. 

## Use Case 2: Patient Record Exists in Client Registry Not in EMR
The Patient record exists in the client registry and not in the EMR
### Pre- conditions
-	Patient exists in the client registry
-	Patient does not exist in the searching EMR
### Post Conditions
-	The client registry returns the patient searched value
-	Patient Record is displayed in the searching EMR window
### Process Flow:
1.	Search Patient Record in the Client registry
2.	Retrieve Patient Record from the client registry.  
3.	Register Patient Record in the EMR with Unique Identifier from the client registry. 

## Use Case 3: Patient Exists in client registry and EMR
### Pre conditions
-	Patient Record exists in the client registry
-	Patient Record exists in both EMR
### Post Conditions
-	Patient Record exists in both client registry and EMR
### Process Flow:
1.	Search Patient Record in the client registry.
2.	Display Patient Record. 

## Use Case 4: Patient Demographics Change
### Pre conditions
-	xxx
### Post Conditions
-	xxxx
### Process Flow:
3.	xxxx
## Test Cases: 
### Case 1: Registration of new patient record in EMR from client registry 
1.Start: Create a new patient record in EMR
2. EMR searches patient record in Client Registry
2. EMR pushes patient record to the client registry
3. End: EMR registers the retrieved patient record in its local database with the unique identifier generated from the client registry
### Case 2: Update of Patient Record



