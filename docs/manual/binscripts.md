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

<h2 class="script" id="at-confgen">at-confgen <span class="module">from adapt-authoring-config</span></h2><div class="details"><p class="description">Generates a template config file which can be populated with required values.</p><p><b>Params</b><ul><li><code>environment</code> The enviroment to write the config for</li><li><code>--defaults</code> Will include default values</li><li><code>--replace</code> Will override any existing values</li><li><code>--update</code> Will update existing configuration with any missing values</li></ul></p>
<h2 class="script" id="at-docgen">at-docgen <span class="module">from adapt-authoring-docs</span></h2><div class="details"><p class="description">Generates documentation for the installed modules.</p>
<h2 class="script" id="at-docserve">at-docserve <span class="module">from adapt-authoring-docs</span></h2><div class="details"><p class="description">Generates an HTTP server for viewing the local copy of the documentation (note these must be build first with `at-docgen`)</p><p><b>Params</b><ul><li><code>dir</code> The dir to serve (all dirs will be served by default)</li><li><code>--open</code> Will automate open the served folders in separate broser windows/tabs</li></ul></p>
<h2 class="script" id="at-langcheck">at-langcheck <span class="module">from adapt-authoring-lang</span></h2><div class="details"><p class="description">Checks for string usage</p>
<h2 class="script" id="at-test">at-test <span class="module">from adapt-authoring-testing</span></h2><div class="details"><p class="description">Runs the automated testing suite.</p><p><b>Params</b><ul><li><code>--modules=[modules...]</code> Comma separated list specifying which modules should be tested (all modules are tested by default).</li></ul></p>

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