# Revamp of the Underwriting Workflow: An AI-Powered Approach

This project, undertaken at Cathay Life Insurance, introduces an AI-driven workflow to modernize the traditional underwriting process. By leveraging Large Language Models (LLMs) and other AI technologies, this initiative aims to address the inefficiencies and inconsistencies inherent in manual, legacy systems.

## The Problem
Traditional underwriting is a labor-intensive process hampered by several key challenges:

**Scattered Information:** Critical data is spread across unstructured medical documents, diverse product guidelines, and extensive legacy rulebooks.

**Manual Interpretation:** Underwriters must manually interpret complex and often lengthy medical records.

**Inefficiencies:** This leads to prolonged turnaround times for evaluations.

**Errors and Inconsistency:** The manual process is prone to data entry errors and variability in decision-making among underwriters.

## The Solution

This project introduces a new, streamlined workflow powered by AI to create consistent and auditable risk evaluations. The system ingests unstructured medical documents, product guidelines, and over 1,000 underwriting guidelines, processing them to assist underwriters in making faster, more informed decisions.

The new workflow utilizes several AI-driven components.

**LLM Pre-processing:** Underwriting and product guidelines are pre-processed by an LLM. The product guidelines are transformed into a knowledge graph.

**Document Digitization and Summarization:** Optical Character Recognition (OCR) extracts text from new medical documents, which are then summarized by an LLM along with past medical records.

**Intelligent Agents:** A "Med Agent" and another central "Agent" are used to process and evaluate the collected information against the pre-processed guidelines.

**Data Integration:** A Text2Cypher model queries the knowledge graph created from product guidelines to integrate relevant product information.

The underwriter remains central to the final decision-making process, supported by the AI-generated evaluation and doctors' opinions.

## Key Applications & Features

### 1. Health Risk Calculator
A dynamic tool that visualizes the underwriting guidelines, allowing for faster and more consistent risk assessment.

**Reduces Human Variance:** Standardizes the evaluation process.

**Enhances Interpretability:** The visual interface makes the complex rules easier to understand and maintain.

**High Adoption:** Achieved a 100% usage rate within the underwriting department.

### 2. Automated Document Processing & Querying

An intelligent system that automates the analysis of medical records.

**High-Accuracy OCR:** Achieves over 88% accuracy in digitizing new medical documents.

**Medical Record Summarization:** An LLM processes and summarizes 30 million old medical records with over 95% accuracy, enabling quick querying by a "Med Agent".

### 3. (Work in Progress) Product Guideline Querying

This upcoming feature will allow for natural language queries of product guidelines by converting text to Cypher queries for a knowledge graph. This will enable the system to automatically factor in product-specific rules during the evaluation.

## Technical Overview

The core of the project is the strategic application of LLMs to parse, understand, and query complex, unstructured information. The underwriting guidelines, which have a semi-recursive structure, are broken down into a hierarchical decision tree. This structured data then powers the applications.

The system architecture integrates:

**Large Language Models (LLMs):** For pre-processing, summarization, and querying.

**Optical Character Recognition (OCR):** For digitizing paper documents.

**Knowledge Graphs & Text2Cypher:** To structure and query product guidelines.

**Vector Stores:** To enable efficient searching of summarized medical records.

This project demonstrates a significant step forward in applying AI to solve real-world challenges in the insurance industry, leading to increased efficiency, accuracy, and consistency in underwriting.

### Role:
1: digitized the underwriting guidelines with LLM.

2: completed the processing and summarization of old medical records with LLM.

3: automated the processing of new medical documents with OCR.
