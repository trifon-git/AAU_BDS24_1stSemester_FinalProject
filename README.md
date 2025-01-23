# Project Title AI and the Danish Job Market: Looking Into Emerging Skills and Evolving Workforce Demands in the Era of Automation

This repository contains all the code and resources developed for the First Semester Final Project in Business Data Science (Class 2024) at Aalborg University.

# Project Overview: Job Listings Analysis Pipeline

## **[STEP 1] - Scraping Job Listings**
- This script scrapes **job listings** for each job category individually from the source website (*Job Index*).  
- It handles **progress tracking** using a progress log and saves the scraped data incrementally in a structured format.

---

## **[STEP1_MidStep1] - Merging Listings with HTML Links**
- This notebook **merges job listing files** generated in previous versions of the code.  

---

## **[STEP1_MidStep2] - Merging Listings Across Categories**
- This notebook combines **job listing data** across all job categories into a single, unified dataset.  
- The result is a comprehensive dataset containing all relevant job listings for analysis.

---

## **[STEP 2] - Generating Archive URLs**
- This script generates **dynamic archive URLs** for each job listing from the merged datasets in previous steps.  
- The URLs are prepared for further web scraping or data extraction.

---

## **[STEP 3] - Filtering Out Small Cities**
- This step filters out job listings associated with **small cities** that do not meet specified size or relevance criteria (e.g., population thresholds).  
- The cleaned data ensures only relevant entries are passed to the Playwright-based scraping operation.

---

## **[STEP 4] - Playwright HTML Extraction**
- In this step, **Playwright** is used to access each generated URL.  
- The script extracts **basic HTML content** from the pages dynamically loaded via the URLs.

---

## **[STEP 5.1] - Preprocessing Job Listings**
- This step further **cleans and filters** the job listings data.  
- It removes entries that fail to meet certain size, relevance, or quality criteria to refine the dataset.

---

## **[STEP 5.2] - LLM Processing**
- This step uses a **Large Language Model (LLM)** (llama 3.1:8b) to process the sampled data.  
- The LLM performs advanced text analysis and extraction based on the created System prompt.

**Some processes required adjustments partway through the project. To address this, we created mid-steps that were executed only once to implement the necessary changes and ensure the pipeline continued smoothly.**

---

## **[STEP 6.1] - Add Extra Variables to the Processed Data**
- Using APIs to add latitude,  longitude aswell as population numbers which will be useful for our application

---

## Authors
- **Anders Bjerring**  
- **Lauris Piziks**  
- **Tryfonas Karmiris**


