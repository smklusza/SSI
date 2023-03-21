---
created: <% tp.date.now("MMM Do YYYY HHmmss") %>
type: project
status: <% await tp.system.suggester(["proposed", "inProgress", "completed"], ["proposed", "inProgress", "completed"]) %>
published: false
tag: <% await tp.system.suggester(["gitHub", "SSI", "priorityIndex"], ["gitHub", "SSI", "priorityIndex"]) %>
priority: <% await tp.system.suggester(["high", "medium", "low"], ["high", "medium", "low"]) %>
parentalNote: <% tp.system.prompt("Is this a parental note?") %>
---

%%

Parent:: 
Child::
Sibling::
Friend::

%%

# Title: [[<% tp.file.title %>]]

# Note created: <% tp.file.creation_date() %>

## Tags: #project

# Notes:
