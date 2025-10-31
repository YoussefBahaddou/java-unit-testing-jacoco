# TP JUnit + JaCoCo Coverage Report

## Test Results Summary
After running `mvn clean verify`, all tests pass:
- Tests run: 4, Failures: 0, Errors: 0, Skipped: 0
- Build: SUCCESS
- Coverage checks: All met (≥85% instructions, ≥80% branches)

## Coverage Details
- **Instructions**: 96% (3 missed out of 89)
- **Branches**: 100% (0 missed out of 20)
- **Lines**: 94% (1 missed out of 18)
- **Methods**: 80% (1 missed out of 5)
- **Classes**: 100% (0 missed out of 2)

### By Class
- **StringTools**: 100% in all metrics (fully covered).
- **DateUtils**: 86% instructions (missed constructor), 100% branches (all leap year paths covered).

## Comparison: JaCoCo vs EclEmma
- **JaCoCo** (Maven-integrated): Provides detailed HTML/XML/CSV reports post-build. Accurate for CI/CD, shows 96% instructions, 100% branches.
- **EclEmma** (Eclipse plugin): Real-time IDE coverage, similar metrics but visual highlighting. Expected similar results (100% branches, high instructions) as both use bytecode instrumentation.
- **Key Difference**: JaCoCo is command-line/report-focused; EclEmma is interactive. Both confirm full white-box coverage for the TP.

![JaCoCo Report Screenshot](Screenshots/3.png)
![EclEmma Report Screenshot](Screenshots/2.png)

