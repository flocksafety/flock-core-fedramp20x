<p align="center">
   <a href="https://flocksafety.com">
     <img src="https://raw.githubusercontent.com/flocksafety/flock-core-fedramp20x/refs/heads/master/images/Flock-Logo.png" awidth="100%">
   </a>
</p>

# Flock Safety's FedRAMP 20x Phase One Pilot Submission

## Flock Safety Overview

Flock Safety is a public safety solution that assists cities, businesses, schools, and law enforcement agencies in collaboratively eliminating crime and maintaining community safety. Flock develops and manufactures license plate reading (LPR) technology, audio recognition sensors, video cameras, and accompanying software to capture objective evidence required by law enforcement to solve crimes.

---
## ☁️ CSP Approach

Our approach can be summarized with the following steps:

1. **Lightweight Documentation**  
   Document the implementation of KSIs using Paramify Cloud with the FedRAMP 20x validations set.

2. **Key Security Indicators and Validations**  
   Gather and upload evidence into Paramify Cloud for each KSI validation, using automation where possible.

3. **Validate Evidence**  
    Meet with 3PAO and have them review and validate evidence in Paramify Cloud.

4. **Automate Machine-readable Package**  
   Generate and publish our machine-readable package using Paramify Cloud.

5. **3PAO Review**  
   3PAO reviews the package and adds attestation.

6. **Continuous Reporting Indication**  
   Either on-demand or per an automated schedule, a new package will be generated with the most current evidence.

7. **Prototype for Continuous Reporting**  
   It is anticipated that Paramify Cloud will allow for a shareable link that shows the KSI dashboard.

8. **CSP Rationale and Summary**  
   Summary of and rationale for the approach used to generate the machine-readable file, and evidence generation methods.

9. **CSP Submission**  
   Similar to the Continuous Reporting capability, the package will be available either with a viewable link or through the machine-readable package file with a friendly HTML viewer.

---

## Step-by-Step Details

### Step 1 – Lightweight Documentation
Document the implementation of our KSIs using Paramify Cloud with the FedRAMP 20x validations set.
![KSI Implementation Status](https://raw.githubusercontent.com/flocksafety/flock-core-fedramp20x/refs/heads/master/images/Paramify%20-%20KSI%20Implementation.png)

### Step 2 – Key Security Indicators and Validations
Gather and upload evidence into Paramify Cloud for each KSI validation, using automation where possible.
![Evidence Repo](https://raw.githubusercontent.com/flocksafety/flock-core-fedramp20x/refs/heads/master/images/Paramify%20-%20Evidence%20Repo.png)

### Step 3 – Validate Evidence
Meet with 3PAO and have them review and validate evidence in Paramify Cloud. 3PAO can set Assurance Steps/Results, Assurance Status, and leave notes or remarks. 
![3PAO Assurance](https://raw.githubusercontent.com/flocksafety/flock-core-fedramp20x/refs/heads/master/images/Paramify%20-%203PAO%20Assessment.png)

Flock Safety is working with Baker Tilly, formerly known as Moss Adams, as 3PAO.

### Step 4 – Automate Machine Readable Package
Publish our machine-readable format package using Paramify Cloud’s DocRobot capabilities.
Our draft package submission is represented using YAML due to its simplicity.

---

## 📑 Assessment File Structure
The machine-readable assessment file is a YAML file with the following structure (see full YAML file here -- [images/flock_safety_20x_scrubbed_v2.yaml](https://github.com/flocksafety/flock-core-fedramp20x/blob/master/images/flock_safety_20x_compliance_scrubbed_v2.yaml)

```yaml
Package:
  CSPName: <Company name of Cloud Service Provider>
  CSO: <Cloud Service Offering / Name of application>
  impact: <Low | Moderate | High>
  summaryOfCSO: <Description of CSO>
  Assessments:
  - Assessment:
    digitalSignature: <SHA hash of assessment elements below>
    assessorOrg: <Third Party Assessment Organization>
    date: <date of assessment>
    leadAssessor: <name of lead assessor>
    recommendation: <Authorize | Do Not Authorize>
    remarks: <assessment remarks>
    KSIs:
    - KSI:
      name: <name of KSI>
      shortName: <shortname of KSI>
      Validations:
      - validation:
        shortName: <shortname of validation>
        description: <description of validation>
        implementationStatus: <True | False | Partial>
        assessmentStatus: <True | False | Partial >
        Evidences:
        - evidence:
          name: <name of evidence>
          Artifacts:
          - artifact:
            reference: <evidence file>
```
---

### Step 5 - 3PAO Review
3PAO reviews package and adds attestation. This is included at the Assessment level in the machine-readable package
```
  - Assessment:
    digitalSignature: <SHA hash of assessment elements below>
    assessorOrg: <Third Party Assessment Organization>
    date: <date of assessment>
    leadAssessor: <name of lead assessor>
    recommendation: <Authorize | Do Not Authorize>
    remarks: <assessment remarks>
```

#### Assessment Methodology</a>

(see [Signed 3PAO Assessment Methodology](https://github.com/flocksafety/flock-core-fedramp20x/blob/c87cad23c6af2f8a1c4f91ee3697843cbf745735/images/Assessment%20Methodology.pdf))

![https://raw.githubusercontent.com/flocksafety/flock-core-fedramp20x/refs/heads/master/images/Signed%203PAO%20Assessment%20Methodology.png?token=GHSAT0AAAAAAC5XQLLV6AK7AAUUKU6YYZWE2CQG7DA](https://raw.githubusercontent.com/flocksafety/flock-core-fedramp20x/refs/heads/master/images/Signed%203PAO%20Assessment%20Methodology.png)

### Step 6 - Continuous Reporting Indication
Either on-demand or per an automated schedule, a new package will be generated with the most current evidence using Paramify's DocRobot capability.

### Step 7 - Prototype for Continuous Reporting
It is anticipated that Paramify Cloud will allow for a shareable link that shows the KSI dashboard.

### Step 8 - CSP Rationale and Summary
A summary of and rationale for the approach used to generate the machine-readable file, and evidence generation methods is provided with the machine-readable package file.

### Step 9 - CSP Submission
Similar to the Continuous Reporting capability, the package will be available either with a viewable link in Paramify or through the machine-readable package file.

---


## 📩 Contact
Reach out to robert.otten@flocksafety.com for questions.
