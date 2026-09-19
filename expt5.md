# Ex. No. 5 — Use Autopsy to Create a Case and Import Evidence

## Digital Forensics Lab

### Aim / Description

**Autopsy** is an open-source digital forensics platform used for analyzing and extracting data from digital devices.

This experiment demonstrates how to use Autopsy to create a forensic case, import evidence, analyze artifacts, and generate a forensic report.

---

## Evidence Files

The evidence files used for this experiment are:

* `4Dell Latitude CPi.E01`
* `4Dell Latitude CPi.E02`

---

# Procedure

## 1. Installation

### Download and Install Autopsy

Download and install **Autopsy** from its official website.

Follow the installation instructions according to the operating system being used.

---

## 2. Starting a New Case

### Open Autopsy

Launch the Autopsy application after installation.

### Create a New Case

1. Click **New Case**.
2. Enter the **Case Name**.
3. Select the **Location** where the case data will be stored.
4. Enter the required case details such as:

   * Case Number
   * Examiner's Name
   * Other relevant information
5. Click **Next**.

---

## 3. Adding a Data Source

### Choose the Type of Data Source

After creating a case, Autopsy prompts you to add a data source.

Autopsy supports different types of data sources, including:

* Disk Images
* Directories
* Logical Files
* Local Disks

### Select the Data Source

Browse to the location of the evidence file or disk that needs to be analyzed.

Supported examples include:

* `.E01`
* `.dd`
* `.raw`
* Physical Disk
* Directory

For this experiment, import:

```text
4Dell Latitude CPi.E01
4Dell Latitude CPi.E02
```

### Configure Ingest Modules

Autopsy provides several analysis modules that can be enabled or disabled depending on the investigation requirements.

Examples include:

* File Type Identification
* Keyword Search
* Hash Lookup
* Other available analysis modules

Select the required modules and click **Next** to start the analysis.

---

# 4. Initial Analysis and Overview

## Ingest Progress

As Autopsy processes the data source, the ingestion progress can be monitored from the application interface.

## Explore the Resulting Artifacts

Autopsy automatically categorizes the findings into different artifact categories, including:

* Web Artifacts
* File System Metadata
* Communication Records

## Use the Tree Viewer

The left-side tree viewer allows the investigator to navigate through different sections of the evidence.

Examples include:

* File System
* Web History
* Email
* Other forensic artifacts

---

# 5. Detailed Analysis

## Keyword Search

The **Keyword Search** module can be used to search for specific words or phrases within the evidence.

You can:

* Use pre-configured keyword lists
* Enter custom keywords
* Search for investigation-specific terms

---

## File Analysis

Navigate through files and folders using the **File Types** or **File System** sections.

You can:

* Open files
* View files
* Examine file information
* Export files for further analysis

---

## Timeline Analysis

Use the **Timeline** module to visualize events according to their timestamps.

Timeline analysis can help investigators understand and track user activity over time.

---

## Hash Analysis

Hash analysis can be used to compare file hashes against known databases.

This helps identify:

* Known good files
* Known bad files
* Previously identified files

---

# 6. Reporting

## Generate a Report

After completing the analysis:

1. Click **Generate Report** from the toolbar.
2. Select the required report format.
3. Choose the information and artifacts that should be included.
4. Generate the report.

Possible report formats include:

* HTML
* CSV
* Excel
* Other supported formats

---

## Export Findings

Individual files or forensic artifacts can be exported for:

* Inclusion in the final report
* Further forensic examination
* Evidence preservation

---

## Final Review

Review the generated report carefully to ensure that all relevant information has been included.

Save or print the report for use in the forensic case.

---

# 7. Case Closure

## Close the Case

Once the investigation has been completed, close the case within Autopsy.

## Archiving

Ensure that all relevant:

* Evidence
* Reports
* Case information

are properly archived according to the organization's policies.

---

# 8. Advanced Features (Optional)

## Custom Ingest Modules

Autopsy supports custom ingest modules that can be added when specific analysis capabilities are required beyond the default modules.

## Collaboration

Autopsy can be configured to support multi-user cases when working as part of a team environment.

---

# Result

The forensic evidence was successfully imported into **Autopsy**, analyzed using various forensic modules, and the relevant findings were reviewed and prepared for reporting.

## Screenshots
<img width="1007" height="577" alt="Screenshot 2026-08-31 162539" src="https://github.com/user-attachments/assets/03e212d9-e332-4c49-87d0-e4706e117f43" />
<img width="940" height="388" alt="image" src="https://github.com/user-attachments/assets/8fe2a0a2-45b9-4692-b4e5-ea3230a21dfa" />
<img width="940" height="348" alt="image" src="https://github.com/user-attachments/assets/e57c92ae-89df-4cd0-95ad-0b7f861c03df" />
<img width="940" height="521" alt="image" src="https://github.com/user-attachments/assets/9c21e24f-1784-4c0a-b5a7-0d2346fe40f4" />
<img width="940" height="485" alt="image" src="https://github.com/user-attachments/assets/2b725d77-144a-4170-a954-c84f8b77d6a0" />





