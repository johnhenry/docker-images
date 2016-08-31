# John Henry's Docker Images
## This is a list of docker scripts that I maintain for portable development

## Images

### Directory Images

These images work by operating on the directory in which they are run.

|image name|description|links|npm command|
|---|---|---|---|
|readme-generator |generate a readme using an ejs template<ul><li>reads: PROJECT/readme-src/data.json</li><li>reads: PROJECT/readme-src/readme.md</li><li>writes: PROJECT/readme.md</li>| <ul> <li> [docker](https://hub.docker.com/r/johnhenry/readme-generator) </li> <li>[github](https://github.com/johnhenry/readme-generator)</li><li>[gitlab](https://gitlab.com/johnhenry/readme-generator)</li></ul>|<ul> <li> \*nix : docker run --rm -v $(pwd):johnhenry/readme-generator:latest ./run </li> <li> \*dos : docker run --rm -v $(pwd):johnhenry/readme-generator:latest ./run </li> </ul>|


### CLI Images

These images work as a command line tool. You should alias them appropriately.

|image name|description|links|alias|
|---|---|---|---|
