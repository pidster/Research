# SDLC Information Architecture Diagrams

## 1. Information Architecture Layers

```mermaid
graph TB
    subgraph "Software Knowledge Distribution"
        F[Formal Layer<br/>20-30%<br/>AI Domain]
        T[Tacit Layer<br/>70-80%<br/>Human Domain]
        E[Emergent Layer<br/>Dynamic<br/>Organisational]
    end
    
    F --> |Documentation<br/>Code<br/>Standards| AUTO[Fully Automatable]
    T --> |Mental Models<br/>Experience<br/>Heuristics| HUMAN[Human Essential]
    E --> |Team Dynamics<br/>Culture<br/>Relationships| SOCIAL[Socially Constructed]
```

## 2. Document Type Mapping to Processes

```mermaid
flowchart LR
    subgraph "Document Types"
        D1[📋 Descriptions]
        D2[📊 Plans]
        D3[📜 Policies]
        D4[🔄 Procedures]
        D5[📈 Reports]
        D6[📝 Requests]
        D7[📑 Specifications]
    end
    
    subgraph "Process Phases"
        P1[Planning]
        P2[Analysis]
        P3[Design]
        P4[Implementation]
        P5[Testing]
        P6[Deployment]
        P7[Maintenance]
    end
    
    D6 --> P1
    P1 --> D2
    P1 --> D7
    
    D6 --> P2
    P2 --> D7
    P2 --> D1
    
    D7 --> P3
    P3 --> D1
    
    D1 --> P4
    P4 --> D4
    
    D7 --> P5
    P5 --> D5
    
    D2 --> P6
    P6 --> D4
    
    D5 --> P7
    P7 --> D6
```

## 3. Human-AI Contribution by Process

```mermaid
graph LR
    subgraph "High Human Contribution (>70%)"
        H1[Architecture Definition - 75%]
        H2[Risk Management - 70%]
        H3[Decision Management - 80%]
    end
    
    subgraph "Balanced (40-60%)"
        B1[Requirements Definition - 60/40]
        B2[Implementation - 50/50]
    end
    
    subgraph "High AI Contribution (>70%)"
        A1[Verification - 70%]
        A2[Configuration Mgmt - 80%]
        A3[Documentation Gen - 85%]
    end
```

## 4. Information Flow Through SDLC

```mermaid
stateDiagram-v2
    [*] --> Stakeholder_Needs
    
    Stakeholder_Needs --> Requirements: Human Understanding
    Requirements --> Architecture: Human Decisions + AI Docs
    Architecture --> Design: Human Trade-offs
    Design --> Implementation: 50/50 Human/AI
    Implementation --> Testing: AI Execution
    Testing --> Deployment: AI Automation
    Deployment --> Operations: AI Monitoring
    Operations --> Maintenance: Human Root Cause
    Maintenance --> Requirements: Feedback Loop
    
    note right of Requirements: 🔴 40-50% failures here
    note right of Architecture: 🟡 ADRs critical
    note right of Implementation: 🟢 AI reduces toil
    note right of Testing: 🟢 AI finds patterns
```

## 5. Document Lifecycle Patterns

```mermaid
graph TD
    subgraph "Standing Documents"
        SD1[Created Once] --> SD2[Updated Rarely]
        SD2 --> SD3[AI Maintains]
        SD3 --> SD4[Human Approves]
        
        SDT[Architecture, Policies, Standards]
    end
    
    subgraph "Dynamic Documents"
        DD1[Frequent Updates] --> DD2[AI Auto-generates]
        DD2 --> DD3[From Live Data]
        DD3 --> DD4[Human Reviews]
        
        DDT[Plans, Reports, Dashboards]
    end
    
    subgraph "Ephemeral Documents"
        ED1[Created] --> ED2[Consumed]
        ED2 --> ED3[Archived]
        ED3 --> ED4[AI Extracts Knowledge]
        
        EDT[PRs, Tickets, Requests]
    end
```

## 6. Critical Information Transitions

```mermaid
flowchart TB
    subgraph "Where Information is Lost"
        L1[Team Member Departure<br/>42% unique knowledge]
        L2[Phase Transitions<br/>Requirements → Design]
        L3[Documentation Decay<br/>78% inadequate]
        L4[Cognitive Biases<br/>45.72% of actions]
    end
    
    subgraph "AI Mitigation Strategies"
        M1[Continuous Documentation]
        M2[Traceability Matrices]
        M3[Auto-update from Code]
        M4[Bias Detection]
    end
    
    L1 --> M1
    L2 --> M2
    L3 --> M3
    L4 --> M4
```

## 7. Process-Document-Knowledge Matrix

| Process | Produces | Consumes | Knowledge Layer | Human/AI Split |
|---------|----------|----------|-----------------|----------------|
| **Requirements** | Specifications | Requests | Tacit (understand needs) | 60/40 |
| **Architecture** | Descriptions, ADRs | Specifications | Tacit (decisions) | 75/25 |
| **Design** | Descriptions | Specifications | Tacit (trade-offs) | 70/30 |
| **Implementation** | Code, Procedures | Descriptions | Mixed | 50/50 |
| **Verification** | Reports | Specifications | Formal (patterns) | 30/70 |
| **Deployment** | Procedures | Plans | Formal (automation) | 20/80 |
| **Maintenance** | Updates, Requests | Reports | Mixed | 40/60 |

## 8. Key Insights from Visualization

### Critical Findings:
1. **70-80% of knowledge is tacit** - Cannot be automated, requires human understanding
2. **Document types cluster by lifecycle** - Standing (rare updates), Dynamic (frequent), Ephemeral (single-use)
3. **Information loss points are predictable** - Phase transitions, departures, documentation decay
4. **Human/AI split varies by process** - Architecture (75% human) vs Configuration (80% AI)

### Optimal Integration Points:
- **Maximum AI Value**: Documentation generation, test execution, configuration management
- **Maximum Human Value**: Architecture decisions, risk identification, stakeholder understanding
- **Balanced Collaboration**: Requirements definition, implementation, maintenance

### Implementation Priority:
1. **Immediate**: Automate ephemeral document generation (PRs, tickets)
2. **Short-term**: AI-assisted dynamic documents (reports, dashboards)
3. **Medium-term**: AI maintenance of standing documents
4. **Long-term**: Tacit knowledge capture assistance

---

*These diagrams visualize the relationships between:*
- *30 unified processes (ISO/IEC/IEEE 12207:2017)*
- *7 document types (ISO/IEC/IEEE 15289:2019)*
- *3 knowledge layers (Formal/Tacit/Emergent)*
- *Human vs AI contribution ratios based on empirical research*