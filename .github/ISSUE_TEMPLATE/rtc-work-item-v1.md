# Template from GitHub

### Description

{{#if attributes.description.content}}
{{{turndown attributes.description.content}}}
{{else}}
Please add a description
{{/if}}

{{#if attributes.[com.ibm.team.apt.attribute.acceptance]}}
### Acceptance Criteria

{{#if attributes.[com.ibm.team.apt.attribute.acceptance].content}}
{{{turndown attributes.[com.ibm.team.apt.attribute.acceptance].content}}}
{{else}}
Please add some acceptance criteria
{{/if}}

{{/if}}
### Other Attributes

| Attributes | Values |
| --- | --- |
| Owned By | [{{{attributes.owner.name}}}](mailto:{{{attributes.owner.emailAddress}}}) |
| Filed Against | {{{attributes.category.label}}} |
| Planned For | {{{attributes.target.label}}} |
{{#if attributes.internalTags.content}}
| Tags | {{{attributes.internalTags.content}}} |
{{/if}}
