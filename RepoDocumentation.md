# Repository Documentation

This document provides an overview of the SFDC Cluster Analysis Package repository.

## Overview

This repository contains the source code for a Salesforce application that performs cluster analysis on Salesforce data. The application is built using Salesforce DX and includes Apex classes, Lightning Web Components, and other Salesforce metadata.

The main functionalities of this application are:

*   **Cluster Analysis:** It uses K-Means and K-Medoids (CLARA) algorithms to group records from any standard or custom object into clusters.
*   **Mixed Data Types:** It supports clustering of objects with mixed data types (numeric, category/picklist, text) using the Gower distance function.
*   **Text Clustering:** It can cluster free text (LongTextArea) fields using the TF-IDF (Term Frequency-Inverse Document Frequency) technique.
*   **Visualization:** It visualizes the clustering result using the t-SNE (t-distributed Stochastic Neighbor Embedding) dimensionality reduction technique.
*   **Similarity and Prediction:** It can find similar records and predict field values for any record using the K-Nearest Neighbors (KNN) algorithm.

## Programming Languages and Frameworks

The primary technologies used in this repository are:

*   **Apex:** A strongly-typed, object-oriented programming language that allows developers to execute flow and transaction control statements on Salesforce servers in conjunction with calls to the API.
*   **Lightning Web Components (LWC):** A UI framework for developing web apps on the Salesforce platform. It uses modern JavaScript, HTML, and CSS.
*   **Salesforce DX:** A set of tools that streamlines the entire development life cycle. It improves team development and collaboration, facilitates automated testing and continuous integration, and makes the release cycle more efficient and agile.

## Project Structure

The repository is structured as a Salesforce DX project:

*   `force-app/`: This directory contains the source code for the application.
    *   `main/default/`: Contains the main source code for the package.
        *   `classes/`: Apex classes.
        *   `lwc/`: Lightning Web Components.
        *   `aura/`: Aura components.
        *   `objects/`: Custom object definitions.
        *   `staticresources/`: Static resources like JavaScript libraries and CSS files.
    *   `main/algorithms/`: Contains the Apex classes for the clustering algorithms.
    *   `main/api/`: Contains the global API Apex classes.
    *   `main/utils/`: Contains utility Apex classes.
    *   `main/test/`: Contains the Apex test classes.
*   `sfdx-project.json`: The project configuration file for Salesforce DX.
*   `manifest/package.xml`: The package manifest file that defines the components to be included in the package.
*   `config/`: Contains configuration files for scratch orgs.
*   `README.md`: The main README file for the repository.

## How to Use

The `README.md` file provides detailed instructions on how to install, develop, build, and test the application. It also includes links to additional resources and documentation.
