# Summary

This is a brief reference to testing practices based on my own experience.

# Test strategy

Big, complex, long-term projects benefit from introducing testing from the start.

Projects with simple business logic may still succeed without dedicated testers.

# Requirements analysis

When testers participate in refinements, they help clarify vague requirements and identify conflicting or untestable statements.

# Manual testing

Manual exploratory testing remains the most effective type of testing, finding up to 80% of issues before release.

The more complex the business logic, the more crucial it is to have dedicated manual testers.

Some companies with complex products have tried to eliminate manual testers, and it didn’t work.

# Automated testing

Regular automated regression testing answers the question of whether there are regression issues.

Regular automated regression testing is vital for project success.

Automated end-to-end (E2E) regression testing may capture up to 10% of issues after minor code changes and up to 80% after major breaking changes.

Integrating automated tests into CI/CD enables regular, scheduled test runs, which dramatically save time compared to manual regression testing.

# Shift-left approach

The idea of this approach is to start testing activities as early as possible.

The most well-known activities are:
- Testing requirements (e.g., during refinements)
- Writing more faster tests (unit, mocked, integration) rather than slower E2E tests
- Testers participating in developers’ code reviews
- Integrating automated tests into CI/CD for regular test runs

# Reporting

Before creating tools to generate test reports, think about who will use them and when. Avoid wasting resources on developing tools that nobody needs.

It may be tempting to treat test run pipelines as a final report. However, considering pipeline results together with reported bugs and tester feedback provides a more accurate picture.

# Testers

Coordination between manual and automated testers speeds up the creation of automated tests and makes them more effective.

An automated tester who also performs manual testing understands the business logic better, which improves the quality of automated tests.

# Test cases and automated tests

Not every test case will be fully covered by an automated test.

In some projects, testers do not write test cases, and this may be acceptable.

Measuring automated test coverage in Agile projects is complex and may require additional resources: time, people, processes, and discipline.

# Interview

When interviewing automated testers, give them an example of an automated test and ask them to fix a known issue in the code, as well as modify it to achieve a different goal.

Programming languages and test automation tools are always secondary—consider candidates with experience in other languages and tools.

When interviewing experienced testers, avoid trivial or overly theoretical questions. Instead, ask about their experience, strategic decisions, and test frameworks. Also, ask them to explain and modify code in a prepared automated test.
