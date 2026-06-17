The **Course Transfer and Equivalency System** is a web-based tool designed to help students understand how their completed courses in one academic program can be recognized when transferring to another. Initially developed for Ilia State University, the system provides a clear visualization of transferable credits, equivalent courses, and additional offerings in the target program.

Built with **HTML, CSS, and JavaScript**, the application emphasizes simplicity and accessibility. Students can view their academic record, select a destination program, and instantly generate an equivalency table showing recognized courses and new program requirements.

**Key Features**

**Student Information Display**

The system presents essential student details such as name, ID, current program, and academic year.

**Course Record Table**

All completed and ongoing courses are listed with attributes like course title, credits, and pass/fail status.

**Program Transfer Selection**

Students can choose from multiple destination programs (e.g., Computer Science, Mathematics, Electrical Engineering). Once selected, the system automatically generates transfer information.

**Transfer Equivalency Display**

Results are divided into two sections:

1. **Passed Courses with Equivalents** – shows recognized courses and their equivalents in the new program.  
2. **Other Courses Offered** – lists additional courses available in the target program for planning purposes.

**Technical Architecture**

| Layer | Technology | Responsibility |
| :---: | ----- | ----- |
| **User Interface** | HTML | Layout, tables, buttons, program selection |
| **Presentation** | CSS | Styling, responsiveness, animations, user experience |
| **Logic** | JavaScript | Course rendering, transfer calculations, equivalency generation |

Data is stored in simple JavaScript objects:

* **Student Object** for personal details  
* **Courses Array** for academic records  
* **Equivalency Database** for predefined mappings

**Current Equivalency Algorithm**

The system uses a **rule-based, position-mapping approach**:

1. User selects a target program.  
2. The system loads the equivalency list for that program.  
3. Only passed courses are considered.  
4. Each course is matched by its index position in the array.  
5. Courses without equivalents are skipped.  
6. Recognized matches are displayed in the equivalency table.

This algorithm runs in time and space, making it efficient for small to medium academic records.

**User Workflow**

1. Open the application  
2. View course record  
3. Click “Transfer”  
4. Select a new program  
5. Generate equivalencies  
6. Review recognized and additional courses

**Limitations**

The current system is functional but limited:

* Equivalencies are manually defined  
* Course descriptions and learning outcomes are not analyzed  
* Credit similarity is not evaluated  
* Syllabi are not processed  
* AI techniques are not yet integrated  
* New programs require manual configuration

**Future Development Roadmap**

The next generation of the system aims to move beyond static mappings and incorporate **AI-driven automation** for greater accuracy and scalability.

**Automatic Syllabus Comparison**

Instead of manual definitions, the system will analyze syllabi and learning outcomes to determine equivalencies.

**Steps include:**

1. **Syllabus Collection** – gather documents from PDFs, DOCX files, and university databases.  
2. **Text Extraction & Preprocessing** – extract descriptions, objectives, topics, and assessments.  
3. **NLP Processing** – tokenize, clean, and extract keywords.  
4. **Semantic Embedding Generation** – convert syllabi into vector representations using models like BERT or Sentence Transformers.  
5. **Similarity Calculation** – measure course similarity using cosine similarity and keyword overlap.  
6. **Credit Evaluation** – compare ECTS values to ensure alignment.  
7. **Learning Outcome Matching** – recognize semantic similarities in objectives.  
8. **Decision Engine** – combine similarity, credits, and assessments into a weighted score.  
9. **Equivalency Table Generation** – produce a confidence-based table of matches.  
10. **Human Review** – advisors validate AI recommendations for fairness and compliance.

**Additional Enhancements**

* **User Authentication** for secure student/advisor access  
* **Real-Time University Data** via APIs for updated curricula  
* **AI Recommendation System** to suggest best-fit programs based on performance and interests  
* **Automatic Credit Calculation** for graduation progress tracking  
* **Automatic GPA calculations** for comparison with international standard

**Benefits of AI-Powered System**

| Feature | Benefit |
| :---: | ----- |
| **Automated Updates** | Eliminates manual data entry |
| **Scalability** | Handles hundreds of courses across programs |
| **Semantic Understanding** | Matches based on content, not just titles |
| **Confidence Scoring** | Provides measurable accuracy |
| **Continuous Learning** | Improves with human validation |
| **Multi-Program Support** | Extends easily across departments |

 

**Conclusion**

The Course Transfer and Equivalency System currently offers a straightforward way to visualize course recognition using manual mappings. However, its future lies in AI-enhanced automation, where syllabi are intelligently compared, credits are automatically calculated, and recommendations are personalized. By integrating natural language processing, semantic embeddings, and human validation, the system can evolve into a powerful academic decision-support tool, reducing manual effort, improving consistency, and empowering students with clearer pathways to success.

 

