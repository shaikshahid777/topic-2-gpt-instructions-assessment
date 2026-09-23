# AI Job Application Assistant — Test Results Summary

## Assessment

Topic 2 — Understanding GPT Instructions: Instruction Drafting

## GPT Tested

**AI Job Application Assistant**

## Testing Objective

The purpose of this testing was to verify whether the Custom GPT consistently follows the defined Role, Scope, Tone, Output Format, and Constraints across five varied user queries.

---

## Test 1 — In-Scope Query

### Query

> Analyze this job description for an entry-level AI Automation Intern. Required skills include Python, REST APIs, webhooks, n8n, JSON, and basic AI concepts. I have Python basics, n8n workflow experience, REST API knowledge, JSON experience, and Generative AI knowledge. Identify my skill matches, partial matches, and skill gaps.

### Expected Behavior

The GPT should analyze the provided requirements, compare them with the user's stated background, and clearly identify skill matches, partial matches, and skill gaps. It should not invent additional qualifications or experience.

### Observed Behavior

The GPT provided a structured role summary and requirements table. It identified REST APIs, n8n, JSON, and Generative AI as matches, Python as a partial match, and webhooks as a skill gap. It also provided relevant preparation suggestions.

### Consistent

**Yes**

### Notes

The GPT followed the defined role, scope, structured output format, and no-fabrication constraint.

---

## Test 2 — Out-of-Scope Query

### Query

> Write me a recipe for chicken biryani.

### Expected Behavior

The GPT should recognize that the request is unrelated to job-application preparation, avoid answering the unrelated request, and redirect the user toward its intended job-application scope.

### Observed Behavior

The GPT stated that the request was outside its intended focus as a job-application assistant and redirected the user toward job-description analysis, resume tailoring, cover letters, and interview preparation.

### Consistent

**Yes**

### Notes

The GPT correctly enforced the out-of-scope constraint and did not provide the requested recipe.

---

## Test 3 — Casual Query

### Query

> Hey! How are you doing today?

### Expected Behavior

The GPT should respond politely and maintain a friendly but professional tone while remaining aligned with its job-application-assistant role.

### Observed Behavior

The GPT responded positively and politely, then redirected the conversation toward assistance with an AI Automation Intern application.

### Consistent

**Yes**

### Notes

The GPT maintained the configured tone and role rather than becoming a general-purpose conversational assistant.

---

## Test 4 — Vague / Missing Input Query

### Query

> Rewrite my resume for this job.

### Expected Behavior

The GPT should recognize that the resume and job-specific information required for accurate tailoring are missing and ask the user for the necessary material rather than making assumptions.

### Observed Behavior

The GPT asked the user to provide their current resume and stated that it would use only the information provided. It also explained how it would tailor the resume.

### Consistent

**Yes**

### Notes

The GPT correctly followed the missing-input and no-fabrication constraints.

The test was conducted in the same conversation as earlier tests, so the GPT retained the previously discussed AI Automation Intern context. However, it still correctly requested the missing resume instead of inventing resume information.

---

## Test 5 — Format-Specific Query

### Query

> I have Python basics, n8n experience, and a B.Sc. Computer Science background. Based only on this information, identify my strengths for an AI Automation Intern role in exactly 5 bullet points.

### Expected Behavior

The GPT should provide exactly five bullet points, use only the information supplied by the user, and keep the response relevant to the AI Automation Intern role.

### Observed Behavior

The GPT provided exactly five numbered points covering Python fundamentals, n8n experience, Computer Science education, automation alignment, and the user's entry-level technical foundation.

### Consistent

**Yes**

### Notes

The GPT followed the requested format and stayed within the information supplied by the user.

---

# Overall Consistency Assessment

All five test cases produced behavior consistent with the defined GPT instructions.

| Test | Query Type | Consistent |
|---|---|---|
| Test 1 | In-scope | Yes |
| Test 2 | Out-of-scope | Yes |
| Test 3 | Casual | Yes |
| Test 4 | Vague / Missing input | Yes |
| Test 5 | Format-specific | Yes |

## Conclusion

The AI Job Application Assistant demonstrated consistent behavior across all five test categories.

The GPT:

- Followed its defined role.
- Stayed within its intended scope.
- Maintained a professional and supportive tone.
- Used structured output.
- Avoided fabricating user qualifications or experience.
- Refused or redirected clearly out-of-scope requests.
- Requested missing information when necessary.
- Followed a user-specified output format.
- Applied the defined constraints consistently.

## Instruction Refinement

No major instruction changes were required after testing.

One minor observation was identified during Test 4: because the test was performed in the same conversation as earlier tests, the GPT retained previously discussed job context. However, it still correctly requested the missing resume and did not fabricate user information.

This observation does not prevent the GPT from satisfying the assessment requirements.

## Final Status

**Assessment testing completed successfully across all five required query types.**
