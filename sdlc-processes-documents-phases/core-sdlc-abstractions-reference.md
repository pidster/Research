# Core SDLC Abstractions Reference

## 30 Unified Processes (ISO/IEC/IEEE 12207:2017)

### 1. Agreement Processes (2 processes)
- **Acquisition Process** - Obtain products/services meeting stakeholder needs
- **Supply Process** - Deliver conforming solutions to acquirers

### 2. Organizational Project-Enabling Processes (6 processes)
- **Life Cycle Model Management Process** - Define and maintain organizational process assets
- **Infrastructure Management Process** - Provide necessary facilities, tools, and technologies
- **Portfolio Management Process** - Align projects with strategic objectives
- **Human Resource Management Process** - Ensure competent staffing
- **Quality Management Process** - Assure products meet standards
- **Knowledge Management Process** - Capture and share organizational learning

### 3. Technical Management Processes (8 processes)
- **Project Planning Process** - Produce and communicate effective plans
- **Project Assessment and Control Process** - Monitor performance and direct corrective action
- **Decision Management Process** - Structure critical decisions using criteria and alternatives
- **Risk Management Process** - Identify, analyse, treat, and monitor risks
- **Configuration Management Process** - Maintain integrity of all project outputs
- **Information Management Process** - Provide timely, complete, valid information
- **Measurement Process** - Collect and analyse process and product data
- **Quality Assurance Process** - Provide independent verification of requirements and plans

### 4. Technical Processes (14 processes)
- **Business or Mission Analysis Process** - Understand the business problem
- **Stakeholder Needs and Requirements Definition Process** - Capture stakeholder needs
- **System/Software Requirements Definition Process** - Transform needs into technical requirements
- **Architecture Definition Process** - Define system architecture
- **Design Definition Process** - Create detailed design
- **System Analysis Process** - Analyse system properties
- **Implementation Process** - Realise specified system elements
- **Integration Process** - Combine elements into complete system
- **Verification Process** - Confirm conformance to specifications
- **Transition Process** - Establish capability in operational environment
- **Validation Process** - Confirm fitness for intended use
- **Operation Process** - Use system to deliver services
- **Maintenance Process** - Sustain capability to provide service
- **Disposal Process** - End existence of system element

---

## 7 Generic Document Types & 73+ Information Items (ISO/IEC/IEEE 15289:2019)

### 1. Descriptions (42 types)
**System/Software Architecture & Design:**
- System Architecture Description
- Software Architecture Description
- Design Description
- Database Design Description
- Interface Description
- System Element Description

**Operational Concepts:**
- Concept of Operations
- Operational Concept
- System Operational Concept

**Process & Procedures:**
- Process Description
- Procedure Description

**Other Descriptions:**
- Function Description
- Object Description
- Component Description
- Module Description
- Data Structure Description
- Algorithm Description
- Service Description
- Use Case Description
- Test Environment Description
- Infrastructure Description
- Tool Description
- Technology Description
- Stakeholder Description
- Organization Description
- Project Context Description
- Risk Description
- Assumption Description
- Constraint Description
- Dependency Description
- Interface Control Description
- Integration Context Description
- Migration Description
- Training Material Description
- User Documentation
- Administrator Documentation
- API Documentation
- Configuration Description
- Deployment Description
- Security Description
- Performance Description
- Reliability Description

### 2. Plans (19 types)
- Acceptance Plan
- Acquisition Plan
- Capacity Plan
- Configuration Management Plan
- Development Plan
- Improvement Plan
- Information Management Plan
- Information Security Plan
- Integration Plan
- Maintenance Plan
- Project Management Plan
- Quality Management Plan
- Release Plan
- Risk Management Plan
- Service Continuity and Availability Plan
- Training Plan
- Transition Plan
- Validation Plan
- Verification Plan

### 3. Policies (2 primary types)
- Life-Cycle Policy
- Quality Management Policy
- (Additional organizational policies as needed: Security Policy, Coding Standards, Branching Strategy, Definition of Done, Acceptable Use Policy)

### 4. Procedures (14 types)
- Configuration Management Procedure
- Implementation Procedure
- Incident Management Procedure
- Information Management Procedure
- Maintenance Procedure
- Measurement Procedure
- Problem Management Procedure
- Quality Management Procedure
- Supplier Management Procedure
- Test Procedure
- Transition Procedure
- Validation Procedure
- Verification Procedure
- Review Procedure (Management, Technical, Inspection, Walk-through, Audit)

### 5. Reports (13 types)
- Acceptance Report
- Configuration Status Report
- Evaluation Report
- Incident Report
- Installation Report
- Integration and Test Report
- Monitoring and Control Report
- Problem Report
- Process Improvement Report
- Progress Report
- Service Report
- Validation Report
- Verification Report

### 6. Requests (4 primary types)
- Change Request
- Request for Proposal (RFP)
- Resource Request
- Risk Action Request
- (Modern additions: User Stories, Bug Reports, Feature Requests, Enhancement Proposals)

### 7. Specifications (4 primary types per ISO/IEC/IEEE 29148:2018)
- System Operational Concept (stakeholder needs)
- Stakeholder Requirements Specification (stakeholder requirements)
- System Requirements Specification (system requirements)
- Software Requirements Specification (software requirements)
- (Additional: Interface Specifications, Data Specifications, Performance Specifications, Security Specifications, Test Specifications)

### 8. Records (15 types)
- Anomaly Record
- Audit Record
- Configuration Item Record
- Decision Record
- Enabling System Record
- Maintenance Record
- Measurement Record
- Meeting Record
- Milestone Record
- Performance Record
- Risk Record
- Stakeholder Record
- Test Record
- Training Record
- Verification/Validation Record

---

## Essential SDLC Phases

### 5-Phase Model (Most Consolidated)
1. **Planning** - Establish project foundation, scope, feasibility
2. **Analysis & Design** - Requirements definition and solution architecture
3. **Implementation** - Build and integrate the system
4. **Testing & Deployment** - Verify, validate, and release
5. **Maintenance** - Operate and sustain the system

### 6-Phase Model (Common Traditional)
1. **Planning/Initiation** - Project charter, feasibility, initial scope
2. **Analysis/Requirements** - Stakeholder needs, system requirements
3. **Design** - Architecture and detailed design
4. **Implementation/Development** - Coding and unit testing
5. **Testing** - Integration, system, and acceptance testing
6. **Deployment/Maintenance** - Release, operations, and support

### 7-Phase Model (Most Granular)
1. **Initiation/Conception** - Initial idea, business case, feasibility
2. **Planning** - Detailed project planning, resource allocation
3. **Analysis/Requirements** - Requirements elicitation and specification
4. **Design/Architecture** - System architecture and component design
5. **Implementation/Construction** - Development and integration
6. **Testing/Validation** - All levels of testing and quality assurance
7. **Deployment/Operations** - Release, transition, maintenance, retirement

### Phase Variations by Methodology

**Waterfall (Sequential):**
- Executes phases in strict sequence
- Comprehensive documentation at phase gates
- Limited iteration between phases

**Agile (Iterative):**
- Compresses all phases into 1-4 week sprints
- Minimal documentation, maximum working software
- Continuous cycling through phases

**DevOps (Continuous):**
- Phases blur into continuous flow
- Automated transitions between phases
- No distinct phase boundaries

**Hybrid (Adaptive):**
- Sequential for planning/analysis
- Iterative for design/implementation
- Continuous for deployment/maintenance

---

## Core Process Minimums

### 10 Essential Processes (Absolute Minimum)
1. Requirements Definition
2. Architecture Definition
3. Design Definition
4. Implementation
5. Verification
6. Integration
7. Transition/Deployment
8. Project Planning
9. Risk Management
10. Configuration Management

### Additional High-Priority Processes
- Stakeholder Needs Definition
- Validation
- Quality Assurance
- Maintenance
- Project Assessment and Control

---

## Key Statistics & Validation

### Methodology Adoption (2024)
- 71% use Agile methodologies
- 42% use hybrid approaches
- 36% incorporate DevOps
- 28% use Waterfall (only 9% pure)
- 22% of enterprises use no mandated framework

### Success Metrics
- Agile: 64% success rate, 9% failure rate
- Waterfall: 49% success rate, 29% failure rate
- 60% average revenue/profit increase after Agile adoption

### Documentation Challenges
- 78% struggle with outdated/insufficient documentation
- 64% spend 4+ hours weekly searching for information
- 57% cite poor documentation as major productivity blocker

### Standards Harmonisation Timeline
- 1995: ISO/IEC 12207 first published
- 2008: Major revision (43 processes)
- 2015: ISO/IEC/IEEE 15288 harmonised
- 2017: ISO/IEC/IEEE 12207 harmonised (30 processes)
- 2024: SWEBOK V4.0 aligned with ISO standards
- 2027: Next anticipated ISO/IEC/IEEE 12207 revision

---

*Note: This reference synthesises formal standards (ISO/IEC/IEEE 12207:2017, ISO/IEC/IEEE 15289:2019, ISO/IEC/IEEE 29148:2018), industry frameworks (PMBOK, BABOK, ITIL), and empirical evidence from the 17th State of Agile Report and industry surveys.*
