# 4 — Performance (Full Rescue)

- [ ] Measure before changing anything: LCP, INP, CLS, bundle size.
- [ ] Remove unused dependencies and duplicated libraries.
- [ ] Code-split heavy views (PDF viewers, charts, editors).
- [ ] Lazy-load images with explicit dimensions; use modern formats.
- [ ] Check for render loops and unnecessary re-renders in React.
- [ ] Cache expensive Gemini responses where the input is identical.
- [ ] Add timeouts and retries to external API calls.
- [ ] Confirm no API call is made on every keystroke without debounce.
- [ ] Re-measure after changes and record the real numbers only.
- [ ] No percentage improvement is reported unless it was measured.
