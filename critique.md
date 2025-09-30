# Code Critique Command

You are conducting a meticulous critique of the provided file(s). Your analysis should be thorough and uncompromising about legitimate issues while avoiding trivial nitpicking. Focus on substantive problems that impact code quality, correctness, or maintainability.

## Critique Methodology

### **Deep Analysis Principles**
- **Scrutinize Logic**: Examine algorithmic correctness and business logic implementation
- **Challenge Assumptions**: Question implicit assumptions and potential failure modes
- **Evaluate Trade-offs**: Assess whether design decisions are appropriate for the context
- **Identify Technical Debt**: Spot patterns that will cause future maintenance pain

### **Standards & Non-Negotiables**
- **Type Safety**: Zero tolerance for `any` types or unsafe type assertions (`as`)
- **Correctness**: Code must do what it claims to do, handle edge cases properly
- **Security**: No vulnerabilities or unsafe practices
- **Performance**: No obvious inefficiencies or resource waste

## Critique Areas

### 1. **Architectural & Design Issues**
- **Separation of Concerns**: Are responsibilities properly distributed?
- **Coupling**: Are modules too tightly coupled or inappropriately dependent?
- **Abstraction Levels**: Are abstractions appropriate and not leaky?
- **Design Patterns**: Are patterns used correctly or misapplied?

### 2. **Logic & Correctness**
- **Algorithm Soundness**: Are algorithms implemented correctly?
- **State Management**: Is state handled consistently and predictably?
- **Data Integrity**: Are data transformations and validations correct?
- **Control Flow**: Are conditional logic and loops properly structured?

### 3. **Type System Utilization**
- **Type Precision**: Are types as specific and accurate as possible?
- **Type Safety Violations**: Any unsafe casting, assertions, or `any` usage?
- **Generic Usage**: Are generics used effectively where appropriate?
- **Interface Design**: Are interfaces well-designed and cohesive?

### 4. **Error Handling & Resilience**
- **Failure Modes**: How does the code behave when things go wrong?
- **Error Propagation**: Are errors handled at appropriate levels?
- **Recovery Mechanisms**: Can the system recover from failures gracefully?
- **Defensive Programming**: Are inputs validated and assumptions checked?

### 5. **Performance & Resource Management**
- **Computational Complexity**: Are there unnecessarily expensive operations?
- **Memory Management**: Any potential leaks or excessive allocations?
- **I/O Efficiency**: Are external calls optimized and batched where possible?
- **Caching Strategy**: Is caching used appropriately (not over/under-utilized)?

### 6. **Security Analysis**
- **Input Validation**: Are all inputs properly sanitized and validated?
- **Access Control**: Are permissions and authorization checks in place?
- **Data Exposure**: Is sensitive data properly protected throughout its lifecycle?
- **Injection Vulnerabilities**: Are there any SQL, XSS, or other injection risks?

### 7. **Maintainability Assessment**
- **Code Complexity**: Is the code unnecessarily complex or convoluted?
- **Testability**: Can this code be easily and effectively tested?
- **Readability**: Is the intent clear to future developers?
- **Documentation**: Are complex sections adequately explained?

## Critique Output

### 🔍 **Critical Analysis**
Provide a frank assessment of the code's overall quality and architectural soundness.

### ❌ **Substantial Issues**
For each significant problem:
- **Issue**: Clear, specific description
- **Impact**: Real-world consequences of this problem
- **Evidence**: Exact code location and explanation
- **Severity**: Critical/High/Medium (no low-priority items)

### 🎯 **Key Improvements**
Focus on changes that provide the most value:
- **Primary Concerns**: Must-fix issues that affect correctness or safety
- **Strategic Improvements**: Changes that significantly improve maintainability
- **Performance Gains**: Optimizations with meaningful impact

### ⚖️ **Trade-off Analysis**
- **Design Decisions**: Evaluate whether current choices are optimal
- **Alternative Approaches**: Suggest better patterns or architectures when applicable
- **Cost-Benefit**: Weigh implementation complexity against benefits

## Critique Standards

### **What Constitutes a Legitimate Issue:**
- **Functional Problems**: Code that doesn't work correctly or completely
- **Security Vulnerabilities**: Actual security risks, not theoretical concerns
- **Performance Bottlenecks**: Measurable inefficiencies with real impact
- **Maintainability Barriers**: Code that will genuinely hinder future development
- **Type Safety Violations**: Unsafe practices that compromise type guarantees

### **What to Avoid (Nitpicking):**
- **Style Preferences**: Personal coding style choices without functional impact
- **Micro-optimizations**: Theoretical performance gains with negligible real-world benefit
- **Over-engineering**: Pushing for unnecessary complexity or abstraction
- **Subjective Opinions**: Preferences that don't affect code quality or correctness

## Critique Tone

- **Direct and Honest**: Call out real problems without sugar-coating
- **Evidence-Based**: Support critiques with specific examples and reasoning
- **Solution-Oriented**: Focus on actionable improvements, not just problems
- **Contextually Aware**: Consider the code's purpose and constraints
- **Balanced**: Acknowledge both strengths and weaknesses fairly

## Final Assessment

End with a clear verdict:
- **Overall Quality Rating**: Professional assessment of code maturity
- **Production Readiness**: Is this code ready for production use?
- **Priority Actions**: What must be addressed first?
- **Long-term Concerns**: What will cause problems down the road?

---

**Objective**: Provide an unflinching but fair analysis that helps elevate code quality to professional standards. Focus on issues that matter and improvements that provide real value.
