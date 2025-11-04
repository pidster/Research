# The Software Development Lifecycle (SDLC)

In this research, I'm analysing the SDLC, its processes, document types and phases and how the industry has described this formally, via specifications and standards. Practitioners know how complex this is and that the different standards have caused many lengthy debates, but most of us feel that there are commonalities - at least when we're feeling open-minded.

My first prompt:

    I want to describe the software development lifecycle (SDLC) in abstract form, 
    specifically I want to enumerate and validate these elements:
    
    1. lifecycle processes (including but not necessarily limited to: Agreement, 
      Organisational, Technical Management, Technical)
    2. generic document types (including but not necessarily limited to: Description,
      Plan, Policy, Procedure, Report, Request, Specification)
    3. SDLC phases: (including but not necessarily limited to: Planning, Analysis,
      Design, Implementation, Testing, and Maintenance)

    Analyze formal specifications of the SDLC and derive a common abstraction, using each of these three elements.

This produced the following: [Validated SDLC Abstractions: Formal Standards Meet Industry Practice](./validated-sdlc-abstractions.md).

In the next prompt I sought a simplified view:

    OK, now let's create a simplified artefact that documents just the 4 groups of
    30 unified processes (perhaps a list of lists would be a good way of organising
    this), the 7 document types and 73 items, the essential phases (you may describe
    variants 5-7 separately for comparative purposes).

This resulted in: [Core SDLC Abstractions Reference](./core-sdlc-abstractions-reference.md).

In the next iteration I start to consider how AI might impact this, so I prompted:

    We will now consider how AI can be used in this context, (considering the strengths
    and weaknesses of humans and of AI separately), using empirical research wherever
    possible to support our analysis. 

    Do not focus on the 2 agreement processes, portfolio, or human resources processes.

    We should assume that AI will be used to produce documents, that the document
    content will be rigorously checked by humans and AI, that those documents will
    feed other AI-based processes, and that our objective is to eliminate toil, and
    manual work that humans are unreliable at, by working out exactly what the human
    inputs need to be at each stage.

    We want to consider factors such as which are 'standing documents' produced once
    and iterated infrequently, which are dynamic, iterated frequently, which are
    produced singularly, which have many instances, and which are ephemerial,
    produced once, consumed quickly and then become less relevant.

Unfortunately, Claude hit the maximum length for this conversation at this stage. After starting another conversation in the same Claude project (which has a variety of documents provided as context, including the prior outputs above), with the same prompt (as above), the results were promising:

    Conclusion
    
    The empirical evidence strongly supports using AI to eliminate documentation toil
    while preserving human judgment for critical decisions. The key is recognising that
    70-80% of valuable knowledge is tacit and requires human interpretation, while the
    20-30% formal layer can be largely automated. By having AI generate comprehensive
    documentation that humans then validate and enrich with context, organisations can
    address both the documentation crisis (78% inadequacy) and the "bad day" factors
    that destroy developer productivity.

The full document: [AI Integration Framework for SDLC Processes](./ai-sdlc-integration-framework.md).




