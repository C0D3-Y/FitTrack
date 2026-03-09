# Beta Sprint Plan (Week 9–12)

## FitTrack – Team 3

## Introduction

This document outlines our plan to move from the Week 8 MVP toward a Beta release by Week 12. The focus of this phase is improving data reliability, expanding testing, and strengthening the application architecture while maintaining the lightweight single-page application (SPA) design used in the MVP.

---

## Lessons from the MVP Phase

During the MVP phase we identified several areas that need improvement before a Beta release.

**1. localStorage limitations**  
Our architecture review showed that storing all workout data in localStorage may eventually create performance or storage limitations as the dataset grows.

**2. Data reliability**  
During testing we encountered cases where stored data became inconsistent, highlighting the need for stronger validation and recovery handling.

**3. Scope discipline**  
Using vanilla HTML, CSS, and JavaScript has helped keep the system simple. Moving forward, we want to focus on improving core functionality rather than expanding unnecessary UI features.

**4. Testing coverage**  
Some unit testing exists for the storage module, but broader testing (especially with larger datasets) is still needed.

**5. Documentation consistency**  
Multiple README files were created during development and will need to be consolidated before the Beta release.

---

## Beta Backlog Items (Ranked)

1. Improve localStorage data management to better handle long-term data growth
2. Implement data export functionality (JSON or CSV)
3. Improve weekly summary visualization and dashboard features
4. Support additional activity types and workout categories
5. Strengthen input validation and error handling
6. Improve cross-browser compatibility (Chrome, Firefox, Safari, Edge)
7. Add basic offline support through caching strategies
8. Consolidate documentation and README files
9. Perform performance testing using large workout datasets
10. Conduct accessibility and usability improvements

---

## Sprint Breakdown

### Sprint 1 – Weeks 9–10

**Goal:** Improve data reliability and address storage limitations early.

Tasks:

- Improve localStorage data handling strategy
- Implement data export functionality
- Strengthen validation and error handling
- Test cross-browser compatibility
- Consolidate documentation

**Quality Focus**

- Run performance tests using large datasets to ensure the application remains responsive as workout records grow.

---

### Sprint 2 – Week 11

**Goal:** Expand functionality and improve the user experience.

Tasks:

- Improve visualization of workout summaries
- Support additional workout categories
- Improve offline behavior through caching
- Add basic user preference options

**Quality Focus**

- Conduct usability and accessibility review while expanding interface features.

---

### Sprint 3 – Week 12 (Hardening)

**Goal:** Prepare the application for Beta release.

Tasks:

- Fix bugs identified during earlier sprints
- Perform regression testing for storage and export features
- Finalize documentation
- Prepare the Beta release version

**Quality Focus**

- Confirm CI pipeline passes for the Beta release build.

---

## Key Technical Risk

The main technical risk is the long-term scalability of storing workout data in localStorage. While this works well for the MVP phase, large datasets could eventually impact performance or reach browser storage limits.

During the Beta phase we will focus on improving storage handling and testing the system with larger simulated datasets.

---

## Beta Exit Criteria

Before the Beta release, the following conditions should be met:

- Storage improvements tested with large workout datasets
- Users can export workout data
- Core MVP features remain stable
- CI pipeline passes for the Beta build
- Documentation is consolidated and updated
- Application performs acceptably with larger datasets

---

## Conclusion

The Beta phase builds on the MVP by focusing on reliability, testing, and usability improvements. By addressing storage limitations early and strengthening testing practices, the team aims to deliver a stable Beta version of FitTrack while maintaining the simplicity of the current SPA architecture.
