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

### Appendix A: Search String Library

#### A.1 Formal Standards Searches
```
Database: IEEE Xplore
("ISO/IEC/IEEE 12207" OR "software life cycle") AND (processes OR documentation)
("ISO/IEC/IEEE 29148" OR "requirements engineering") AND (specification OR elicitation)
("architecture decision" OR "design rationale") AND software
("verification" OR "validation") AND (documentation OR artifacts)

Database: ISO Standards Repository
12207:2017 software processes
15288:2015 system processes
29148:2018 requirements
42010:2011 architecture

Database: Google Scholar
"software documentation" AND "empirical study" AND (quality OR effectiveness)
"requirements engineering" AND "project failure" AND empirical
"tacit knowledge" AND "software development" AND (transfer OR sharing)
"cognitive bias" AND (programming OR "software engineering")
"Conway's Law" AND (architecture OR organization) AND empirical
```

#### A.2 Theoretical Foundations Searches
```
Primary Terms:
("Programming as Theory Building" OR "Naur") AND software
("tacit knowledge" OR "implicit knowledge") AND (software OR programming)
"Conway's Law" AND (architecture OR organisation OR organization)
("cognitive bias" OR "systematic bias") AND (developer OR programmer)
("mental model" OR "shared understanding") AND software
("knowledge management" OR "knowledge transfer") AND development
("transactive memory" OR "team knowledge") AND software
"documentation debt" OR "documentation technical debt"
"self-admitted technical debt" OR SATD

Combined Searches:
("software project failure" OR "project success") AND (documentation OR requirements)
("information loss" OR "knowledge loss") AND "software development"
("organizational structure" OR "team structure") AND "system architecture"
"Architecture Decision Record" OR ADR OR "design rationale"
```

#### A.3 Empirical Studies Searches
```
Industry Reports:
site:standishgroup.com CHAOS report
site:mckinsey.com "software project" failure
site:gartner.com "IT project" success rate
site:pmi.org "pulse of profession" software

Academic Empirical:
"systematic mapping study" AND "software engineering"
"empirical study" AND "software documentation"
"case study" AND "requirements engineering" 
"field study" AND "cognitive bias" AND software
meta-analysis AND "software project" AND (success OR failure)
```

### Appendix B: Coding Dictionaries

#### B.1 Theory and Mental Model Codes
```
T1: Explicit Theory Building
- Direct reference to Naur or "theory building"
- Mentions of "mental model" or "conceptual model"
- Discussion of "understanding" vs "knowing"
Example: "Developers build a theory of how the system works"

T2: Implicit Mental Models
- References to "how developers think about" the system
- Mentions of "system understanding"
- Implicit knowledge descriptions
Example: "The team just knows how it works"

T3: Knowledge Transfer
- Onboarding discussions
- Mentoring or pairing references
- Documentation for future developers
Example: "We pair new developers with seniors"

T4: Theory Loss
- Departure of key personnel
- Loss of system understanding
- "Bus factor" discussions
Example: "When John left, nobody understood the payment system"

T5: Theory Reconstruction
- Reverse engineering efforts
- Archaeological debugging
- Legacy system understanding
Example: "We had to figure out how the old system worked"
```

#### B.2 Cognitive Bias Codes
```
CB1: Preconception Bias
Keywords: assumed, expected, obvious, clearly
Example: "We assumed users would understand"

CB2: Ownership Bias
Keywords: my code, their code, not mine
Example: "My code doesn't need documentation"

CB3: Fixation Bias
Keywords: original design, initial approach, always done
Example: "We stuck with the original design"

CB4: Resort to Default
Keywords: standard, usual, template, boilerplate
Example: "We used the standard template"

CB5: Optimism Bias
Keywords: should work, probably fine, unlikely to fail
Example: "The code should be self-explanatory"

CB6: Convenience Bias
Keywords: quick fix, temporary, for now, technical debt
Example: "This is just a temporary workaround"

CB7: Subconscious Action
Keywords: copied, found online, Stack Overflow
Example: "I found this solution on Stack Overflow"

CB8: Blissful Ignorance
Keywords: seems to work, haven't seen problems, probably okay
Example: "It seems to work fine in testing"

CB9: Superficial Selection
Keywords: looks good, seems right, good enough
Example: "This looks like it'll work"

CB10: Memory Bias
Keywords: recently, last time, remember when
Example: "Last time we did it this way"
```

#### B.3 Documentation Gap Codes
```
DG1: Requirements Context
- Missing WHY behind requirements
- Stakeholder rationale absent
- Business context not captured

DG2: Design Rationale
- Alternatives not documented
- Trade-offs not explained
- Decisions without justification

DG3: Implementation Knowledge
- Code without comments
- Complex logic unexplained
- Assumptions not stated

DG4: Operational Wisdom
- Deployment steps missing
- Monitoring not documented
- Troubleshooting absent

DG5: Historical Context
- Evolution not tracked
- Changes without explanation
- Legacy decisions forgotten
```

### Appendix C: Extraction Templates

#### C.1 Study Data Extraction Form
```yaml
study_id: [Author_Year_Title]
citation: [Full citation]
source_type: [Academic/Industry/Grey Literature]
  
methodology:
  design: [Case Study/Survey/Experiment/Review]
  sample_size: [n=X]
  context: [Industry/Domain/Geography]
  duration: [Time period]
  
findings:
  failure_rate: [%]
  success_factors: [List]
  failure_causes: [List]
  documentation_impact: [Description + %]
  
knowledge_gaps:
  formal: [What documentation was missing]
  tacit: [What knowledge was implicit]
  emergent: [What arose from context]
  
quality_assessment:
  score: [1-10]
  strengths: [List]
  limitations: [List]
  confidence: [High/Medium/Low]
  
relevant_quotes:
  - quote: [Text]
    page: [Number]
    context: [Explanation]
```

#### C.2 Expert Discourse Extraction Form
```yaml
expert_name: [Name]
source: [Blog/Talk/Article]
date: [Publication date]
url: [Web address]

key_insights:
  theory_building: [References to mental models]
  documentation: [Views on documentation]
  knowledge_transfer: [Approaches mentioned]
  biases: [Cognitive biases discussed]
  
practical_advice:
  practices_recommended: [List]
  practices_discouraged: [List]
  tools_mentioned: [List]
  
assumptions_identified:
  explicit: [Stated assumptions]
  implicit: [Unstated beliefs detected]
  
gaps_acknowledged:
  - gap: [Description]
    impact: [Consequences mentioned]
    mitigation: [Solutions proposed]
```

#### C.3 Post-Mortem Analysis Template
```yaml
incident: [Name/Company]
date: [When occurred]
cost: [Financial/human impact]
source: [Report URL/citation]

failure_pattern:
  category: [Requirements/Design/Implementation/etc]
  root_cause: [Primary cause]
  contributing_factors: [List]
  
documentation_gaps:
  missing: [What wasn't documented]
  outdated: [What was wrong]
  ignored: [What was documented but not followed]
  
knowledge_issues:
  tacit_knowledge_lost: [What wasn't transferred]
  assumptions_made: [Unstated beliefs]
  biases_present: [Cognitive biases identified]
  
lessons:
  technical: [Technical learnings]
  process: [Process improvements]
  organizational: [Organizational changes]
  
prevention:
  could_have_helped: [What would have prevented]
  recommendations: [Specific actions]
```

### Appendix D: Quality Assessment Tools

#### D.1 Study Quality Rubric
```
Scoring Guide (10 point scale):

Methodology (3 points):
□ Clear research questions (1 point)
□ Appropriate method for questions (1 point)
□ Rigorous execution described (1 point)

Sample (3 points):
□ Sample size >500 or longitudinal (2 points)
□ Sample size 50-500 (1 point)
□ Representative sample (1 point)

Analysis (2 points):
□ Appropriate statistical/qualitative analysis (1 point)
□ Clear presentation of results (1 point)

Validity (2 points):
□ Limitations acknowledged (1 point)
□ Threats to validity addressed (1 point)

Classification:
8-10: High Quality (strong confidence)
5-7: Medium Quality (moderate confidence)
2-4: Low Quality (supporting only)
```

#### D.2 Documentation Quality Checklist
```
Coverage Assessment:
□ Requirements documented
□ Architecture documented
□ Design rationale captured
□ Implementation documented
□ Test coverage documented
□ Deployment procedures exist
□ Operational runbooks present
□ Maintenance guides available

Quality Criteria:
□ Up-to-date (< 30 days old)
□ Accurate (verified against code)
□ Complete (all sections filled)
□ Clear (readability score >60)
□ Accessible (easy to find)
□ Useful (actually used by team)
□ Maintained (regular updates)
```

#### D.3 Bias Detection Checklist
```
For Research Papers:
□ Publication bias considered
□ Confirmation bias in interpretation
□ Selection bias in sampling
□ Survivorship bias in cases

For Expert Discourse:
□ Authority bias (accepting without evidence)
□ Recency bias (overweighting recent events)
□ Availability bias (memorable over representative)
□ Hindsight bias (knew it all along)

For Case Studies:
□ Outcome bias (judging by results only)
□ Attribution bias (cause assignment)
□ Narrative bias (fitting stories)
□ Cherry-picking (selective examples)
```

### Appendix E: Expert Source List

#### E.1 Individual Thought Leaders
```
Software Architecture:
- Martin Fowler: https://martinfowler.com
  Topics: Architecture, Refactoring, Patterns
  Key Articles: "Is Design Dead?", "Architecture Decision Records"
  
- Simon Brown: https://simonbrown.je
  Topics: C4 Model, Architecture Documentation
  Resources: Software Architecture for Developers

- Grady Booch: https://handbook.booch.com
  Topics: Architecture, Design, UML
  Notable: Architecture handbook online

Engineering Practices:
- Kent Beck: https://www.kentbeck.com
  Topics: XP, TDD, Patterns
  Key Work: "Extreme Programming Explained"

- Michael Feathers: https://michaelfeathers.com
  Topics: Legacy Code, Theory Building
  Key Work: "Working Effectively with Legacy Code"

- Jessica Kerr: https://jessitron.com
  Topics: Sociotechnical Systems, Symmathesy
  Notable: Systems thinking in software

DevOps and Operations:
- Charity Majors: https://charity.wtf
  Topics: Observability, Operations, Testing in Production
  
- Gene Kim: https://itrevolution.com
  Topics: DevOps, Phoenix Project
  Resources: DevOps Research

- Nicole Forsgren: https://nicolefv.com
  Topics: DORA metrics, DevOps research
  Key Work: "Accelerate"

Cognitive Science & Teams:
- Chelsea Troy: https://chelseatroy.com
  Topics: Technical Debt, Maintenance, Team Dynamics
  
- Dan Luu: https://danluu.com
  Topics: Postmortems, Performance, Failure Analysis
  Notable: Extensive postmortem collection

- Hillel Wayne: https://www.hillelwayne.com
  Topics: Formal Methods, Empirical Software Engineering
```

#### E.2 Organizational Blogs
```
Engineering Excellence:
- Stripe Engineering: https://stripe.com/blog/engineering
- Netflix Tech Blog: https://netflixtechblog.com
- Uber Engineering: https://eng.uber.com
- Airbnb Engineering: https://medium.com/airbnb-engineering
- Spotify Engineering: https://engineering.atspotify.com

Documentation Culture:
- GitLab Handbook: https://about.gitlab.com/handbook
- Thoughtworks Tech Radar: https://www.thoughtworks.com/radar
- Google Engineering: https://developers.googleblog.com

Incident Analysis:
- Google SRE: https://sre.google/sre-book
- AWS Post-Event Summaries: https://aws.amazon.com/message
- Cloudflare Blog: https://blog.cloudflare.com (incident tag)
- GitHub Engineering: https://github.blog/category/engineering
```

#### E.3 Research Organizations
```
Industry Research:
- Standish Group: https://www.standishgroup.com
- McKinsey Digital: https://www.mckinsey.com/capabilities/mckinsey-digital
- Gartner Research: https://www.gartner.com
- PMI: https://www.pmi.org
- DORA: https://www.devops-research.com

Academic:
- IEEE Software: https://www.computer.org/csdl/magazine/sw
- ACM Queue: https://queue.acm.org
- Empirical Software Engineering journal
- Information and Software Technology journal
```

### Appendix F: Repository Examples

#### F.1 High-Quality Documentation Examples
```yaml
kubernetes/kubernetes:
  examine:
    - /docs/design-proposals/* (design decisions)
    - /docs/devel/* (development documentation)
    - /CHANGELOG/* (evolution tracking)
  patterns:
    - KEPs (Kubernetes Enhancement Proposals)
    - SIG documentation structure
    - API documentation generation

rust-lang/rfcs:
  examine:
    - /text/* (accepted RFCs)
    - Template structure
    - Decision process documentation
  patterns:
    - RFC process for decisions
    - Community input integration
    - Rationale documentation

python/peps:
  examine:
    - PEP structure and categories
    - Status workflow
    - Historical decisions
  patterns:
    - Standardized proposal format
    - Clear decision criteria
    - Implementation tracking
```

#### F.2 Architecture Decision Records
```yaml
adr/adr:
  location: https://github.com/adr/adr
  examine:
    - Template variations
    - Tool ecosystem
    - Example implementations

golang/go:
  examine:
    - /doc/go1.*.html (decision history)
    - Proposal process
    - Design documents
  patterns:
    - Proposal-driven development
    - Community review process
    - Compatibility promises

aws/aws-cdk:
  examine:
    - /design/* (design documents)
    - RFC process
    - Decision records
  patterns:
    - RFC-driven development
    - API design decisions
    - Breaking change management
```

#### F.3 Documentation Anti-Patterns
```
Search GitHub for:
- "TODO" OR "FIXME" (technical debt)
- "temporary" OR "hack" (shortcuts)
- "don't know" OR "not sure" (uncertainty)
- "legacy" OR "deprecated" (old code)
- "DO NOT TOUCH" (fragile code)

Common Anti-Pattern Locations:
- README files with "Coming soon"
- Docs folders with .gitkeep only
- Comments like "Ask Bob" (person dependency)
- Version 0.0.1 for years
- Last updated timestamps >2 years
```

#### F.4 Post-Mortem Collections
```yaml
Public Collections:
- danluu/post-mortems: 
  URL: https://github.com/danluu/post-mortems
  Content: Curated list of public postmortems

- hjacobs/kubernetes-failure-stories:
  URL: https://github.com/hjacobs/kubernetes-failure-stories
  Content: Kubernetes-specific failures

Example Structure to Extract:
- Timeline of events
- Root cause identification
- Contributing factors
- Mitigation steps
- Lessons learned
- Action items
```

---

END OF PROTOCOL WITH COMPLETE APPENDICES

Document Status: Complete with All Appendices
Next Step: Execute Phase 1 using these resources