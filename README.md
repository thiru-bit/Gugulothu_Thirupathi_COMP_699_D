# iBooks – Your Intelligent Reading Companion

iBooks is a structured and explainable book recommendation system developed as part of the COMP-699-D Professional Seminar course. The system generates personalized book recommendations using explicitly defined user preferences such as favorite authors and previously rated books.

Unlike commercial recommendation platforms that rely on hidden behavioral tracking and complex machine learning pipelines, iBooks focuses on transparency, modularity, and explainable recommendation logic.

The project demonstrates:
- Object-oriented systems analysis and design
- Strategy-based recommendation logic
- Content-based recommendation concepts
- Boundary–Control–Entity (BCE) architecture
- Unit testing and modular implementation

---

# Project Objective

The objective of this project is to design and implement a lightweight recommendation system that:
- Accepts user-defined preferences
- Computes explainable similarity scores
- Generates ranked book recommendations
- Demonstrates modular object-oriented design principles
- Provides traceable recommendation outputs

---

# Technologies Used

- Python 3
- Jupyter Notebook
- Pandas
- NumPy
- unittest Framework

---

# Recommendation Approach

The system follows a content-based recommendation strategy using:
- Author similarity
- Rating similarity
- Weighted recommendation scoring

The recommendation logic is fully explainable and deterministic.

---

# Core Features

## User Features
- Create a user profile
- Add favorite authors
- Rate previously read books
- Generate personalized recommendations
- View recommendation explanations
- View recommendation scores and rankings

## Administrative Features
- Import book datasets
- Validate dataset structure
- Extract and organize dataset features
- Maintain dataset records

---

# System Architecture

The system follows the Boundary–Control–Entity (BCE) architecture.

## Boundary Layer
- RecommendationUI
- AdminUI

## Control Layer
- RecommendationController
- DatasetController

## Entity Layer
- UserProfile
- Book
- BookDataset
- Recommendation

## Strategy Layer
- SimilarityStrategy
- AuthorSimilarity
- RatingSimilarity

---

# Similarity Strategies

## Author Similarity
Checks whether a book author matches the user’s favorite authors.

## Rating Similarity
Compares the candidate book rating with the user’s average rating preference.

## Weighted Scoring
Final recommendation scores are generated using weighted similarity contributions.

Example:

```text
Final Score =
(Author Similarity × Weight)
+
(Rating Similarity × Weight)
```

---

# Project Structure

```text
Gugulothu_Thirupathi_COMP_699_D/
│
├── iBooks–ProjectCodewithUnitTests.ipynb
├── FinalPaper_CorrectedMappings.docx
├── README.md
```

---

# Dataset Information

The project uses a Goodreads books dataset containing:
- Book titles
- Authors
- Average ratings

Dataset Characteristics:
- ~11,000 book records
- Structured CSV format
- Lightweight and demonstration-friendly

Important attributes:
- `title`
- `author`
- `average_rating`

---

# Installation

## Clone Repository

```bash
git clone https://github.com/<your-username>/Gugulothu_Thirupathi_COMP_699_D.git
```

## Navigate to Repository

```bash
cd Gugulothu_Thirupathi_COMP_699_D
```

## Install Dependencies

```bash
pip install pandas numpy jupyter
```

---

# Running the Project

## Start Jupyter Notebook

```bash
jupyter notebook
```

## Open Notebook

Open:

```text
iBooks–ProjectCodewithUnitTests.ipynb
```

## Run All Cells

Execute all notebook cells sequentially.

The notebook will:
- Load and preprocess dataset
- Create system entities
- Build recommendation logic
- Generate recommendations
- Execute unit tests

---

# Example Recommendation Output

```text
1. Harry Potter and the Prisoner of Azkaban
   Author: J.K. Rowling
   Rating: 4.8
   Score: 0.92

   Reason:
   - Matches your favorite author
   - Rating is close to your preference
```

---

# Core Components

## Book Class
Represents individual books.

Attributes:
- Title
- Author
- Rating

## UserProfile Class
Stores:
- Favorite authors
- Rated books

## RecommendationController
Responsible for:
- Applying similarity strategies
- Combining weighted scores
- Filtering rated books
- Ranking recommendations

---

# Unit Testing

The project includes unit tests using Python’s `unittest` framework.

## Test Coverage

### Author Similarity Testing
Verifies preferred author matching logic.

### Rating Similarity Testing
Validates normalized similarity score generation.

### Recommendation Filtering
Ensures previously rated books are excluded.

### Recommendation Ranking
Validates recommendation ordering by score.

### End-to-End Workflow Testing
Tests the complete recommendation pipeline.

---

# Design Principles

The system emphasizes:
- Explainability
- Transparency
- Modularity
- Separation of concerns
- Maintainability

The recommendation process is intentionally interpretable and avoids black-box prediction models.

---

# UML and System Models

The project includes:
- Use-Case Diagram
- Activity Diagram
- Sequence Diagram
- Class Diagram
- Object Diagram
- Package Diagram
- Wireframe Design

---

# Performance Characteristics

The system is designed for:
- Interactive recommendation generation
- Small to moderate datasets
- Fast execution within Jupyter Notebook
- Demonstration-oriented workflows

---

# Limitations

- Limited to book recommendations
- Uses deterministic logic only
- No real-time learning
- No collaborative filtering
- No deep learning or behavioral tracking
- Requires structured datasets

---

# Future Enhancements

Possible future improvements include:
- Genre-based similarity
- Collaborative filtering
- Web application frontend
- Database integration
- Real-time recommendation updates
- User authentication
- Hybrid recommendation models

---

# Academic Context

Developed for:

```text
COMP-699-D Professional Seminar
Rivier University
Spring 2026
```

---

# References

1. Dennis, A., Wixom, B., & Tegarden, D. (2020).  
   *Systems Analysis and Design: An Object-Oriented Approach with UML (6th ed.)*

2. Gamma, E., Helm, R., Johnson, R., & Vlissides, J. (1994).  
   *Design Patterns: Elements of Reusable Object-Oriented Software*

3. Ricci, F., Rokach, L., & Shapira, B. (2011).  
   *Introduction to Recommender Systems Handbook*

---

# Author

## Thirupathi Gugulothu

Graduate Student  
COMP-699-D Professional Seminar  
Rivier University

---

# Repository Contents

- Final Project Report
- Jupyter Notebook Implementation
- Recommendation Engine Logic
- Strategy Pattern Implementation
- Unit Tests
- UML Models
- System Design Documentation
- Build and Execution Instructions
