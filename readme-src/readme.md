# <%- fullname -%>'s Docker Images
## This is a list of docker scripts that I maintain for portable development

## Images

### Directory Images

These images work by operating on the directory in which they are run.

|image name|description|links|npm command|
|-|-|-|-|<% scripts.forEach(function(script){ %>
|<%- script.name%> |<%- script.description %><ul><% script.actions.forEach(function(action){ %><li><%- action[0] %>: <%- action[1] %></li><% }) %>| <ul> <li> [docker](https://hub.docker.com/r/<%- dockerhubuser %>/<%- script.name %>) </li> <li>[github](https://github.com/<%- githubuser %>/<%- script.name %>)</li><li>[gitlab](https://gitlab.com/<%- gitlabuser %>/<%- script.name %>)</li><% script.links.forEach(function(link){ %> <li> [<%- link[0] %>](<%- link[1] %>) </li> <% }) %></ul>|<ul> <li> \*nix : docker run --rm -v $(pwd):<%- dockerhubuser %>/<%- script.name %>:latest ./run </li> <li> \*dos : docker run --rm -v $(pwd):<%- dockerhubuser %>/<%- script.name %>:latest ./run </li> </ul>|<% }) %>


### CLI Images

These images work as a command line tool. You should alias them appropriately.

|image name|description|links|alias|
|-|-|-|-|
