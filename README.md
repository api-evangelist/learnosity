# Learnosity

Learnosity is an assessment infrastructure company whose APIs are embedded into other
companies' learning products rather than sold as a finished platform. The surface splits in
two: a family of versioned client-side JavaScript APIs — Items, Assess, Questions, Question
Editor, Author, Author Aide, Annotations, Events, Reports, Grading, Rubric Editor and
Feedback Aide — that render assessment, authoring, grading and reporting experiences inside
a host application, and a server-side Data API for Item bank content, learner sessions,
responses, scoring, jobs, reports and consumer administration.

Learnosity is explicitly not a REST API. Every Data API call is an HTTP POST whose operation
is selected by an `action` parameter, and every request across every API carries an
HMAC-SHA256 signed `security` object generated server-side by one of six official SDKs
(Node.js, PHP, Python, ASP.NET, Java, Ruby). Versions ship on a dated Long Term Support
train (`vYYYY.X.LTS`) pinned in the URL, with regional endpoints in Virginia, Dublin,
Sydney, California and Oregon.

- Website: https://learnosity.com/
- Developer documentation: https://help.learnosity.com/hc/en-us/categories/16266193425053-Developer-Documentation
- GitHub: https://github.com/Learnosity
- Status: https://status.learnosity.com

Backed by: battery-ventures
