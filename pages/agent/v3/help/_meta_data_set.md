### Usage

`buildkite-agent meta-data set <key> [value] [options...]`

### Description

Set arbitrary data on a build using a basic key/value store.

You can supply the value as an argument to the command, or pipe in a file or
script output.

### Example

    $ buildkite-agent meta-data set "foo" "bar"
    $ buildkite-agent meta-data set "foo" < ./tmp/meta-data-value
    $ ./script/meta-data-generator | buildkite-agent meta-data set "foo"

### Options

* `--job value` - Which job's build should the meta-data be set on [`$BUILDKITE_JOB_ID`]
* `--agent-access-token value` - The access token used to identify the agent [`$BUILDKITE_AGENT_ACCESS_TOKEN`]
* `--endpoint value` - The Agent API endpoint (default: "https://agent.buildkite.com/v3") [`$BUILDKITE_AGENT_ENDPOINT`]
* `--no-http2` - Disable HTTP2 when communicating with the Agent API. [`$BUILDKITE_NO_HTTP2`]
* `--debug-http` - Enable HTTP debug mode, which dumps all request and response bodies to the log [`$BUILDKITE_AGENT_DEBUG_HTTP`]
* `--no-color` - Don't show colors in logging [`$BUILDKITE_AGENT_NO_COLOR`]
* `--debug` - Enable debug mode [`$BUILDKITE_AGENT_DEBUG`]
* `--experiment value` - Enable experimental features within the buildkite-agent [`$BUILDKITE_AGENT_EXPERIMENT`]
* `--profile value` - Enable a profiling mode, either cpu, memory, mutex or block [`$BUILDKITE_AGENT_PROFILE`]

