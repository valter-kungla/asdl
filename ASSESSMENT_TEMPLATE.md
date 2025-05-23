# ASDL Assessment Template

> *Self-assessment questionnaire for determining your organization's current Autonomous Software Development Level*

**Contributor: Claude (Anthropic) — Assessment methodology and templates**

---

## Organization Information

- **Organization Name**: _______________
- **Assessment Date**: _______________
- **Assessment Scope**: _______________
- **Team Size**: _______________
- **Primary Technology Stack**: _______________

---

## Current State Assessment

### Coding Practices

**Question**: What percentage of your code is currently generated or significantly assisted by AI?

- [ ] 0% - All code written manually by humans **(L0)**
- [ ] 1-20% - AI suggests completions, developers type most code **(L1)**  
- [ ] 21-50% - AI generates functions/methods, humans review and integrate **(L2)**
- [ ] 51-80% - AI implements features end-to-end, humans provide guidance **(L3)**
- [ ] 81-95% - AI handles most development, humans monitor and intervene **(L4)**
- [ ] 95%+ - AI writes code autonomously, humans provide strategic oversight **(L5)**

**Evidence/Tools Used**: _______________

### Testing Strategy

**Question**: How are tests created and maintained in your organization?

- [ ] Manually written by developers **(L0)**
- [ ] AI suggests test templates, developers complete them **(L1)**
- [ ] AI generates unit tests, developers review and modify **(L2)**
- [ ] AI creates comprehensive test suites, developers approve **(L3)**
- [ ] AI generates and maintains all tests, auto-adapts to code changes **(L4)**
- [ ] AI designs testing strategies and continuously improves test coverage **(L5)**

**Test Coverage**: ____% **AI-Generated Test %**: ____%

### Code Review Process

**Question**: How is code review handled in your development process?

- [ ] Human reviewers examine all changes manually **(L0)**
- [ ] Automated linting + human review **(L1)**
- [ ] AI highlights issues, humans make final decisions **(L2)**
- [ ] AI reviews and summarizes changes, humans approve/reject **(L3)**
- [ ] AI approves routine changes, humans handle complex cases **(L4)**
- [ ] AI manages entire review process with human oversight policies **(L5)**

**Average Review Time**: _____ hours **Auto-approval Rate**: ____%

### Deployment and Operations

**Question**: How are deployments to production handled?

- [ ] Manual deployment triggered by humans **(L0)**
- [ ] Automated pipeline triggered by humans **(L1)**
- [ ] AI-assisted deployment with human approval for production **(L2)**
- [ ] AI can deploy to production with human sign-off **(L3)**
- [ ] AI handles deployments and rollbacks autonomously **(L4)**
- [ ] AI manages entire release lifecycle and optimization **(L5)**

**Deployment Frequency**: _____ **Human Intervention Rate**: ____%

### Architecture and Design

**Question**: Who makes architectural decisions in your organization?

- [ ] Human architects design all systems **(L0)**
- [ ] AI suggests patterns, humans choose and implement **(L1)**
- [ ] AI proposes architectural changes, humans evaluate **(L2)**
- [ ] AI implements bounded architectural changes within constraints **(L3)**
- [ ] AI makes most architectural decisions with human oversight **(L4)**
- [ ] AI continuously evolves architecture based on requirements **(L5)**

**Recent AI Architectural Contributions**: _______________

---

## Capability Inventory

### Current Tools and Platforms

Check all that apply to your current development environment:

#### AI-Assisted Development
- [ ] GitHub Copilot
- [ ] Tabnine
- [ ] Amazon CodeWhisperer
- [ ] Cursor/Windsurf
- [ ] Other: _______________

#### Autonomous Agents
- [ ] Devin
- [ ] SWE-Agent
- [ ] AutoGPT
- [ ] LangGraph agents
- [ ] Custom agent systems
- [ ] Other: _______________

#### Testing and QA
- [ ] AI-generated unit tests
- [ ] Automated integration testing
- [ ] AI-driven security scanning
- [ ] Automated performance testing
- [ ] Other: _______________

#### DevOps and Infrastructure
- [ ] Infrastructure as Code (IaC)
- [ ] Automated CI/CD pipelines
- [ ] AI-driven monitoring and alerting
- [ ] Self-healing systems
- [ ] Auto-scaling infrastructure
- [ ] Other: _______________

---

## Risk and Governance Assessment

### Security and Compliance

**Question**: How do you ensure security and compliance with AI-generated code?

- [ ] Manual security reviews for all code
- [ ] Automated security scanning with human review
- [ ] AI-assisted security analysis with human approval
- [ ] Automated security enforcement with human oversight
- [ ] AI-managed security with comprehensive audit trails
- [ ] Fully autonomous security management with constitutional constraints

**Compliance Requirements**: _______________
**Audit Frequency**: _______________

### Error Handling and Recovery

**Question**: How does your system handle errors or failures?

- [ ] Manual investigation and resolution by humans
- [ ] Automated alerts with manual resolution
- [ ] AI-assisted diagnosis with human-implemented fixes
- [ ] AI-suggested fixes with human approval and implementation
- [ ] Automated fixes for routine issues, human escalation for complex ones
- [ ] Fully autonomous error detection, analysis, and resolution

**Mean Time to Recovery (MTTR)**: _____ **AI Resolution Rate**: ____%

---

## Future Readiness Assessment

### Cultural Readiness

Rate your organization's readiness (1-5 scale, 5 being highest):

- **Trust in AI systems**: ___/5
- **Willingness to adopt automation**: ___/5  
- **Risk tolerance for AI decisions**: ___/5
- **Investment in AI training/tools**: ___/5
- **Management support for AI initiatives**: ___/5

### Technical Infrastructure

Rate your current infrastructure capabilities (1-5 scale):

- **Monitoring and observability**: ___/5
- **Automated testing coverage**: ___/5
- **CI/CD pipeline maturity**: ___/5
- **Security and compliance automation**: ___/5
- **Documentation and knowledge management**: ___/5

---

## Assessment Results

### Current ASDL Level Determination

Based on your responses above, your organization appears to be at:

**Primary Level**: L___ 

**Evidence Summary**:
- Coding: _______________
- Testing: _______________  
- Review: _______________
- Deployment: _______________
- Architecture: _______________

### Mixed-Level Capabilities

Many organizations operate at different levels across different capabilities:

| Capability | Current Level | Target Level | Gap Analysis |
|------------|---------------|--------------|--------------|
| Coding | L___ | L___ | _____________ |
| Testing | L___ | L___ | _____________ |
| Code Review | L___ | L___ | _____________ |
| Deployment | L___ | L___ | _____________ |
| Architecture | L___ | L___ | _____________ |

---

## Improvement Roadmap

### Immediate Next Steps (0-3 months)

1. **Priority 1**: _______________
2. **Priority 2**: _______________
3. **Priority 3**: _______________

### Medium-term Goals (3-12 months)

1. **Target Level**: L___
2. **Key Capabilities to Develop**:
   - _______________
   - _______________
   - _______________

3. **Required Investments**:
   - **Tooling**: _______________
   - **Training**: _______________
   - **Infrastructure**: _______________

### Long-term Vision (1-3 years)

1. **Ultimate Target Level**: L___
2. **Strategic Initiatives**:
   - _______________
   - _______________
   - _______________

3. **Success Metrics**:
   - **Velocity**: _______________
   - **Quality**: _______________
   - **Risk**: _______________

---

## Risk Assessment and Mitigation

### Identified Risks

| Risk | Probability | Impact | Mitigation Strategy |
|------|-------------|--------|-------------------|
| _____________ | High/Med/Low | High/Med/Low | _____________ |
| _____________ | High/Med/Low | High/Med/Low | _____________ |
| _____________ | High/Med/Low | High/Med/Low | _____________ |

### Safety Measures Required

For your target autonomy level, ensure you have:

- [ ] Comprehensive audit logging
- [ ] Human override capabilities  
- [ ] Automated rollback mechanisms
- [ ] Security constraint enforcement
- [ ] Regular compliance reviews
- [ ] Incident response procedures

---

## Assessment Metadata

- **Completed by**: _______________
- **Role/Title**: _______________
- **Review Date**: _______________
- **Next Assessment Date**: _______________
- **Stakeholders Consulted**: _______________

---

## Appendix: Evidence Collection Guide

### Documentation to Gather
- Development metrics (velocity, defect rates, etc.)
- Tool usage analytics  
- Code review statistics
- Deployment frequency and success rates
- Security incident reports
- Developer satisfaction surveys

### Recommended Follow-up Actions
1. Share assessment with development team for validation
2. Benchmark against industry standards for your sector
3. Develop detailed implementation plan for next ASDL level
4. Establish measurement framework for tracking progress
5. Schedule regular reassessments (quarterly recommended)

---

*This assessment template is designed to be completed collaboratively by development teams, engineering managers, and organizational leadership to ensure comprehensive evaluation of autonomous development capabilities.* 