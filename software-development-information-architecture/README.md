# Software Engineering Information Architecture

In this research I used AI (Claude 4.1 in research and extended thinking mode) to analyse the software development lifecycle.

The initial prompt:

    I've uploaded an information architecture research report. It reveals that 
    45-70% of software development work involves cognitive biases, 22-49% of 
    code commits contain undocumented knowledge, and systematic information 
    gaps at SDLC transition points are primary drivers of project failure. The 
    report maps all information required across 10 SDLC phases through three 
    fundamental layers (Formal/Explicit, Tacit/Implicit, and Emergent/Contextual), 
    analyzes five critical handoff points where knowledge is systematically 
    lost, documents cognitive biases affecting 45.72% of developer actions, 
    examines Conway's Law and organizational dynamics, and provides actionable 
    strategies including Architecture Decision Records, hypothesis-driven 
    development, and documentation-as-code practices to transform information 
    capture from afterthought to first-class concern.
    
The [information architecture research report](./information_architecture_3-layer_report.md) was produced in a prior session, with a significantly more loose approach to generation.

I then prompted Claude as follows:

    I want to analyse, model and prototype an information architecture (via a 
    mixed methods, literature review, systematic review, meta-analysis 
    research) that describes precisely and completely the information required 
    to design, build, deploy and operate a piece of software that (perhaps 
    eventually) successfully achieves an outcome that meets a business need. 

    We should consider how humans have performed this activity and our analysis
    should consider what parts of that information may have been subtly elided
    or omitted from written records because humans err and sometimes retain
    information in individual and collective memory, instead of recording it in
    writing. 

    We should consider the role that theories (Naur, Programming as Theory
    Building 1985) and hypotheses play at various stages of the process and
    identify places where there is a risk of assumptions rather than logical
    analysis.

    I want to enumerate and validate these elements:
    * lifecycle processes
    * generic document types
    * SDLC phases

Claude responded by suggested a research approach that was partly interview-based, which isn't what I intended. I corrected this as follows:

    Let's omit the interviews for now and replace that with literature analysis,
    but broadly consider internet-based writing published by experts and thought
    leaders.

The results this time were more inline with my expectations, so I prompted:

    Next, generate an artefact that describes this question/method/approach in a
    format that is suitable for both you (AI/LLM) and a human to reproduce the
    research.

    After that, I will review the doc, then I expect we will perform the actual
    research.

The results were reasonable from a quick review, and then:

    Now perform this research

There's a little more inconsequential prompting as Claude seemed to be having some UI glitches and the document artefacts weren't being linked properly, but with this corrected the results are:

 1. [Research Protocol: Complete Information Architecture for Software Development](./information_architecture_research_protocol.md)
 2. [Information Architecture for Software Development: Research Findings and Synthesis](./information_architecture_research_findings.md)
 3. [A Complete Information Architecture for Software Development: A Mixed-Methods Analysis of Formal, Tacit, and Emergent Knowledge in the Software Development Life Cycle](./information_architecture_academic_paper.md)
 4. [Practical Implementation Guide: Complete Information Architecture for Software Development](./information_architecture_implementation_guide.md)

