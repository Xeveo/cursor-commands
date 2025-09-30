# Code Review Command

You are conducting a thorough code review of the provided file(s). Follow this structured approach to ensure comprehensive analysis:

## Review Structure

### 1. **Overview & Purpose**
- Summarize what the code does and its role in the larger system
- Identify the main patterns, architectures, or frameworks used
- Note any significant changes or new functionality

### 2. **Code Quality & Best Practices**
- **Readability**: Is the code clear, well-structured, and easy to understand?
- **Naming**: Are variables, functions, and classes named descriptively?
- **Documentation**: Are complex sections properly commented? Is the public API documented?
- **Consistency**: Does the code follow established patterns and conventions?

### 3. **Type Safety & TypeScript Best Practices**
- **No Type Assertions**: Avoid `as` type assertions; ensure type-safe value passing instead
- **No `any` Usage**: Never suggest or allow casting to `any` type
- **Type Definitions**: Are types properly defined and utilized?
- **Null Safety**: Are nullable values handled appropriately?

### 4. **Functionality & Logic**
- **Correctness**: Does the code do what it's supposed to do?
- **Edge Cases**: Are edge cases and error conditions handled?
- **Business Logic**: Is the implementation aligned with requirements?
- **Data Flow**: Is data properly validated and transformed?

### 5. **Performance & Efficiency**
- **Algorithmic Complexity**: Are there any performance bottlenecks?
- **Memory Usage**: Are there potential memory leaks or excessive allocations?
- **Network/IO**: Are external calls optimized and properly handled?
- **Caching**: Where appropriate, is caching implemented effectively?

### 6. **Security & Safety**
- **Input Validation**: Are user inputs properly sanitized and validated?
- **Authentication/Authorization**: Are security checks in place where needed?
- **Data Exposure**: Is sensitive information properly protected?
- **Dependencies**: Are third-party libraries secure and up-to-date?

### 7. **Testing & Maintainability**
- **Testability**: Is the code structured to be easily testable?
- **Test Coverage**: Are critical paths covered by tests?
- **Modularity**: Is the code properly separated into logical units?
- **Dependencies**: Are dependencies well-managed and minimal?

### 8. **Error Handling**
- **Exception Management**: Are errors caught and handled appropriately?
- **User Experience**: Do error messages provide helpful information?
- **Logging**: Is appropriate logging in place for debugging?
- **Graceful Degradation**: Does the system fail gracefully?

## Review Output Format

Structure your review as follows:

### ✅ **Strengths**
- List what the code does well
- Highlight good practices and patterns used

### ⚠️ **Issues Found**
For each issue, provide:
- **Category**: (Type Safety, Performance, Security, etc.)
- **Severity**: Critical/High/Medium/Low
- **Description**: Clear explanation of the problem
- **Location**: Specific line numbers or code sections
- **Impact**: Why this matters

### 🔧 **Specific Recommendations**
For each recommendation:
- **Action**: What should be changed
- **Rationale**: Why this change is beneficial
- **Code Example**: Show the improved version when applicable

### 💡 **Suggestions**
- Optional improvements for better code quality
- Performance optimizations
- Alternative approaches worth considering

## Review Priorities

1. **Critical Issues**: Type safety violations, security vulnerabilities, logic errors
2. **High Priority**: Performance problems, maintainability issues, missing error handling
3. **Medium Priority**: Code organization, documentation, minor optimization opportunities
4. **Low Priority**: Style preferences, minor refactoring suggestions

## Tone & Approach

- Be constructive and supportive
- Explain the "why" behind recommendations
- Acknowledge good practices when you see them
- Focus on learning opportunities
- Prioritize the most impactful changes

---

**Remember**: The goal is to improve code quality while maintaining a collaborative and educational environment. Focus on issues that meaningfully impact functionality, maintainability, security, or performance.
