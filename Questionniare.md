# Algorithm Debt in Machine and Deep Learning Systems (V1)

## Page 1 — Introduction

You are invited to participate in this study conducted by **Iko-Ojo Simon**, a PhD candidate at the School of Computing at the Australian National University, as part of his thesis.  

The focus of his research is on *Algorithm Debt*, a new type of Technical Debt that arises from decisions made by developers during algorithm implementation. The aim of this study is to investigate the **causes, effects, and mitigation strategies** of Algorithm Debt within the Machine and Deep Learning domain.  

This survey consists of both open and closed-ended questions about Algorithm Debt in Machine and Deep Learning Systems.  

**If you do not have experience in developing Machine and Deep Learning systems, please do not proceed with the questionnaire.**  

**Definition:** Machine and Deep Learning systems are systems that integrate ML/DL models or algorithms with other non-ML/DL components.  

**Time:** The survey should take no more than **10 minutes** to complete and is required to be completed only once.  

**Ethics:** Approved by ANU’s Human Ethics Committee (Protocol: H/2024/0982).  

---

### Consent

By continuing, I confirm that:  

- I have read and understood the Participant Information Sheet.
- I have at least one year of hands-on experience with frameworks such as TensorFlow, Keras, DL4J, PyTorch, MXNet, or Microsoft Cognitive Toolkit e.t.c.
- Any questions or concerns I had about the project have been addressed.  
- I agree to participate in the study and understand that I may withdraw at any time before submitting my data.  
- I consent to the information I provide being included in a thesis, presentations, publications, and stored in an open repository, with anonymity preserved.

**Consent options:**

- [ ] Yes, I meet all the requirements and agree to participate.
- [ ] No, I do not agree or do not meet the criteria.

---

# Page 2 — Participant Characterisation

### Q1 — In which region are you currently employed?

- [ ] Africa
- [ ] Antarctica
- [ ] Oceania
- [ ] Asia
- [ ] Europe
- [ ] North America
- [ ] South America

### Q2 — Rate your experience in ML/DL systems development:

- [ ] Novice ovice (Minimal or “textbook” knowledge without connecting it to practice)
- [ ] Beginner (Working knowledge of key aspects of practice)
- [ ] Competent (Good working and background knowledge of area of practice)
- [ ] Proficient (Depth of understanding of discipline and area of practice)
- [ ] Expert (Authoritative knowledge of domain and deep tacit understanding across area of practice)

### Q3 — Are you answering based on your:

- [ ] Current role
- [ ] Previous role
- [ ] Both

### Q4 — Current or previous role:

- [ ] ML/DL Model Developer
- [ ] ML/DL Engineer
- [ ] ML/DL Model Analyst
- [ ] ML/DL Researcher
- [ ] Other: __________

---

# Page 3 — Technical Debt & Algorithm Debt

### Technical Debt

*Technical Debt* refers to the additional work or cost incurred due to shortcuts or suboptimal choices made during software development.

### Algorithm Debt

*Algorithm Debt* is a newly uncovered type of Technical Debt that results from algorithm implementations that may require rework as systems evolve — degrading performance, scalability, and quality.


### Algorithm Debt

*Algorithm Debt* is a newly uncovered type of Technical Debt that results from algorithm implementations that may require rework as systems evolve — degrading performance, scalability, and quality.

**Example of Algorithm Debt:**

```cpp
template <typename Dtype>
void PoolingLayer<Dtype>::Forward_cpu(const vector<Blob<Dtype>*>& bottom,
                                      const vector<Blob<Dtype>*>& top) {
    const Dtype* bottom_data = bottom[0]->cpu_data();
    Dtype* top_data = top[0]->mutable_cpu_data();
    const int top_count = top[0]->count();
    // TODO: improve pooling for "channel-first" cases
}
```
---

### Q5 — Familiarity with Algorithm Debt

- [ ] Not familiar at all
- [ ] Slightly familiar
- [ ] Moderately familiar
- [ ] Very familiar
- [ ] Extremely familiar

### Q6 — How often do you encounter Algorithm Debt?

- [ ] Never
- [ ] Rarely
- [ ] Sometimes
- [ ] Often
- [ ] Always

---

# Q7 — Causes of Algorithm Debt

**Please indicate how often each factor leads to Algorithm Debt:**

| Cause                                                    | Never | Rarely | Sometimes | Often | Always |
|----------------------------------------------------------|-------|--------|-----------|-------|--------|
| Hardware limitations                                     |       |        |           |       |        |
| API changes / compatibility issues                       |       |        |           |       |        |
| Data issues                                              |       |        |           |       |        |
| Model training processes                                 |       |        |           |       |        |

---

### Q8 — Other factors leading to Algorithm Debt

- [ ] Complexity of ML/DL algorithms
- [ ] Lack of developer knowledge
- [ ] Tight deadlines and delivery pressure
- [ ] Lack of documentation
- [ ] Insufficient testing
- [ ] Lack of team collaboration
- [ ] Other: __________

---

# Page 5 — Effects of Algorithm Debt

### Q9 — If encountered, what was the impact?

- [ ] No impact
- [ ] Minor impact
- [ ] Moderate impact
- [ ] Significant impact
- [ ] Not applicable

### Q10 — Effects of Algorithm Debt

- [ ] Poor model scalability
- [ ] Decreased model performance
- [ ] Model bias
- [ ] Increased maintenance costs
- [ ] Delayed project timelines
- [ ] Increased model complexity
- [ ] Loss of stakeholder confidence
- [ ] Other: __________

---

# Page 6 — Resolving/Mitigating Algorithm Debt

### Q11 — Could Algorithm Debt have been prevented?

- [ ] No
- [ ] Yes

### Q12 — How can Algorithm Debt be mitigated?

- [ ] Code reviews and refactoring
- [ ] Better resource allocation
- [ ] Improved team communication
- [ ] Systematic testing
- [ ] Automated management tools
- [ ] Other: __________

---

# Final Page — Final Thoughts

### Q13 — What are your thoughts on Algorithm Debt?

- [ ] It is an important concept needing more attention
- [ ] It is overemphasized
- [ ] It poses significant maintenance/scaling challenges
- [ ] I am concerned about long-term impacts
- [ ] There should be tools to manage it effectively
- [ ] Other: __________

---

**End of Survey**
