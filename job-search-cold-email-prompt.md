# Job Search Cold Email Prompt for Claude

Use this prompt to find active job postings, identify hiring managers, and create Gmail draft cold emails for each role.

---

## Prompt

I'm doing a job search and want you to find active job postings that match my target role, identify hiring managers, and create Gmail draft cold emails for each one.

## My Background
[Describe yourself -- e.g., "Former Amazon Principal (L7) with 14+ years across strategy, operations, supply chain, and finance. Most recently led planning for Amazon's 4.5B-unit North America network."]

## Target Roles
Search for active postings at the following seniority levels:
- [e.g., Director, VP, Senior Director, Sr. Manager]

In these functions:
- [e.g., Supply Chain, Operations, Procurement, S&OP, Manufacturing]

## Companies to Skip
Do not draft emails for any of these companies (already contacted):
- [List company names]

## Search Instructions
1. Search for active job postings using site: searches on:
   - job-boards.greenhouse.io
   - jobs.lever.co
   - jobs.ashbyhq.com
   - boards.greenhouse.io

2. For every URL you find, verify it is still active before drafting:
   - Greenhouse: if the URL redirects to ?error=true, it is EXPIRED -- skip it
   - Lever: fetch the URL; if it returns content with a job title, it is ACTIVE
   - Ashby: JS-rendered; if og:title meta tag has a job title, it is likely ACTIVE

3. For each confirmed active role, find the hiring manager -- the person the role reports to, based on the job description's "reporting to" line. Search LinkedIn and the web for their name and LinkedIn profile URL.

## Email Template
Use this exact HTML template for every draft:

```html
<p>Hi [HM First Name].</p>
<p>I know your time's valuable so I'll be brief.</p>
<p>The [Role Title] <a href="[JOB_POSTING_URL]">role</a> at [Company] looks closely aligned with my background. [One sentence summary of your background]. Would love to connect.</p>
<p>I've attached my resume for your reference.</p>
<p>Regards,<br>[Your Name]<br>Ph: [Your Phone]<br>Email: <a href="mailto:[Your Email]">[Your Email]</a></p>
```

Rules:
- Hyperlink the word "role" in the body to the actual job posting URL
- Subject line format: [Company] [Role Title] Role
- No em dashes anywhere (including subject lines)
- No "Not X but Y" phrasing
- Always greet with "Hi [First Name]." (period, not comma)

## Gmail Draft Settings
- TO field: [your-email@gmail.com] (placeholder -- you will manually replace with HM email)
- Create one draft per role
- Never send -- only create drafts

## Deliverables
After all drafts are created, provide a list of all hiring managers sorted alphabetically by last name, formatted as:

1. **[First Last]** ([Company], [HM Title]) -- [LinkedIn URL]
2. ...

---

## How This Works

Claude will:
1. Run site: searches across Greenhouse, Lever, and Ashby job boards
2. Fetch each job URL to verify the posting is still active (expired Greenhouse listings redirect to ?error=true)
3. Search LinkedIn and the web to identify the hiring manager for each role
4. Create a Gmail draft for each active role using the template above
5. Return an alphabetical list of all hiring managers with their LinkedIn profiles

## Tips
- Connect your Gmail MCP before running (required for draft creation)
- The more specific your target role and function, the better the results
- Review each draft and manually add the real hiring manager email before sending
- If Claude cannot find a direct HM, it will escalate to the next level up (e.g., CEO)
# Job Search Cold Email Prompt for Claude

Use this prompt to find active job postings, identify hiring managers, and create Gmail draft cold emails for each role.

---

## Prompt

I'm doing a job search and want you to find active job postings that match my target role, identify hiring managers, and create Gmail draft cold emails for each one.

## My Background
[Describe yourself -- e.g., "Former Amazon Principal (L7) with 14+ years across strategy, operations, supply chain, and finance. Most recently led planning for Amazon's 4.5B-unit North America network."]

## Target Roles
Search for active postings at the following seniority levels:
- [e.g., Director, VP, Senior Director, Sr. Manager]

In these functions:
- [e.g., Supply Chain, Operations, Procurement, S&OP, Manufacturing]

## Companies to Skip
Do not draft emails for any of these companies (already contacted):
- [List company names]

## Search Instructions
1. Search for active job postings using site: searches on:
   - job-boards.greenhouse.io
   - jobs.lever.co
   - jobs.ashbyhq.com
   - boards.greenhouse.io

2. For every URL you find, verify it is still active before drafting:
   - Greenhouse: if the URL redirects to ?error=true, it is EXPIRED -- skip it
   - Lever: fetch the URL; if it returns content with a job title, it is ACTIVE
   - Ashby: JS-rendered; if og:title meta tag has a job title, it is likely ACTIVE

3. For each confirmed active role, find the hiring manager -- the person the role reports to, based on the job description's "reporting to" line. Search LinkedIn and the web for their name and LinkedIn profile URL.

## Email Template
Use this exact HTML template for every draft:

```html
<p>Hi [HM First Name].</p>
<p>The [Role Title] <a href="[JOB_POSTING_URL]">role</a> at [Company] looks closely aligned with my background. [One sentence summary of your background]. Would love to connect. I've attached my resume for your reference.</p>
<p>Regards,<br>[Your Name]<br>Ph: [Your Phone]<br>Email: <a href="mailto:[Your Email]">[Your Email]</a></p>
```

Rules:
- Hyperlink the word "role" in the body to the actual job posting URL
- Subject line format: [Company] [Role Title] Role
- No em dashes anywhere (including subject lines)
- No "Not X but Y" phrasing
- Always mention resume is attached
- Always greet with "Hi [First Name]." (period, not comma)

## Gmail Draft Settings
- TO field: [your-email@gmail.com] (placeholder -- you will manually replace with HM email)
- Create one draft per role
- Never send -- only create drafts

## Deliverables
After all drafts are created, provide a list of all hiring managers sorted alphabetically by last name, formatted as:

1. **[First Last]** ([Company], [HM Title]) -- [LinkedIn URL]
2. ...

---

## How This Works

Claude will:
1. Run site: searches across Greenhouse, Lever, and Ashby job boards
2. Fetch each job URL to verify the posting is still active (expired Greenhouse listings redirect to ?error=true)
3. Search LinkedIn and the web to identify the hiring manager for each role
4. Create a Gmail draft for each active role using the template above
5. Return an alphabetical list of all hiring managers with their LinkedIn profiles

## Tips
- Connect your Gmail MCP before running (required for draft creation)
- The more specific your target role and function, the better the results
- Review each draft and manually add the real hiring manager email before sending
- If Claude cannot find a direct HM, it will escalate to the next level up (e.g., CEO)
