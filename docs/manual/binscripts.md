# Bin scripts
The authoring tool core bundle includes a number of useful scripts which make setting up and using the tool more straightforward. This page outlines these scripts and how they function, along with any parameters they may expect.

## Running a bin script

To run a bin script, you must use the npx command which comes bundled with npm which and used to execute node modules. Scripts are run using the following format: **npx** followed by the **script name**, with any **flags or parameters** coming at the end.

As an example, a task called `at-myscript` may be run like so:

> We prefix any core authoring tool scripts `at-` for transparency (as an added bonus they also come towards the top of the `bin/` folder in `node_modules`!).

```bash
npx at-myscript --test=true
```

See the [official npx docs](https://docs.npmjs.com/cli/v7/commands/npx) for more information on npx.

<h2 class="script" id="at-docgen">at-docgen <span class="module">from adapt-authoring-docs</span></h2><div class="details"><p class="description">Generates documentation for the installed modules.</p>
<h2 class="script" id="at-docserve">at-docserve <span class="module">from adapt-authoring-docs</span></h2><div class="details"><p class="description">Generates an HTTP server for viewing the local copy of the documentation (note these must be built first with `at-docgen`)</p>
<h2 class="script" id="at-integration-test">at-integration-test <span class="module">from adapt-authoring-integration-tests</span></h2><div class="details"><p class="description">Integration test runner. Must be run from the adapt-authoring app directory (where node_modules are installed). Usage: npx at-integration-test                    # run all tests npx at-integration-test auth               # run auth.spec.js npx at-integration-test mongodb content    # run mongodb.spec.js and content.spec.js CUSTOM_DIR=/path/to/custom npx at-integration-test Environment variables: CUSTOM_DIR - Path to a directory containing additional fixtures/ and/or tests/ Custom fixtures override built-in fixtures when keys collide.</p>
<h2 class="script" id="at-schemacheck">at-schemacheck <span class="module">from adapt-authoring-jsonschema</span></h2><div class="details"><p class="description">Checks for duplicate schema properties</p>

<style>
  h2.script {
    margin-bottom: 5px;   
  }
  h2.script .module {
    font-weight: 300;
    font-size: 16px;
    vertical-align: middle;
  }
  p.description,
  .details ul {
    margin: 0;   
  }
</style>