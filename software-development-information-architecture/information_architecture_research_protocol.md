# Research Protocol: Complete Information Architecture for Software Development
## A Mixed-Methods Analysis of Formal, Tacit, and Emergent Knowledge in the SDLC

---

## 1. RESEARCH IDENTIFICATION

**Protocol Version:** 1.0  
**Date:** November 2024  
**Research Type:** Mixed-methods systematic review with documentary analysis  
**Expected Duration:** 12-16 weeks  
**Output Format:** Validated information architecture model with empirical evidence  

---

## 2. RESEARCH QUESTION

### Primary Research Question
What constitutes a precise and complete information architecture describing ALL information required to design, build, deploy, and operate software that successfully achieves business outcomes?

### Secondary Research Questions
1. What information is formally documented versus retained in human memory (individual and collective)?
2. Where do theories (per Naur 1985) and hypotheses replace formal documentation across SDLC phases?
3. What assumptions substitute for logical analysis at critical decision points?
4. How do cognitive biases systematically affect what information gets captured?
5. What are the validated lifecycle processes, document types, and SDLC phases based on empirical evidence?

### Research Hypothesis
Software project failures correlate with systematic information gaps at three layers:
- **Layer 1:** Formal/Explicit (documented but incomplete)
- **Layer 2:** Tacit/Implicit (known but not written)
- **Layer 3:** Emergent/Contextual (arising from interactions)

---

## 3. THEORETICAL FRAMEWORK

### Core Theories
1. **Programming as Theory Building** (Naur 1985): Programs exist as theories in developers' minds
2. **SECI Model** (Nonaka & Takeuchi): Tacit/explicit knowledge conversion
3. **Conway's Law**: Organisational structure shapes system architecture
4. **Cognitive Bias Theory**: Systematic errors in information processing
5. **Transactive Memory Systems**: Distributed knowledge in teams

### Key Concepts to Track
- Theory: Knowledge enabling intelligent action, explanation, and modification
- Tacit Knowledge: Known but not articulated
- Information Gap: Difference between required and captured information
- Assumption: Unstated belief replacing analysis
- Cognitive Bias: Systematic deviation from rational judgment

---

## 4. METHODOLOGY

### 4.1 Research Design Overview

```
Phase 1: Systematic Literature Review (Weeks 1-3)
├── Stream A: Formal Standards Analysis
├── Stream B: Theoretical Foundations
└── Stream C: Empirical Studies

Phase 2: Documentary Analysis (Weeks 4-8)
├── Expert Discourse Mining
├── Post-Mortem Analysis
└── Repository Archaeology

Phase 3: Synthesis & Modelling (Weeks 9-11)
├── Information Architecture Model
├── Theory-Building Framework
└── Gap Analysis

Phase 4: Validation & Output (Weeks 12-16)
├── Cross-Validation
├── Model Refinement
└── Final Documentation
```

---

## 5. PHASE 1: SYSTEMATIC LITERATURE REVIEW

### 5.1 Search Strategy

#### A. Formal Standards Stream

**Sources:**
- IEEE Xplore Digital Library
- ISO Standards Repository
- SEI Digital Library
- Professional Body Standards (PMI, IIBA, ITIL)

**Standards to Review:**
```
ISO/IEC/IEEE 12207:2017 - Software Life Cycle Processes
ISO/IEC/IEEE 15288:2015 - System Life Cycle Processes
ISO/IEC/IEEE 29148:2018 - Requirements Engineering
ISO/IEC/IEEE 42010:2011 - Architecture Description
IEEE 1012-2016 - Verification and Validation
IEEE 829-2008 - Test Documentation
ISO/IEC 25010:2011 - Quality Models
```

**Extraction Template:**
```yaml
standard_id: [ISO/IEC/IEEE number]
lifecycle_phase: [phase name]
required_documents:
  - document_type: [name]
    purpose: [stated purpose]
    contents: [required elements]
    implicit_assumptions: [unstated prerequisites]
    theory_requirements: [knowledge needed to create/use]
```

#### B. Theoretical Foundations Stream

**Search Terms:**
```
("Programming as Theory Building" OR "Naur") AND software
("tacit knowledge" OR "implicit knowledge") AND (software OR programming)
"Conway's Law" AND (architecture OR organisation)
("cognitive bias" OR "systematic bias") AND (developer OR programmer)
("mental model" OR "shared understanding") AND software
("knowledge management" OR "knowledge transfer") AND development
```

**Databases:**
- Google Scholar
- ACM Digital Library
- arXiv
- ResearchGate
- Academia.edu

**Inclusion Criteria:**
- Published 1985-2024
- Peer-reviewed OR highly cited (>50 citations)
- Addresses knowledge/information in software development
- Empirical evidence OR theoretical framework

#### C. Empirical Studies Stream

**Target Sources:**
- Standish Group CHAOS Reports (1994-2024)
- State of DevOps Reports (2014-2024)
- McKinsey Digital Reports
- Gartner Research
- IEEE Software empirical studies
- ACM Computing Surveys

**Data Extraction Points:**
```python
study_data = {
    'sample_size': int,
    'methodology': str,
    'failure_rate': float,
    'primary_causes': list,
    'documentation_impact': float,
    'knowledge_gaps_identified': list,
    'success_factors': list
}
```

### 5.2 Quality Assessment Rubric

```
High Quality (Score 8-10):
□ Sample size > 500 OR longitudinal design
□ Clear methodology with reproducible procedures
□ Statistical significance reported
□ Limitations acknowledged
□ Peer-reviewed OR industry standard

Medium Quality (Score 5-7):
□ Sample size 50-500
□ Methodology described
□ Some quantitative data
□ Context specified

Low Quality (Score 2-4):
□ Sample size < 50
□ Limited methodology
□ Primarily anecdotal
□ Single organisation
```

---

## 6. PHASE 2: DOCUMENTARY ANALYSIS OF EXPERT DISCOURSE

### 6.1 Source Collection Protocol

#### Tier 1: Individual Thought Leaders

**Collection Method:**
```python
thought_leaders = {
    'architecture': [
        ('Martin Fowler', 'martinfowler.com', ['architecture', 'refactoring']),
        ('Simon Brown', 'simonbrown.je', ['C4 model', 'documentation']),
        ('Grady Booch', 'handbook.booch.com', ['design', 'architecture']),
    ],
    'engineering': [
        ('Kent Beck', 'multiple sources', ['XP', 'testing']),
        ('Michael Feathers', 'michaelfeathers.com', ['legacy', 'theory']),
        ('Jessica Kerr', 'jessitron.com', ['sociotechnical', 'systems']),
    ],
    'operations': [
        ('Charity Majors', 'charity.wtf', ['observability', 'ops']),
        ('Gene Kim', 'multiple sources', ['DevOps', 'transformation']),
    ]
}

for category, experts in thought_leaders.items():
    for name, source, topics in experts:
        collect_writings(name, source, topics)
        extract_patterns()
```

#### Tier 2: Organisational Knowledge

**Engineering Blogs to Mine:**
```
- engineering.stripe.com (documentation culture)
- netflixtechblog.com (operational knowledge)
- eng.uber.com (architectural decisions)
- medium.com/airbnb-engineering (knowledge sharing)
- about.gitlab.com/handbook (remote documentation)
- github.com/readme (engineering practices)
- stackoverflow.blog (developer insights)
```

#### Tier 3: Post-Mortem Collection

**Public Incident Databases:**
```
- github.com/danluu/post-mortems
- sre.google/sre-book/postmortem-culture
- aws.amazon.com/message/
- blog.cloudflare.com (incident tag)
- status.cloud.google.com/summary
```

### 6.2 Content Analysis Framework

#### A. Theory and Mental Model Detection

**Coding Instructions:**
```
WHEN encountering text about understanding/knowledge:
1. Mark passage with theory code (T1-T5)
2. Extract key quote
3. Note context (phase, role, situation)
4. Identify if formal/tacit/emergent
5. Note any tools/methods mentioned

Theory Codes:
T1: Explicit theory building
T2: Mental models described
T3: Knowledge transfer discussed
T4: Theory loss mentioned
T5: Theory reconstruction attempted
```

#### B. Assumption Mining

**Pattern Recognition Rules:**
```regex
Assumption Indicators:
/\b(assum\w+|suppos\w+|thought|believed|expected)\b/i
/\b(obvious\w+|clear\w+|of course|surely|definitely)\b/i
/\b(everyone knows?|well[- ]known|common knowledge)\b/i
/\b(didn't (think|consider|expect)|never occurred)\b/i
/\b(in (retrospect|hindsight)|looking back|should have)\b/i
```

#### C. Documentation Gap Extraction

**Gap Identification Protocol:**
```
FOR each story/example found:
  IDENTIFY the problem described
  EXTRACT what information was missing
  CATEGORISE the information type:
    - Requirements context
    - Design rationale  
    - Implementation decisions
    - Operational knowledge
    - Historical context
  ASSESS the impact described
  NOTE any mitigation suggested
```

### 6.3 Cognitive Bias Coding Scheme

```python
bias_detection = {
    'optimism': ['easy', 'simple', 'just', 'straightforward', 'trivial'],
    'confirmation': ['as expected', 'proves', 'validates', 'obviously worked'],
    'hindsight': ['should have seen', 'was obvious', 'signs were there'],
    'anchoring': ['original plan', 'initial design', 'first thought'],
    'availability': ['recent', 'last time', 'remember when', 'similar to'],
    'curse_of_knowledge': ['basic', 'fundamental', 'everyone knows', 'standard']
}
```

### 6.4 Repository Archaeology Protocol

**Target Repositories:**
```yaml
high_quality_examples:
  - name: kubernetes/kubernetes
    examine: [/docs, /design-proposals, ADRs]
  - name: rust-lang/rfcs
    examine: [RFC process, decision rationale]
  - name: python/peps
    examine: [PEP structure, acceptance criteria]

anti_patterns:
  - search: "legacy" "technical debt" "documentation"
  - extract: What went wrong, why not maintained
```

---

## 7. PHASE 3: SYNTHESIS AND MODELLING

### 7.1 Information Architecture Construction

**Four-Dimensional Model:**

```python
class InformationArchitecture:
    """Complete information model for SDLC"""
    
    dimensions = {
        'phase': [
            'business_need', 'requirements', 'architecture',
            'design', 'implementation', 'integration', 
            'verification', 'deployment', 'operation',
            'maintenance', 'disposal'
        ],
        'layer': [
            'formal_explicit',      # Written documents
            'tacit_implicit',       # Mental models, theories
            'emergent_contextual',  # Organisational, Conway's Law
            'assumed_hypothetical'  # Unstated beliefs
        ],
        'document_type': [
            # Populated from empirical findings
        ],
        'characteristics': [
            'rationale', 'alternatives', 'assumptions',
            'constraints', 'dependencies', 'context',
            'evolution', 'theory'
        ]
    }
    
    def map_information(self, phase, layer, doc_type, characteristics):
        """Maps information requirements across dimensions"""
        return self.validate_against_empirical_data()
```

### 7.2 Theory-Building Analysis

**For Each SDLC Phase:**
```yaml
phase_name:
  theory_components:
    - what: [What constitutes the theory at this phase]
    - who: [Who holds this theory]
    - transfer: [How theory transfers to next phase]
    - loss_points: [Where theory is lost]
    - documentation_gap: [What can't be documented]
    - reconstruction: [How to rebuild if lost]
  
  hypothesis_replacing_facts:
    - hypothesis: [Statement]
    - should_be: [What analysis should determine]
    - risk: [Impact if hypothesis wrong]
    - validation: [How to test]
```

### 7.3 Gap Analysis Framework

```python
def analyse_transition_gaps(phase_a, phase_b):
    """Analyses information loss at phase transitions"""
    
    required = get_required_information(phase_b)
    produced = get_typical_output(phase_a)
    documented = get_documented_information(phase_a)
    tacit = get_tacit_knowledge(phase_a)
    
    gaps = {
        'not_produced': required - produced,
        'not_documented': produced - documented,
        'not_transferable': tacit,
        'assumptions': get_assumptions_made(phase_a, phase_b)
    }
    
    return gaps, estimate_impact(gaps)
```

---

## 8. PHASE 4: VALIDATION AND OUTPUT

### 8.1 Triangulation Strategy

```
Method Triangulation:
├── Quantitative: Statistical patterns from empirical studies
├── Qualitative: Themes from expert discourse
└── Case Study: Patterns from post-mortems

Source Triangulation:
├── Academic: Peer-reviewed research
├── Practitioner: Expert blogs/talks
└── Organisational: Company practices

Theory Triangulation:
├── Naur's Theory Building
├── Knowledge Management
└── Cognitive Psychology
```

### 8.2 Validation Criteria

**Model Completeness:**
- [ ] All SDLC phases covered
- [ ] All information types identified
- [ ] All stakeholder perspectives included
- [ ] All failure patterns explained

**Empirical Grounding:**
- [ ] Supported by >5 independent sources
- [ ] Consistent with failure analyses
- [ ] Validated against success patterns
- [ ] No contradicting evidence unaddressed

### 8.3 Output Specifications

**Deliverable 1: Validated Information Architecture**
```yaml
format: Structured model
contents:
  - Complete enumeration by phase
  - Criticality ratings
  - Formal/tacit classification
  - Supporting evidence
validation: Cross-referenced with empirical data
```

**Deliverable 2: Theory-Building Framework**
```yaml
format: Practical guide
contents:
  - Theory components by phase
  - Transfer protocols
  - Loss prevention strategies
  - Reconstruction procedures
validation: Mapped to real examples
```

**Deliverable 3: Document Template Library**
```yaml
format: Actionable templates
contents:
  - Phase-specific templates
  - Decision records (ADRs)
  - Assumption tracking
  - Knowledge transfer checklists
validation: Based on successful practices
```

**Deliverable 4: Research Database**
```yaml
format: Searchable corpus
contents:
  - All sources analysed
  - Coded passages
  - Patterns identified
  - Evidence mapping
validation: Traceable and auditable
```

---

## 9. EXECUTION INSTRUCTIONS

### For Human Researchers

1. **Setup Phase:**
   - Create reference management system (Zotero/Mendeley)
   - Establish coding framework (NVivo/Atlas.ti/Obsidian)
   - Set up extraction templates

2. **Collection Phase:**
   - Follow search strategy systematically
   - Document all searches (query, date, results)
   - Apply inclusion/exclusion criteria consistently

3. **Analysis Phase:**
   - Code according to frameworks provided
   - Maintain audit trail of decisions
   - Regular inter-rater reliability checks if team

4. **Synthesis Phase:**
   - Use provided models as structure
   - Map findings to dimensions
   - Identify patterns and gaps

### For AI/LLM Researchers

```python
# Execution Framework for AI/LLM

class ResearchProtocol:
    """Reproducible research protocol for AI execution"""
    
    def execute_research(self):
        # Phase 1: Literature Review
        standards = self.analyse_standards()
        theory = self.extract_theoretical_foundations()
        empirical = self.synthesise_empirical_studies()
        
        # Phase 2: Documentary Analysis
        expert_discourse = self.mine_expert_writings()
        postmortems = self.analyse_failure_patterns()
        repositories = self.examine_real_examples()
        
        # Phase 3: Synthesis
        information_model = self.build_architecture_model(
            standards + theory + empirical + expert_discourse
        )
        
        # Phase 4: Validation
        validated_model = self.triangulate_findings(information_model)
        
        return self.generate_outputs(validated_model)
    
    def analyse_standards(self):
        """Process formal standards systematically"""
        for standard in STANDARDS_LIST:
            extract_lifecycle_processes(standard)
            identify_document_types(standard)
            detect_implicit_assumptions(standard)
            map_theory_requirements(standard)
    
    def mine_expert_writings(self):
        """Extract patterns from expert discourse"""
        for expert in EXPERT_LIST:
            collect_writings(expert)
            detect_theory_references()
            extract_assumptions()
            identify_gaps()
            code_cognitive_biases()
```

### Quality Controls

**Systematic Review Checklist:**
- [ ] Protocol registered/documented
- [ ] Search strategy comprehensive
- [ ] Inclusion criteria applied consistently
- [ ] Quality assessment performed
- [ ] Data extraction verified
- [ ] Synthesis method appropriate
- [ ] Limitations acknowledged

**Validity Threats Addressed:**
- [ ] Selection bias: Comprehensive search
- [ ] Publication bias: Include grey literature
- [ ] Confirmation bias: Contrary evidence sought
- [ ] Temporal bias: Date ranges specified

---

## 10. ETHICAL CONSIDERATIONS

- No human subjects involved
- Public sources only
- Fair use of copyrighted materials for research
- Proper attribution maintained
- No proprietary information used

---

## 11. TIMELINE

```
Weeks 1-3: Literature Review
├── Week 1: Standards analysis
├── Week 2: Theoretical foundations
└── Week 3: Empirical studies

Weeks 4-8: Documentary Analysis
├── Week 4-5: Expert discourse mining
├── Week 6-7: Post-mortem analysis
└── Week 8: Repository archaeology

Weeks 9-11: Synthesis
├── Week 9: Model construction
├── Week 10: Theory mapping
└── Week 11: Gap analysis

Weeks 12-16: Validation & Documentation
├── Week 12-13: Triangulation
├── Week 14-15: Model refinement
└── Week 16: Final outputs
```

---

## 12. REPRODUCIBILITY STATEMENT

This protocol is designed for reproducibility by:
- Providing explicit search strategies
- Defining clear inclusion/exclusion criteria
- Specifying coding schemes
- Documenting analysis procedures
- Including validation methods

Researchers following this protocol should achieve comparable findings, with variations expected in:
- Specific examples found
- Exact percentages (within 10% margin)
- Minor categorisation differences
- Temporal changes in practice

---

## APPENDICES

### A. Search String Library
[Detailed search strings for each database]

### B. Coding Dictionaries
[Complete coding schemes with examples]

### C. Extraction Templates
[Forms for data extraction]

### D. Quality Assessment Tools
[Rubrics and checklists]

### E. Expert Source List
[Comprehensive list with URLs]

### F. Repository Examples
[Specific files and patterns to examine]

---

END OF PROTOCOL

Document Status: Ready for Review
Next Step: Review protocol, then execute Phase 1