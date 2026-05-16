# Automation Coding Standards

This repository follows maintainable and QA-focused automation engineering practices.

---

# Framework Principles

- Keep tests independent
- Avoid hardcoded waits
- Prefer reusable utilities
- Use maintainable selectors
- Keep assertions meaningful
- Improve debugging visibility

---

# Locator Strategy

Preferred locator order:

1. accessibility id
2. stable test id
3. unique css selector
4. xpath only if necessary

Avoid brittle locators.

---

# Wait Strategy

- Prefer explicit waits
- Avoid unnecessary pauses
- Use framework wait utilities
- Reduce flaky execution behavior

Bad Example:

```js
browser.pause(5000)
```

Preferred:

```js
await element.waitForDisplayed()
```

---

# Page Object Standards

- Keep selectors centralized
- Separate page logic from test logic
- Avoid duplicated actions
- Keep methods reusable

---

# Assertion Standards

- Assertions must be readable
- Validate business behavior
- Avoid weak assertions

---

# Reporting & Debugging

- Capture useful logs
- Preserve screenshots on failure
- Keep failures reproducible
- Improve CI debugging visibility

---

# Engineering Philosophy

This framework emphasizes:

- Maintainability
- Stability
- Scalability
- QA engineering mindset
- Reliable automation
